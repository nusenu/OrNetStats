---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-05-02 14:00 UTC**

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


## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://metrics.torproject.org/rs.html#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: VSIF Support &lt;support AT vsif dot ca&gt; (7) {#vsif-support-support-at-vsif-dot-ca}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [VSIFweb](https://metrics.torproject.org/rs.html#details/78378DDD015C4E1C9242A5EC41158AF1E24CF43E)        | 2017-06-23   | Yes         |                     4 |
| [VSIFviking1](https://metrics.torproject.org/rs.html#details/1DEB985E3EEC0E7E0F6A887B417065E63522C5E2)    | 2017-06-15   | No          |                     7 |
| [VSIFenterprise](https://metrics.torproject.org/rs.html#details/59AE2B55941324B24354ADAAF971FC2C9F836963) | 2017-06-15   | No          |                     7 |
| [VSIFsalyut4](https://metrics.torproject.org/rs.html#details/D2461A903A754DEA625827AB333A2ECD06CE2E43)    | 2017-06-09   | No          |                     7 |
| [VSIFcopernicus](https://metrics.torproject.org/rs.html#details/D509A7A321FF9660665B75CB19F0FF09964C0B80) | 2018-02-11   | No          |                     6 |
| [VSIFvoyager](https://metrics.torproject.org/rs.html#details/E1DDAE70F14B9A6A7C01BDB9BDCCB70307BEE90A)    | 2018-02-11   | No          |                     6 |
| [VSIFskylab](https://metrics.torproject.org/rs.html#details/F13B97699EF7328A6289E5C2540560903CBC79A8)     | 2017-06-04   | No          |                     6 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://metrics.torproject.org/rs.html#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://metrics.torproject.org/rs.html#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

78378DDD015C4E1C9242A5EC41158AF1E24CF43E,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7