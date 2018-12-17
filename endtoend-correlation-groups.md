---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-12-17 17:00 UTC**

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
| [myTorVer](https://metrics.torproject.org/rs.html#details/70953563B6AC3EF22E0754B7345757C6FB205989)          | 2018-10-09   | Yes         |                     1 |
| [anotherRelay](https://metrics.torproject.org/rs.html#details/F6691E3EB7CAB3C876AAA885E6801B63DC998C39)      | 2018-10-29   | Yes         |                     1 |
| [DimasNiceRelay](https://metrics.torproject.org/rs.html#details/BE5CE67AAC8EC61551173844D874385996F4C439)    | 2018-08-15   | Yes         |                     1 |
| [DimasNiceRelay2nd](https://metrics.torproject.org/rs.html#details/10901213FFAB09B5085131D57311563424CF2DBD) | 2018-09-25   | Yes         |                     1 |
| [jgautRelay](https://metrics.torproject.org/rs.html#details/21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA)        | 2018-08-17   | Yes         |                     1 |
| [DivisionBy1](https://metrics.torproject.org/rs.html#details/9879492B344126F899254E0F618F43D2B51F7505)       | 2018-11-08   | Yes         |                     2 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/9FC15C742C2E95A34F104CB5A0826C6659CFF2B7)       | 2018-06-20   | No          |                     1 |
| [SlurmExit](https://metrics.torproject.org/rs.html#details/C0BFC0A0341BD0293F093DEC6966B99038A31B79)         | 2018-11-24   | No          |                     1 |

## ContactInfo: abuse@to-surf-and-protect.net (34) {#abuseto-surf-and-protectnet}

| Nickname                                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [niftysquirrel](https://metrics.torproject.org/rs.html#details/348B89013EDDD99E4755951D1EC284D9FED71226)       | 2016-09-20   | Yes         |                    32 |
| [niftyhedgehog](https://metrics.torproject.org/rs.html#details/1084200B44021D308EA4253F256794671B1D099A)       | 2016-08-23   | No          |                    32 |
| [niftywoodmouse](https://metrics.torproject.org/rs.html#details/14877C6384A9E793F422C8D1DDA447CACA4F7C4B)      | 2016-09-18   | No          |                    32 |
| [niftymouse](https://metrics.torproject.org/rs.html#details/24E91955D969AEA1D80413C64FE106FAE7FD2EA9)          | 2016-07-27   | No          |                    32 |
| [niftyrabbitrat](https://metrics.torproject.org/rs.html#details/25526E61B8BC22B662E3D4A50504021CC3D9873D)      | 2018-01-12   | No          |                    32 |
| [niftycottonmouse](https://metrics.torproject.org/rs.html#details/28F4F392F8F19E3FBDE09616D9DB8143A1E2DDD3)    | 2016-10-23   | No          |                    32 |
| [niftyeuropeanrabbit](https://metrics.torproject.org/rs.html#details/4031460683AE9E0512D3620C2758D98758AC6C93) | 2017-12-30   | No          |                    32 |
| [niftysugarglider](https://metrics.torproject.org/rs.html#details/47C42E2094EE482E7C9B586B10BABFB67557030B)    | 2016-08-30   | No          |                    32 |
| [niftyplagiodontia](https://metrics.torproject.org/rs.html#details/5D5006E4992F2F97DF4F8B926C3688870EB52BD8)   | 2016-09-22   | No          |                    32 |
| [niftychipmunk](https://metrics.torproject.org/rs.html#details/609E598FB6A00BCF7872906B602B705B64541C50)       | 2016-08-28   | No          |                    32 |
| [niftytucotuco](https://metrics.torproject.org/rs.html#details/619349D82424C601CAEB94161A4CF778993DAEE7)       | 2016-10-20   | No          |                    32 |
| [niftyhare](https://metrics.torproject.org/rs.html#details/6781471814DF164C2A6F17CD1F2584923FDE2101)           | 2018-02-03   | No          |                    32 |
| [niftyhutia](https://metrics.torproject.org/rs.html#details/6CADB707B2E0170B5F13557E42DB7E5C151CC0BC)          | 2018-09-13   | No          |                     1 |
| [niftybeaver](https://metrics.torproject.org/rs.html#details/6E94866ED8CA098BACDFD36D4E8E2B459B8A734E)         | 2016-11-23   | No          |                    32 |
| [niftycottontail](https://metrics.torproject.org/rs.html#details/71AB4726D830FAE776D74AEF790CF04D8E0151B4)     | 2016-02-05   | No          |                    32 |
| [niftyDNS2](https://metrics.torproject.org/rs.html#details/72048FB55DA1A40EA0D299769304444A64594358)           | 2018-12-16   | No          |                     1 |
| [niftyllipika](https://metrics.torproject.org/rs.html#details/7DC52AE6667A30536BA2383CD102CFC24F20AD71)        | 2016-12-02   | No          |                    32 |
| [niftyporcupine](https://metrics.torproject.org/rs.html#details/7E281CD2C315C4F7A84BC7C8721C3BC974DDBFA3)      | 2016-11-25   | No          |                    32 |
| [niftyDNS1](https://metrics.torproject.org/rs.html#details/88AE3BC088396F1D3FCC4F2F588C0DC837599D20)           | 2018-12-16   | No          |                     1 |
| [niftyjerboa](https://metrics.torproject.org/rs.html#details/8EE0534532EA31AA5172B1892F53B2F25C76EB02)         | 2016-08-30   | No          |                    32 |
| [niftyquokka](https://metrics.torproject.org/rs.html#details/906DCB390F2BA987AE258D745E60BAAABAD31DE8)         | 2016-08-03   | No          |                    32 |
| [niftypedetes](https://metrics.torproject.org/rs.html#details/92A6085EABAADD928B6F8E871540A1A41CBC08BA)        | 2016-08-24   | No          |                    32 |
| [niftynutria](https://metrics.torproject.org/rs.html#details/9A857254F379194D1CD76F4A79A20D2051BEDA3F)         | 2016-11-25   | No          |                    32 |
| [niftypygmyjerboa](https://metrics.torproject.org/rs.html#details/9B816A5B3EB20B8E4E9B9D1FBA299BD3F40F0320)    | 2017-12-27   | No          |                    32 |
| [niftybunny](https://metrics.torproject.org/rs.html#details/B740BCECC4A9569232CDD45C0E1330BA0D030D33)          | 2017-12-27   | No          |                    32 |
| [niftypika](https://metrics.torproject.org/rs.html#details/B771AA877687F88E6F1CA5354756DF6C8A7B6B24)           | 2016-01-25   | No          |                    32 |
| [niftycapybara](https://metrics.torproject.org/rs.html#details/BC82F2190DE2E97DE65F49B4A95572374BDC0789)       | 2016-08-30   | No          |                    32 |
| [niftyvolcanorabbit](https://metrics.torproject.org/rs.html#details/C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)  | 2016-02-06   | No          |                    32 |
| [niftyjackrabbit](https://metrics.torproject.org/rs.html#details/CA37CD46799449D83B6B98B8C22C649906307888)     | 2017-12-27   | No          |                    32 |
| [niftygerbil](https://metrics.torproject.org/rs.html#details/CDA2EA326E2272C57ACB26773D7252C211795B78)         | 2016-05-22   | No          |                    32 |
| [niftydormouse](https://metrics.torproject.org/rs.html#details/E6FAC9A7F33EE66F03C55C119770B2D45D3C576B)       | 2016-11-25   | No          |                    32 |
| [niftyguineapig](https://metrics.torproject.org/rs.html#details/EC1997D51892E4607C68E800549A1E7E4694005A)      | 2016-05-25   | No          |                    32 |
| [niftytreerat](https://metrics.torproject.org/rs.html#details/FAEC86A9A37152F0371D67917ABA398467DFBD9C)        | 2018-01-11   | No          |                    32 |
| [niftyrat](https://metrics.torproject.org/rs.html#details/FDA70EC93DB01E3CB418CB6943B0C68464B18B4C)            | 2016-09-17   | No          |                    32 |

## ContactInfo: &lt;nobody AT example dot com&gt; (2) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://metrics.torproject.org/rs.html#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: &lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq (31) {#zwiebeln-at-online-de-please-donate-btc-1k38x9xq}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Goethe](https://metrics.torproject.org/rs.html#details/D667A56F4E43D16524C68324B4A6444D3C9699FF)         | 2018-04-03   | Yes         |                    27 |
| [Goethe2](https://metrics.torproject.org/rs.html#details/75630B41925DB77E893FEA93A34EB5B838B2CE53)        | 2018-04-03   | Yes         |                    27 |
| [Schiller2](https://metrics.torproject.org/rs.html#details/08F1E380B2811D795A8B024E7FE21008ABFC9462)      | 2017-04-22   | No          |                    29 |
| [Gandhi2](https://metrics.torproject.org/rs.html#details/1A6F41D7B3A18134C8E3C20F56B17263AF2030F4)        | 2017-04-22   | No          |                    29 |
| [itl2](https://metrics.torproject.org/rs.html#details/1E075F7966871F8318FA2ECEF42DFEC356A53DEA)           | 2018-11-25   | No          |                     6 |
| [Nietzsche](https://metrics.torproject.org/rs.html#details/24E383836A0C6393E6F70646B6C02B46FD488A6C)      | 2018-09-17   | No          |                    27 |
| [Humboldt](https://metrics.torproject.org/rs.html#details/294CAB9AC06A4484E48E61FE1FB7EF4D7839E402)       | 2018-09-17   | No          |                    27 |
| [Hecker](https://metrics.torproject.org/rs.html#details/2EF07234ACA495086AE2476C324FB6F5F92E111A)         | 2018-09-17   | No          |                    27 |
| [Hecker2](https://metrics.torproject.org/rs.html#details/32435F652D6F06E71534BC83952EC2DC2C6450F6)        | 2018-09-17   | No          |                    27 |
| [montrealonion](https://metrics.torproject.org/rs.html#details/3246ECCAEDC4FF2949B655E0245AFFF42F8C9DFC)  | 2016-11-12   | No          |                    29 |
| [Luther](https://metrics.torproject.org/rs.html#details/5BF0617E6F94B1C993A8AC0534C4C759613A000B)         | 2018-09-17   | No          |                    27 |
| [Humboldt2](https://metrics.torproject.org/rs.html#details/6088C9AE1F712A9478FDE64CADEFF8E74ED4AE7C)      | 2018-09-17   | No          |                    27 |
| [itl4](https://metrics.torproject.org/rs.html#details/68C36BD39030350CF51366C1ED625C72FE20B43A)           | 2018-12-05   | No          |                     6 |
| [montrealonionb](https://metrics.torproject.org/rs.html#details/74FB777F25E7F80BA6BF8B808DF873A1708821A7) | 2016-12-18   | No          |                    29 |
| [quebeconion](https://metrics.torproject.org/rs.html#details/777B2DECD67C607D8857AD60E976EE3E1E8A52BF)    | 2016-11-15   | No          |                    29 |
| [i2p3](https://metrics.torproject.org/rs.html#details/92D8008026AA72131A5357005054048F879F2808)           | 2018-11-20   | No          |                    15 |
| [Nietzsche2](https://metrics.torproject.org/rs.html#details/9795AEB7A11F20333A7E41466496ACCCB0E8C232)     | 2018-09-17   | No          |                    27 |
| [Luther](https://metrics.torproject.org/rs.html#details/9B054080395062284F289061CE64DFC1F2AC9BD9)         | 2018-09-17   | No          |                    27 |
| [itl6](https://metrics.torproject.org/rs.html#details/ACA23FAA90E10A9B397D7AEB02D6148CB2B28B8E)           | 2018-12-05   | No          |                     6 |
| [itl1](https://metrics.torproject.org/rs.html#details/AD940667E1057E9690B5B2AC5C37BD017855E661)           | 2018-11-25   | No          |                     6 |
| [alsaceonionb](https://metrics.torproject.org/rs.html#details/AE271FF27CE9D274674BD8542B5F82310B02E02F)   | 2016-12-18   | No          |                    29 |
| [quebeconionb](https://metrics.torproject.org/rs.html#details/B56D5A0543C35B45D81D792A4735590E3612A815)   | 2016-12-18   | No          |                    29 |
| [Schiller](https://metrics.torproject.org/rs.html#details/C2256F7DC6130B08B94BBD6D39BAA00DB766FC40)       | 2017-04-22   | No          |                    29 |
| [itl5](https://metrics.torproject.org/rs.html#details/CC114AA5E2BCC05DE1D9ED4B817FD84F60C41A11)           | 2018-12-05   | No          |                     6 |
| [itl3](https://metrics.torproject.org/rs.html#details/CC56EF7E4A54C4B7E94E883DADF654694FBD09BA)           | 2018-11-25   | No          |                     6 |
| [heine](https://metrics.torproject.org/rs.html#details/DA0FE8B5DD9717F52376F55885BC72E619ACD97D)          | 2016-12-05   | No          |                    29 |
| [heineb](https://metrics.torproject.org/rs.html#details/E3FF9A2F09B974313AFBD7618A1451DC8610CCEC)         | 2016-12-05   | No          |                    29 |
| [Gandhi](https://metrics.torproject.org/rs.html#details/EC9D12C8F7F8721C4A9147F75E3D3F024C1B9C29)         | 2017-04-22   | No          |                    29 |
| [alsaceonion](https://metrics.torproject.org/rs.html#details/F0D44DAD8CB9A07737709F3F5AD0A93600259640)    | 2016-11-14   | No          |                    29 |
| [i2p2](https://metrics.torproject.org/rs.html#details/F944D964F00B9B121EB9544A4241D6718BA777CD)           | 2018-11-20   | No          |                    15 |
| [i2p](https://metrics.torproject.org/rs.html#details/FCDA182B78E5C37D43D5CEC49FC5F668A6610828)            | 2018-09-07   | No          |                    29 |

## ContactInfo: Cheena &lt;cheena @ cheena . net&gt; (4) {#cheena-cheena--cheena--net}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CheenaTorRelay1](https://metrics.torproject.org/rs.html#details/AC3DAFEDBBA5A78007A5835F4728E2408B094E49) | 2018-10-20   | Yes         |                     5 |
| [CheenaTorExit1](https://metrics.torproject.org/rs.html#details/01729F10A81DDD8A92D770B2133082EB56C75E26)  | 2018-11-26   | No          |                     5 |
| [CheenaTorExit4](https://metrics.torproject.org/rs.html#details/022A116E79A66F9D1081A9ED083075A8841F0CE4)  | 2018-10-26   | No          |                     5 |
| [CheenaTorExit3](https://metrics.torproject.org/rs.html#details/50825758CC2DA41DEEF6AE29CB20A803BDCC6F79)  | 2018-12-03   | No          |                     1 |

## ContactInfo: emerson tor@nodevine.net bitcoin:126gyYcBjirRmDh2G (2) {#emerson-tornodevinenet-bitcoin126gyycbjirrmdh2g}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [nodvrelay10](https://metrics.torproject.org/rs.html#details/4AA5669E80CC6265C88A4A8ECE289778286E78C5) | 2018-12-04   | Yes         |                     1 |
| [nodvexit01](https://metrics.torproject.org/rs.html#details/436B6515C78D7A4FB2104805DBB9533F77D43255)  | 2018-08-20   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

10901213FFAB09B5085131D57311563424CF2DBD,21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA,348B89013EDDD99E4755951D1EC284D9FED71226,4AA5669E80CC6265C88A4A8ECE289778286E78C5,70953563B6AC3EF22E0754B7345757C6FB205989,75630B41925DB77E893FEA93A34EB5B838B2CE53,9879492B344126F899254E0F618F43D2B51F7505,A9A4213EA3D707857368C683F2208C83B8755D8A,AC3DAFEDBBA5A78007A5835F4728E2408B094E49,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,BE5CE67AAC8EC61551173844D874385996F4C439,D667A56F4E43D16524C68324B4A6444D3C9699FF,F6691E3EB7CAB3C876AAA885E6801B63DC998C39