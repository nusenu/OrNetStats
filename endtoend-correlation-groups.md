---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-08-26 06:00 UTC**

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


## ContactInfo: Jordan &lt;jordan@yui.cat&gt; (4) {#jordan-jordanyuicat}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [yuicat1](https://metrics.torproject.org/rs.html#details/431EA69FC4089BE4304AAEC38FEAE8BC8F8711C5) | 2017-12-29   | Yes         |                     4 |
| [yuicat4](https://metrics.torproject.org/rs.html#details/85D8B60E3429AD9A5A3FDAB89477C77E8F7EA2C5) | 2018-02-11   | Yes         |                     4 |
| [yuicat0](https://metrics.torproject.org/rs.html#details/BEF65D2CA651B5E484BB0E3DA31DD192935FEB1E) | 2018-06-26   | Yes         |                     1 |
| [yuicat2](https://metrics.torproject.org/rs.html#details/EF4351738CD6B454745C5432B1A15A3DEB6FE99E) | 2016-06-24   | No          |                     4 |

## ContactInfo: VSIF Support &lt;support AT vsif dot ca&gt; (7) {#vsif-support-support-at-vsif-dot-ca}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [VSIFweb](https://metrics.torproject.org/rs.html#details/78378DDD015C4E1C9242A5EC41158AF1E24CF43E)        | 2017-06-23   | Yes         |                     5 |
| [VSIFviking1](https://metrics.torproject.org/rs.html#details/1DEB985E3EEC0E7E0F6A887B417065E63522C5E2)    | 2017-06-15   | No          |                     7 |
| [VSIFenterprise](https://metrics.torproject.org/rs.html#details/59AE2B55941324B24354ADAAF971FC2C9F836963) | 2017-06-15   | No          |                     7 |
| [VSIFsalyut4](https://metrics.torproject.org/rs.html#details/D2461A903A754DEA625827AB333A2ECD06CE2E43)    | 2017-06-09   | No          |                     7 |
| [VSIFcopernicus](https://metrics.torproject.org/rs.html#details/D509A7A321FF9660665B75CB19F0FF09964C0B80) | 2018-02-11   | No          |                     6 |
| [VSIFvoyager](https://metrics.torproject.org/rs.html#details/E1DDAE70F14B9A6A7C01BDB9BDCCB70307BEE90A)    | 2018-02-11   | No          |                     6 |
| [VSIFskylab](https://metrics.torproject.org/rs.html#details/F13B97699EF7328A6289E5C2540560903CBC79A8)     | 2017-06-04   | No          |                     7 |

## ContactInfo: tor-operator@your-emailaddress-domain (3) {#tor-operatoryour-emailaddress-domain}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [DimasNiceRelay](https://metrics.torproject.org/rs.html#details/BE5CE67AAC8EC61551173844D874385996F4C439) | 2018-08-15   | Yes         |                     1 |
| [jgautRelay](https://metrics.torproject.org/rs.html#details/21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA)     | 2018-08-17   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/9FC15C742C2E95A34F104CB5A0826C6659CFF2B7)    | 2018-06-20   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA,431EA69FC4089BE4304AAEC38FEAE8BC8F8711C5,78378DDD015C4E1C9242A5EC41158AF1E24CF43E,85D8B60E3429AD9A5A3FDAB89477C77E8F7EA2C5,BE5CE67AAC8EC61551173844D874385996F4C439,BEF65D2CA651B5E484BB0E3DA31DD192935FEB1E