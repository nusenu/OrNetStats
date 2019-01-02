---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2019-01-02 19:00 UTC**

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


## ContactInfo: tor-operator@your-emailaddress-domain (8) {#tor-operatoryour-emailaddress-domain}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [myTorVer](https://metrics.torproject.org/rs.html#details/70953563B6AC3EF22E0754B7345757C6FB205989)       | 2018-10-09   | Yes         |                     1 |
| [DivisionBy1](https://metrics.torproject.org/rs.html#details/9879492B344126F899254E0F618F43D2B51F7505)    | 2018-11-08   | Yes         |                     2 |
| [anotherRelay](https://metrics.torproject.org/rs.html#details/F6691E3EB7CAB3C876AAA885E6801B63DC998C39)   | 2018-10-29   | Yes         |                     1 |
| [DimasNiceRelay](https://metrics.torproject.org/rs.html#details/BE5CE67AAC8EC61551173844D874385996F4C439) | 2018-08-15   | Yes         |                     1 |
| [Marsu](https://metrics.torproject.org/rs.html#details/8750A946DD5AB24AE71A40B1BA7672034F24663F)          | 2018-12-23   | Yes         |                     1 |
| [jgautRelay](https://metrics.torproject.org/rs.html#details/21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA)     | 2018-08-17   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/9FC15C742C2E95A34F104CB5A0826C6659CFF2B7)    | 2018-06-20   | No          |                     1 |
| [SlurmExit](https://metrics.torproject.org/rs.html#details/C0BFC0A0341BD0293F093DEC6966B99038A31B79)      | 2018-11-24   | No          |                     1 |

## ContactInfo: sysop at openinternet.io BTC: 1LZCkCZRqJ3fXnVqCBrq (2) {#sysopatopeninternetio-btc-1lzckczrqj3fxnvqcbrq}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Gihkal](https://metrics.torproject.org/rs.html#details/6E2256A26DD4A31746DF3B70F223E5A3CE03F92E)      | 2018-12-16   | Yes         |                     1 |
| [MilesPrower](https://metrics.torproject.org/rs.html#details/79E169B25E4C7CE99584F6ED06F379478F23E2B8) | 2016-01-28   | No          |                     2 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://metrics.torproject.org/rs.html#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: &lt;schneider&gt; schneiderweisse AT tutanota DOT de (3) {#schneider-schneiderweisse-at-tutanota-dot-de}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [anyname](https://metrics.torproject.org/rs.html#details/4DB8F213C3685CA4A3CF616352A8F7D39E61801A) | 2015-09-01   | Yes         |                     1 |
| [ohsally](https://metrics.torproject.org/rs.html#details/C5D55D11F26C52A6BFEE8DD23C250548AA67E9AC) | 2015-09-04   | Yes         |                     1 |
| [raybold](https://metrics.torproject.org/rs.html#details/AC80F46DAB7E902E9D6AEE056E79089577814B3D) | 2015-09-17   | No          |                     1 |

## ContactInfo: wgetdataatprotonmailch tor-relay.co (2) {#wgetdataatprotonmailch-tor-relayco}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [TorGuard](https://metrics.torproject.org/rs.html#details/8B576610170A1C716392D0D5D577D4422773FE3D) | 2018-09-07   | Yes         |                     1 |
| [Guard](https://metrics.torproject.org/rs.html#details/04A1785CDA43C3815DFEE6FF25404CD42CAD34F5)    | 2018-09-17   | No          |                     1 |

## ContactInfo: 7FE06A60 Tomas Savenas &lt;tomas AT savenas dot lt&gt; (2) {#7fe06a60-tomas-savenas-tomas-at-savenas-dot-lt}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [whitepaper](https://metrics.torproject.org/rs.html#details/778C5CA5C38E3865808AD9F86330288075276526) | 2018-12-25   | Yes         |                     1 |
| [freeSpeech](https://metrics.torproject.org/rs.html#details/4AE544F48C317D9EF4A4380754A5B1FAC10DEEF6) | 2018-12-25   | No          |                     1 |

## ContactInfo: &lt;nobody AT example dot com&gt; (2) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |

## ContactInfo: Cheena &lt;cheena @ cheena . net&gt; (3) {#cheena-cheena--cheena--net}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CheenaTorRelay1](https://metrics.torproject.org/rs.html#details/AC3DAFEDBBA5A78007A5835F4728E2408B094E49) | 2018-10-20   | Yes         |                     4 |
| [CheenaTorExit1](https://metrics.torproject.org/rs.html#details/01729F10A81DDD8A92D770B2133082EB56C75E26)  | 2018-11-26   | No          |                     4 |
| [CheenaTorExit3](https://metrics.torproject.org/rs.html#details/50825758CC2DA41DEEF6AE29CB20A803BDCC6F79)  | 2018-12-03   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

10901213FFAB09B5085131D57311563424CF2DBD,21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA,4DB8F213C3685CA4A3CF616352A8F7D39E61801A,6E2256A26DD4A31746DF3B70F223E5A3CE03F92E,70953563B6AC3EF22E0754B7345757C6FB205989,778C5CA5C38E3865808AD9F86330288075276526,8750A946DD5AB24AE71A40B1BA7672034F24663F,8B576610170A1C716392D0D5D577D4422773FE3D,9879492B344126F899254E0F618F43D2B51F7505,A9A4213EA3D707857368C683F2208C83B8755D8A,AC3DAFEDBBA5A78007A5835F4728E2408B094E49,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,BE5CE67AAC8EC61551173844D874385996F4C439,C5D55D11F26C52A6BFEE8DD23C250548AA67E9AC,F6691E3EB7CAB3C876AAA885E6801B63DC998C39