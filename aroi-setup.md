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

A day after creating or your AROI, you should be able to see your graph showing your set of relays on OrNetStats.

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

It is fine to have other content in your torrc ContactInfo line as well.


# Text file over HTTPS option 

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

