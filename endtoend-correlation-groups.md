---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-12-10 19:00 UTC**

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
| [DivisionBy1](https://metrics.torproject.org/rs.html#details/9879492B344126F899254E0F618F43D2B51F7505)       | 2018-11-08   | Yes         |                     2 |
| [jgautRelay](https://metrics.torproject.org/rs.html#details/21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA)        | 2018-08-17   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/9FC15C742C2E95A34F104CB5A0826C6659CFF2B7)       | 2018-06-20   | No          |                     1 |
| [SlurmExit](https://metrics.torproject.org/rs.html#details/C0BFC0A0341BD0293F093DEC6966B99038A31B79)         | 2018-11-24   | No          |                     1 |

## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv (7) {#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay2](https://metrics.torproject.org/rs.html#details/D5B8C38539C509380767D4DE20DE84CF84EE8299) | 2016-09-05   | Yes         |                     6 |
| [NeelTorRelay1](https://metrics.torproject.org/rs.html#details/D31BFE2048AD5B77CA072E977B5961861A2415E6) | 2018-01-21   | Yes         |                     6 |
| [NeelTorExit3](https://metrics.torproject.org/rs.html#details/18E3A51E779560063D22E5069349E137BF1422B2)  | 2018-02-13   | No          |                     6 |
| [NeelTorExit4](https://metrics.torproject.org/rs.html#details/59FE609666A0EAC5A1BF80E482647F1FEE05C465)  | 2018-03-14   | No          |                     6 |
| [NeelTorExit5](https://metrics.torproject.org/rs.html#details/81103399BE96904954227E84362D14AD8FC94D4F)  | 2018-12-10   | No          |                     1 |
| [NeelTorExit2](https://metrics.torproject.org/rs.html#details/8A3B2D50590CAB574108507FC5D36C9BA079D9AF)  | 2018-10-31   | No          |                     6 |
| [NeelTorExit1](https://metrics.torproject.org/rs.html#details/C8B03E4DC7FF4398110DE8A8E93566CAAFE9BB43)  | 2018-04-16   | No          |                     6 |

## ContactInfo: &lt;nobody AT example dot com&gt; (2) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |

## ContactInfo: c dot gloeckner at tuta dot io tor-relay.co (2) {#cdotgloecknerattutadotio-tor-relayco}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Schlangenbiss](https://metrics.torproject.org/rs.html#details/04DA2A0E8564A8E98BC2848C8629CC7F4BC8BBA6) | 2018-11-25   | Yes         |                     1 |
| [Netzfreiheit](https://metrics.torproject.org/rs.html#details/888FEC76A96C05D185B1C2174B95DAB4E7274A6C)  | 2018-12-06   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://metrics.torproject.org/rs.html#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: &lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq (32) {#zwiebeln-at-online-de-please-donate-btc-1k38x9xq}

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
| [mandela2](https://metrics.torproject.org/rs.html#details/36F5D375ED389FC346C3AB01DE179864EE334596)       | 2018-08-12   | No          |                    27 |
| [Luther](https://metrics.torproject.org/rs.html#details/5BF0617E6F94B1C993A8AC0534C4C759613A000B)         | 2018-09-17   | No          |                    27 |
| [Humboldt2](https://metrics.torproject.org/rs.html#details/6088C9AE1F712A9478FDE64CADEFF8E74ED4AE7C)      | 2018-09-17   | No          |                    27 |
| [itl4](https://metrics.torproject.org/rs.html#details/68C36BD39030350CF51366C1ED625C72FE20B43A)           | 2018-12-05   | No          |                     6 |
| [montrealonionb](https://metrics.torproject.org/rs.html#details/74FB777F25E7F80BA6BF8B808DF873A1708821A7) | 2016-12-18   | No          |                    29 |
| [quebeconion](https://metrics.torproject.org/rs.html#details/777B2DECD67C607D8857AD60E976EE3E1E8A52BF)    | 2016-11-15   | No          |                    29 |
| [i2p3](https://metrics.torproject.org/rs.html#details/92D8008026AA72131A5357005054048F879F2808)           | 2018-11-20   | No          |                    15 |
| [Nietzsche2](https://metrics.torproject.org/rs.html#details/9795AEB7A11F20333A7E41466496ACCCB0E8C232)     | 2018-09-17   | No          |                    27 |
| [Luther](https://metrics.torproject.org/rs.html#details/9B054080395062284F289061CE64DFC1F2AC9BD9)         | 2018-09-17   | No          |                    27 |
| [Mandela](https://metrics.torproject.org/rs.html#details/A6D6F20891BDD1367DEB56C024DB4E6D7FADBE09)        | 2018-08-12   | No          |                    27 |
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
| [i2p](https://metrics.torproject.org/rs.html#details/FCDA182B78E5C37D43D5CEC49FC5F668A6610828)            | 2018-09-07   | No          |                    29 |

## ContactInfo: tech@emeraldonion.org (4) {#techemeraldonionorg}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [emeraldMini](https://metrics.torproject.org/rs.html#details/78E39D497195209FA45A3320E67F0E114ECC9398)  | 2018-11-19   | Yes         |                     1 |
| [EmeraldOnion](https://metrics.torproject.org/rs.html#details/AAB8C81C9443B917A49BEF56C9B38F4CD34D4A45) | 2018-11-13   | No          |                     3 |
| [nitrohorse](https://metrics.torproject.org/rs.html#details/B4944F8E31472498E86F89A028F5B84BEEC0B73A)   | 2018-07-13   | No          |                     3 |
| [shelob](https://metrics.torproject.org/rs.html#details/C42E78EC7BEB5CA0FABD4A6BBDDD67EDD61DFF8D)       | 2018-05-24   | No          |                     3 |


## Fingerprint List of Guard-only Relays in E2E Groups

04DA2A0E8564A8E98BC2848C8629CC7F4BC8BBA6,10901213FFAB09B5085131D57311563424CF2DBD,21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA,70953563B6AC3EF22E0754B7345757C6FB205989,75630B41925DB77E893FEA93A34EB5B838B2CE53,78E39D497195209FA45A3320E67F0E114ECC9398,9879492B344126F899254E0F618F43D2B51F7505,A9A4213EA3D707857368C683F2208C83B8755D8A,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,BE5CE67AAC8EC61551173844D874385996F4C439,D31BFE2048AD5B77CA072E977B5961861A2415E6,D5B8C38539C509380767D4DE20DE84CF84EE8299,D667A56F4E43D16524C68324B4A6444D3C9699FF,F6691E3EB7CAB3C876AAA885E6801B63DC998C39