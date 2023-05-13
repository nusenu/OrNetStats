---
title: "How to setup your Authenticated Relay Operator ID (AROI)"
permalink: aroi-setup.html
hide_sidebar: true
---

There are two options to create your AROI:

* The **dns-rsa** proof type makes use of DNS TXT record(s).
* The **uri-rsa** proof type makes use of a text file served over HTTPS.

You can choose one option. If you do not own a DNS domain the second option is for you.

Make sure to keep your proof up to date when adding more relays.

You should be able to see your graph showing your set of relays on OrNetStats a day after creating your AROI.

# DNS TXT records option

**Requirements:**

* the domain must be DNSSEC signed

If your domain is not DNSSEC signed, use the **uri-rsa** proof type instead.

**Setup steps**

1. for every relay create a DNS TXT record following this scheme:
```
relayfingerprint.example.com value: "we-run-this-tor-relay"
```
The RSA SHA1 relay fingerprint is exactly 40 characters long and can be found in the file named 
"fingerprint" located in the tor data directory on your relay.

2. make sure your torrc ``ContactInfo`` line contains at least the following content on **all** your relays:

```
url:example.com proof:dns-rsa ciissversion:2
```

Replace "example.com" with your own domain.

It is fine to have other content in your torrc `ContactInfo` line as well.


# Text File served over HTTPS option

**Requirements:**

* you must be able to create a text file under the well-known URI:
/.well-known/tor-relay/rsa-fingerprint.txt
* the URI must allow robots to fetch it without requiring CAPTCHAs
* the webserver certificate must be valid and from a trusted certificate authority
* the URI must not redirect to another domain

**Setup Steps**

1. create the file **[/.well-known/tor-relay/rsa-fingerprint.txt](https://gitlab.torproject.org/tpo/core/torspec/-/blob/main/proposals/326-tor-relay-well-known-uri-rfc8615.md#well-knowntor-relayrsa-fingerprinttxt)** containing all your relay RSA fingerprints, one per line
and make it available via HTTPS.
2. make sure your torrc `ContactInfo` line contains at least the following content:

```
url:example.com proof:uri-rsa ciissversion:2 
```

Replace "example.com" with the correct domain that provides your `rsa-fingerprint.txt` file.

It is fine to have other content in your torrc `ContactInfo` line as well.

If you do not own a domain and webserver you can use 3rd party services like GitHub Pages to publish the text file.

Example by an operator:

https://hydra-family.github.io/.well-known/tor-relay/rsa-fingerprint.txt ([repo](https://github.com/hydra-family/hydra-family.github.io/blob/main/rsa-fingerprint.txt))

# Frequently Asked Questions (FAQ)

* What are the main benefits of creating an AROI for my relays?

  * You get a daily updated graph for your group of relays that allow you to see how your relays are doing. Example by another operator: [graph](https://nusenu.github.io/OrNetStats/nothingtohide.nl.html)
  * Impersonation Detecion: By creating an AROI we and you can easily detect misconfigurations or malicious entities that claim to be you by using your relay's `ContactInfo`
    because they will fail the AROI verification step.

* Do I need a (DNSSEC-signed) domain to setup my AROI?

No, a (DNSSEC-signed) domain is optional. You can serve a text file via HTTPS instead, but if you want to use the DNS TXT records option, your domain must be DNSSEC-signed.

* Do I need to run a webserver to create my AROI?

No, running a webserver is optional. You can serve the text file via public services like GitHub Pages or create DNS TXT records instead.

* How can I verify whether I did setup my AROI correctly?

  * After setting up your AROI (torrc ContactInfo + rsa-fingerprint.txt or DNS TXT records) wait for a day.
  * Then open [this OrNetStats page](https://nusenu.github.io/OrNetStats/w/misc/families-by-bandwidth.html) and search for your `ContactInfo` (ctrl-f),
    click on your entry and ensure every line shows the black checkbox in the second column. If it does not, either you have an error in your AROI setup or someone is trying to impersonate you.
    Verify the IP address of the given relay missing the checkbox in the second column is yours. If you need further help feel free to reach out to me.
