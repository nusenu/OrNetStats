---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2019-03-10 09:00 UTC**

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


## ContactInfo: tor-operator@your-emailaddress-domain (6) {#tor-operatoryour-emailaddress-domain}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [anotherRelay](https://metrics.torproject.org/rs.html#details/F6691E3EB7CAB3C876AAA885E6801B63DC998C39)   | 2018-10-29   | Yes         |                     1 |
| [DimasNiceRelay](https://metrics.torproject.org/rs.html#details/BE5CE67AAC8EC61551173844D874385996F4C439) | 2018-08-15   | Yes         |                     1 |
| [DivisionBy1](https://metrics.torproject.org/rs.html#details/9879492B344126F899254E0F618F43D2B51F7505)    | 2018-11-08   | Yes         |                     1 |
| [Marsu](https://metrics.torproject.org/rs.html#details/8750A946DD5AB24AE71A40B1BA7672034F24663F)          | 2018-12-23   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/9FC15C742C2E95A34F104CB5A0826C6659CFF2B7)    | 2018-06-20   | No          |                     1 |
| [SlurmExit](https://metrics.torproject.org/rs.html#details/C0BFC0A0341BD0293F093DEC6966B99038A31B79)      | 2018-11-24   | No          |                     1 |

## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv (6) {#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay2](https://metrics.torproject.org/rs.html#details/D5B8C38539C509380767D4DE20DE84CF84EE8299)  | 2016-09-05   | Yes         |                     7 |
| [NeelTorRelay1](https://metrics.torproject.org/rs.html#details/D31BFE2048AD5B77CA072E977B5961861A2415E6)  | 2018-01-21   | Yes         |                     5 |
| [NeelTorRelay3](https://metrics.torproject.org/rs.html#details/E6124EC00A2457F181E99117C7D67B79A2A0E61B)  | 2019-01-16   | Yes         |                     7 |
| [NeelTorFusion](https://metrics.torproject.org/rs.html#details/1CD029594B08E07F29B9420410C2E34DB71FBB28)  | 2019-03-05   | No          |                     7 |
| [NeelTorFusionB](https://metrics.torproject.org/rs.html#details/A0EB2BD840838FAD51BDAD86B0BA3908FADFAE05) | 2019-03-09   | No          |                     6 |
| [NeelTorExit1](https://metrics.torproject.org/rs.html#details/D87799B6DF17C8DD2DB1253E1D1DFB96F88675AB)   | 2019-02-20   | No          |                     7 |

## ContactInfo: Jelle Jansen &lt;tormail@gigawebs.net&gt; (4) {#jelle-jansen-tormailgigawebsnet}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [TVISION02](https://metrics.torproject.org/rs.html#details/52E018563FA31D13D6776E0897AF68AA3E21EA08) | 2019-01-09   | Yes         |                     2 |
| [TVISION04](https://metrics.torproject.org/rs.html#details/2E254E254A1FC66D6AD968E567B22F378C063026) | 2017-10-24   | Yes         |                     5 |
| [TVISION05](https://metrics.torproject.org/rs.html#details/5E1207FC5BE02728D9D0B540384EB081B53987E6) | 2018-02-11   | Yes         |                     3 |
| [TVISION01](https://metrics.torproject.org/rs.html#details/8DAF2CAF4BFB0DD56B51955A17599A9FB0E933D3) | 2017-08-06   | No          |                     3 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://metrics.torproject.org/rs.html#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |


## Fingerprint List of Guard-only Relays in E2E Groups

2E254E254A1FC66D6AD968E567B22F378C063026,52E018563FA31D13D6776E0897AF68AA3E21EA08,5E1207FC5BE02728D9D0B540384EB081B53987E6,8750A946DD5AB24AE71A40B1BA7672034F24663F,9879492B344126F899254E0F618F43D2B51F7505,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,BE5CE67AAC8EC61551173844D874385996F4C439,D31BFE2048AD5B77CA072E977B5961861A2415E6,D5B8C38539C509380767D4DE20DE84CF84EE8299,E6124EC00A2457F181E99117C7D67B79A2A0E61B,F6691E3EB7CAB3C876AAA885E6801B63DC998C39