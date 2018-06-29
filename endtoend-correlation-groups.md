---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-06-29 08:00 UTC**

For each operator the list of running relays is shown (relays are linked to [Relay Search](https://metrics.torproject.org/rs.html)).
Operators and relays are sorted from more relevant to less relevant. More relevant in terms of guard probability.
Guardonly relays have the guard flag but not the exit flag.
Since exits are less common than guards their guard probability is usually 0% even when they have the guard flag.
The number next to the contactinfo shows the number of relays running with the given ContactInfo (excluding middle-only relays).
Middle-only relays (no guard and exit flag) are excluded to reduce the size of this list.

At the end of this page you can find a comma separated list of fingerprints of all guard-only relays on this page.

## If your relay is listed here
Please configure [MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) in your torrc configuration files.
This page should help you with debugging your MyFamily configuration. The number in the last column should equal to the number of
relays you operate (for every relay).

Once MyFamily is fixed the relays will automatically disappear from this page (within ~1-2 days).
If you need help with the MyFamily configuration you can reach out to the
[tor-relays mailing list](https://lists.torproject.org/cgi-bin/mailman/listinfo/tor-relays).
You can also use tools that handle MyFamily automatically (I maintain an ansible role - 
[relayor](https://medium.com/@nusenu/deploying-tor-relays-with-ansible-6612593fa34d))
If someone else is using your contactInfo please send an email to bad-relays AT lists DOT torproject DOT org.


## ContactInfo: tor-operator@your-emailaddress-domain (2) {#tor-operatoryour-emailaddress-domain}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/64B8A00F64E16BF5C5685A76C4D9722DCBF05400) | 2018-05-01   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/9FC15C742C2E95A34F104CB5A0826C6659CFF2B7) | 2018-06-20   | No          |                     1 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://metrics.torproject.org/rs.html#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://metrics.torproject.org/rs.html#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |

## ContactInfo: zcashtorservers.org supported by a z.cash.foundati (5) {#zcashtorserversorg-supported-by-a-zcashfoundati}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [ZcashTor0se](https://metrics.torproject.org/rs.html#details/381DB186136F95370B0A7C7575E40B5DE8C18BDB) | 2017-03-14   | Yes         |                    10 |
| [ZcashTor0lv](https://metrics.torproject.org/rs.html#details/53825DFB32426F4D02E2FAA43AF713DC185299F4) | 2017-03-14   | Yes         |                    10 |
| [ZcashTor0ca](https://metrics.torproject.org/rs.html#details/800C0EBDF0C7B4A7950D445435706CD9B901C47B) | 2018-05-10   | No          |                     1 |
| [ZcashTor3nl](https://metrics.torproject.org/rs.html#details/B5A68709FF46B730CCA37D98CA477C4B9FF9296D) | 2018-01-31   | No          |                    10 |
| [ZcashTor2nl](https://metrics.torproject.org/rs.html#details/DB3B3FBD826C80E24C45043044AD33489012920F) | 2018-01-31   | No          |                    10 |


## Fingerprint List of Guard-only Relays in E2E Groups

381DB186136F95370B0A7C7575E40B5DE8C18BDB,64B8A00F64E16BF5C5685A76C4D9722DCBF05400,C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7