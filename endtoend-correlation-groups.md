---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-01-15 19:00 UTC**

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


## ContactInfo: see https://www.artikel5ev.de/torcontact/ (14) {#see-httpswwwartikel5evdetorcontact}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [dc6jgk7b](https://metrics.torproject.org/rs.html#details/F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A)       | 2016-11-04   | Yes         |                    18 |
| [dc6jgk9barm64](https://metrics.torproject.org/rs.html#details/78BC2254D3B31CD865F7682633AA438212132532)  | 2016-11-11   | Yes         |                    18 |
| [dc6jgk6](https://metrics.torproject.org/rs.html#details/A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13)        | 2016-10-06   | Yes         |                    18 |
| [dc6jgk11barm64](https://metrics.torproject.org/rs.html#details/7B700C0C207EBD0002E00F499BE265519AC3C25A) | 2016-11-11   | Yes         |                    18 |
| [dc6jgk1](https://metrics.torproject.org/rs.html#details/486740353B905AA4731F82C0B4CC25821A62C6E3)        | 2014-06-09   | Yes         |                    18 |
| [dc6jgk5b](https://metrics.torproject.org/rs.html#details/846B3EAAF0C07FF72FC79AEBB11FA3ADC58F240F)       | 2016-09-05   | Yes         |                    18 |
| [artikel5ev7](https://metrics.torproject.org/rs.html#details/22404A3E87F2D7FE2FC6359FDE71B6DC2D6E730F)    | 2017-08-30   | Yes         |                    17 |
| [artikel5ev1](https://metrics.torproject.org/rs.html#details/0BC8BA32CC3CB0F598E0C92778F7C0946DFBCE91)    | 2016-10-19   | No          |                    17 |
| [artikel5ev3b](https://metrics.torproject.org/rs.html#details/195712E96FD1C1B18D14D09E9E4E7A6416E23B2C)   | 2017-12-05   | No          |                    17 |
| [artikel5ev4](https://metrics.torproject.org/rs.html#details/26C28F29B611DF4DE23ACF5D9DC1EB4895EF5E8B)    | 2019-01-25   | No          |                    17 |
| [artikel5ev8](https://metrics.torproject.org/rs.html#details/4D0DF468DC816F8096702C2DA2C6FD67561F81C8)    | 2019-12-29   | No          |                    18 |
| [Artikel5ev6](https://metrics.torproject.org/rs.html#details/4DD902046E7155BBE79C34EE6D53BF7408B98CE4)    | 2017-03-05   | No          |                    18 |
| [artikel5ev2](https://metrics.torproject.org/rs.html#details/DC2191663DD4BAECB34F949CCAC3FDA004CE5BCE)    | 2016-10-29   | No          |                    17 |
| [artikel5ev9](https://metrics.torproject.org/rs.html#details/FC077C25B8DBB3132D397D7DF03C92BFC14C9D76)    | 2020-01-11   | No          |                    12 |

## ContactInfo: &lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq (23) {#zwiebeln-at-online-de-please-donate-btc-1k38x9xq}

| Nickname                                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [LuXun](https://metrics.torproject.org/rs.html#details/693A982584CF4DD7BF2158B640CCF9A75A87B1BD)               | 2019-12-12   | Yes         |                     1 |
| [GaoZhisheng](https://metrics.torproject.org/rs.html#details/23B3EF4271E38A744E23ACC4345E56CBDB42A1A5)         | 2019-12-12   | Yes         |                     1 |
| [LiuXiaobo](https://metrics.torproject.org/rs.html#details/1617A702B30320C37A5C9FA3CFB737A2AFA9198D)           | 2019-11-26   | No          |                    17 |
| [TahirElci](https://metrics.torproject.org/rs.html#details/3246ECCAEDC4FF2949B655E0245AFFF42F8C9DFC)           | 2016-11-12   | No          |                    17 |
| [Hecker](https://metrics.torproject.org/rs.html#details/348439F4A3D959E6D1481070DA81A135343419CB)              | 2019-12-01   | No          |                    17 |
| [LechWalesa](https://metrics.torproject.org/rs.html#details/364E18848469385C5948376FAF778AC61D4CFB67)          | 2019-11-29   | No          |                    17 |
| [RosaLuxemburg](https://metrics.torproject.org/rs.html#details/42EB556E25A3C33A238AB68AFD043273D0FC6B41)       | 2019-12-01   | No          |                     1 |
| [weirenminfuwu](https://metrics.torproject.org/rs.html#details/53FF1EDC8528AF4238FB7501831E6BACFF4B42D2)       | 2019-11-26   | No          |                    17 |
| [SimonBolivar](https://metrics.torproject.org/rs.html#details/69ECFB731C2B0AA7B4D8746EF3504ADCB1F0A556)        | 2019-11-29   | No          |                    17 |
| [SebnemKorurFincanci](https://metrics.torproject.org/rs.html#details/74FB777F25E7F80BA6BF8B808DF873A1708821A7) | 2016-12-18   | No          |                    17 |
| [Politkowskaja](https://metrics.torproject.org/rs.html#details/777B2DECD67C607D8857AD60E976EE3E1E8A52BF)       | 2016-11-15   | No          |                    17 |
| [MartinLutherKing](https://metrics.torproject.org/rs.html#details/78DF2B937849E6B7636E901377DB08A15B51525C)    | 2020-01-10   | No          |                     1 |
| [Freiheit](https://metrics.torproject.org/rs.html#details/8B496F3EF3BF5CC32A4C20ECDBEC2A06E7EA4357)            | 2020-01-06   | No          |                     1 |
| [JanKuciak](https://metrics.torproject.org/rs.html#details/9C1559C46AD0279EEF6FD187E1B27D939C303086)           | 2020-01-06   | No          |                     1 |
| [ShirinEbadi](https://metrics.torproject.org/rs.html#details/A926970FE1AEF9C6D8D4BF57ED6B88F3F8C66415)         | 2019-11-28   | No          |                    17 |
| [DaphneCaruana](https://metrics.torproject.org/rs.html#details/B22169DDB936E4CF4B8C81E9514BD05658466974)       | 2019-11-28   | No          |                    17 |
| [BadshahKhan](https://metrics.torproject.org/rs.html#details/B56D5A0543C35B45D81D792A4735590E3612A815)         | 2016-12-18   | No          |                    17 |
| [RudiDutschke](https://metrics.torproject.org/rs.html#details/B8D596040EDFF67D7A200FB289DC1620275EAF52)        | 2019-12-01   | No          |                     1 |
| [Marx](https://metrics.torproject.org/rs.html#details/BCB6AC303A69A7E87BB2D6F3F13A0C0F0A6C938E)                | 2019-11-26   | No          |                    17 |
| [Brecht](https://metrics.torproject.org/rs.html#details/E00C087ECFB27D7BF969936F1FDD9354E03CAE2F)              | 2020-01-10   | No          |                     1 |
| [Sacharow](https://metrics.torproject.org/rs.html#details/E79A58AF0DB93B90F97B48963CC4729E4CFA43C5)            | 2019-11-26   | No          |                    17 |
| [Mandela](https://metrics.torproject.org/rs.html#details/F1F9D1DBD7E56F99C61C3712D5F4A02153FD9AD4)             | 2019-11-26   | No          |                    17 |
| [Gandhi](https://metrics.torproject.org/rs.html#details/F2AF93D23D91F9CFE03C5151DF01B0481BF99E12)              | 2019-11-28   | No          |                    17 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (2) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4) | 2019-10-25   | Yes         |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/71840F45C2478347B872321066F9805D1A1B79FD)  | 2019-10-25   | No          |                     1 |

## ContactInfo: report at dustin dot in tor-relay.co (2) {#reportatdustindotin-tor-relayco}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [RAWRELAY](https://metrics.torproject.org/rs.html#details/CCD3CE265252F0BC284358754769E2EDC7D19593) | 2019-12-01   | Yes         |                     1 |
| [RAWREXIT](https://metrics.torproject.org/rs.html#details/E571246BDD42BCFB0EF8F8AAE759DEEE64BA94DB) | 2019-12-01   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

22404A3E87F2D7FE2FC6359FDE71B6DC2D6E730F,23B3EF4271E38A744E23ACC4345E56CBDB42A1A5,486740353B905AA4731F82C0B4CC25821A62C6E3,693A982584CF4DD7BF2158B640CCF9A75A87B1BD,78BC2254D3B31CD865F7682633AA438212132532,7B700C0C207EBD0002E00F499BE265519AC3C25A,846B3EAAF0C07FF72FC79AEBB11FA3ADC58F240F,A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13,CCD3CE265252F0BC284358754769E2EDC7D19593,DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4,F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A