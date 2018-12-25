---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-12-25 08:00 UTC**

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

| Nickname                                                                                                     | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [anotherRelay](https://metrics.torproject.org/rs.html#details/F6691E3EB7CAB3C876AAA885E6801B63DC998C39)      | 2018-10-29   | Yes         |                     1 |
| [myTorVer](https://metrics.torproject.org/rs.html#details/70953563B6AC3EF22E0754B7345757C6FB205989)          | 2018-10-09   | Yes         |                     1 |
| [DimasNiceRelay2nd](https://metrics.torproject.org/rs.html#details/10901213FFAB09B5085131D57311563424CF2DBD) | 2018-09-25   | Yes         |                     1 |
| [DimasNiceRelay](https://metrics.torproject.org/rs.html#details/BE5CE67AAC8EC61551173844D874385996F4C439)    | 2018-08-15   | Yes         |                     1 |
| [DivisionBy1](https://metrics.torproject.org/rs.html#details/9879492B344126F899254E0F618F43D2B51F7505)       | 2018-11-08   | Yes         |                     2 |
| [jgautRelay](https://metrics.torproject.org/rs.html#details/21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA)        | 2018-08-17   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/9FC15C742C2E95A34F104CB5A0826C6659CFF2B7)       | 2018-06-20   | No          |                     1 |
| [SlurmExit](https://metrics.torproject.org/rs.html#details/C0BFC0A0341BD0293F093DEC6966B99038A31B79)         | 2018-11-24   | No          |                     1 |

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

## ContactInfo: &lt;nobody AT example dot com&gt; (2) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |

## ContactInfo: &lt;schneider&gt; schneiderweisse AT tutanota DOT de (3) {#schneider-schneiderweisse-at-tutanota-dot-de}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [anyname](https://metrics.torproject.org/rs.html#details/4DB8F213C3685CA4A3CF616352A8F7D39E61801A) | 2015-09-01   | Yes         |                     1 |
| [ohsally](https://metrics.torproject.org/rs.html#details/C5D55D11F26C52A6BFEE8DD23C250548AA67E9AC) | 2015-09-04   | Yes         |                     1 |
| [raybold](https://metrics.torproject.org/rs.html#details/AC80F46DAB7E902E9D6AEE056E79089577814B3D) | 2015-09-17   | No          |                     1 |

## ContactInfo: &lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq (31) {#zwiebeln-at-online-de-please-donate-btc-1k38x9xq}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Goethe](https://metrics.torproject.org/rs.html#details/D667A56F4E43D16524C68324B4A6444D3C9699FF)         | 2018-04-03   | Yes         |                    25 |
| [Goethe2](https://metrics.torproject.org/rs.html#details/75630B41925DB77E893FEA93A34EB5B838B2CE53)        | 2018-04-03   | Yes         |                    25 |
| [Schiller2](https://metrics.torproject.org/rs.html#details/08F1E380B2811D795A8B024E7FE21008ABFC9462)      | 2017-04-22   | No          |                    27 |
| [Gandhi2](https://metrics.torproject.org/rs.html#details/1A6F41D7B3A18134C8E3C20F56B17263AF2030F4)        | 2017-04-22   | No          |                    27 |
| [itl2](https://metrics.torproject.org/rs.html#details/1E075F7966871F8318FA2ECEF42DFEC356A53DEA)           | 2018-11-25   | No          |                     6 |
| [Nietzsche](https://metrics.torproject.org/rs.html#details/24E383836A0C6393E6F70646B6C02B46FD488A6C)      | 2018-09-17   | No          |                    25 |
| [Humboldt](https://metrics.torproject.org/rs.html#details/294CAB9AC06A4484E48E61FE1FB7EF4D7839E402)       | 2018-09-17   | No          |                    25 |
| [Hecker](https://metrics.torproject.org/rs.html#details/2EF07234ACA495086AE2476C324FB6F5F92E111A)         | 2018-09-17   | No          |                    25 |
| [Hecker2](https://metrics.torproject.org/rs.html#details/32435F652D6F06E71534BC83952EC2DC2C6450F6)        | 2018-09-17   | No          |                    25 |
| [montrealonion](https://metrics.torproject.org/rs.html#details/3246ECCAEDC4FF2949B655E0245AFFF42F8C9DFC)  | 2016-11-12   | No          |                    27 |
| [Luther](https://metrics.torproject.org/rs.html#details/5BF0617E6F94B1C993A8AC0534C4C759613A000B)         | 2018-09-17   | No          |                    25 |
| [Humboldt2](https://metrics.torproject.org/rs.html#details/6088C9AE1F712A9478FDE64CADEFF8E74ED4AE7C)      | 2018-09-17   | No          |                    25 |
| [itl4](https://metrics.torproject.org/rs.html#details/68C36BD39030350CF51366C1ED625C72FE20B43A)           | 2018-12-05   | No          |                     6 |
| [montrealonionb](https://metrics.torproject.org/rs.html#details/74FB777F25E7F80BA6BF8B808DF873A1708821A7) | 2016-12-18   | No          |                    27 |
| [quebeconion](https://metrics.torproject.org/rs.html#details/777B2DECD67C607D8857AD60E976EE3E1E8A52BF)    | 2016-11-15   | No          |                    27 |
| [i2p3](https://metrics.torproject.org/rs.html#details/92D8008026AA72131A5357005054048F879F2808)           | 2018-11-20   | No          |                    15 |
| [Nietzsche2](https://metrics.torproject.org/rs.html#details/9795AEB7A11F20333A7E41466496ACCCB0E8C232)     | 2018-09-17   | No          |                    25 |
| [Luther](https://metrics.torproject.org/rs.html#details/9B054080395062284F289061CE64DFC1F2AC9BD9)         | 2018-09-17   | No          |                    25 |
| [itl6](https://metrics.torproject.org/rs.html#details/ACA23FAA90E10A9B397D7AEB02D6148CB2B28B8E)           | 2018-12-05   | No          |                     6 |
| [itl1](https://metrics.torproject.org/rs.html#details/AD940667E1057E9690B5B2AC5C37BD017855E661)           | 2018-11-25   | No          |                     6 |
| [alsaceonionb](https://metrics.torproject.org/rs.html#details/AE271FF27CE9D274674BD8542B5F82310B02E02F)   | 2016-12-18   | No          |                    27 |
| [quebeconionb](https://metrics.torproject.org/rs.html#details/B56D5A0543C35B45D81D792A4735590E3612A815)   | 2016-12-18   | No          |                    27 |
| [Schiller](https://metrics.torproject.org/rs.html#details/C2256F7DC6130B08B94BBD6D39BAA00DB766FC40)       | 2017-04-22   | No          |                    27 |
| [itl5](https://metrics.torproject.org/rs.html#details/CC114AA5E2BCC05DE1D9ED4B817FD84F60C41A11)           | 2018-12-05   | No          |                     6 |
| [itl3](https://metrics.torproject.org/rs.html#details/CC56EF7E4A54C4B7E94E883DADF654694FBD09BA)           | 2018-11-25   | No          |                     6 |
| [heine](https://metrics.torproject.org/rs.html#details/DA0FE8B5DD9717F52376F55885BC72E619ACD97D)          | 2016-12-05   | No          |                    27 |
| [heineb](https://metrics.torproject.org/rs.html#details/E3FF9A2F09B974313AFBD7618A1451DC8610CCEC)         | 2016-12-05   | No          |                    27 |
| [Gandhi](https://metrics.torproject.org/rs.html#details/EC9D12C8F7F8721C4A9147F75E3D3F024C1B9C29)         | 2017-04-22   | No          |                    27 |
| [alsaceonion](https://metrics.torproject.org/rs.html#details/F0D44DAD8CB9A07737709F3F5AD0A93600259640)    | 2016-11-14   | No          |                    27 |
| [i2p2](https://metrics.torproject.org/rs.html#details/F944D964F00B9B121EB9544A4241D6718BA777CD)           | 2018-11-20   | No          |                    15 |
| [i2p](https://metrics.torproject.org/rs.html#details/FCDA182B78E5C37D43D5CEC49FC5F668A6610828)            | 2018-09-07   | No          |                    27 |

## ContactInfo: Cheena &lt;cheena @ cheena . net&gt; (3) {#cheena-cheena--cheena--net}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CheenaTorRelay1](https://metrics.torproject.org/rs.html#details/AC3DAFEDBBA5A78007A5835F4728E2408B094E49) | 2018-10-20   | Yes         |                     5 |
| [CheenaTorExit1](https://metrics.torproject.org/rs.html#details/01729F10A81DDD8A92D770B2133082EB56C75E26)  | 2018-11-26   | No          |                     5 |
| [CheenaTorExit3](https://metrics.torproject.org/rs.html#details/50825758CC2DA41DEEF6AE29CB20A803BDCC6F79)  | 2018-12-03   | No          |                     1 |

## ContactInfo: emerson tor@nodevine.net bitcoin:126gyYcBjirRmDh2G (2) {#emerson-tornodevinenet-bitcoin126gyycbjirrmdh2g}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [nodvrelay10](https://metrics.torproject.org/rs.html#details/4AA5669E80CC6265C88A4A8ECE289778286E78C5) | 2018-12-04   | Yes         |                     1 |
| [nodvexit01](https://metrics.torproject.org/rs.html#details/436B6515C78D7A4FB2104805DBB9533F77D43255)  | 2018-08-20   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

10901213FFAB09B5085131D57311563424CF2DBD,21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA,4AA5669E80CC6265C88A4A8ECE289778286E78C5,4DB8F213C3685CA4A3CF616352A8F7D39E61801A,6E2256A26DD4A31746DF3B70F223E5A3CE03F92E,70953563B6AC3EF22E0754B7345757C6FB205989,75630B41925DB77E893FEA93A34EB5B838B2CE53,9879492B344126F899254E0F618F43D2B51F7505,A9A4213EA3D707857368C683F2208C83B8755D8A,AC3DAFEDBBA5A78007A5835F4728E2408B094E49,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,BE5CE67AAC8EC61551173844D874385996F4C439,C5D55D11F26C52A6BFEE8DD23C250548AA67E9AC,D667A56F4E43D16524C68324B4A6444D3C9699FF,F6691E3EB7CAB3C876AAA885E6801B63DC998C39