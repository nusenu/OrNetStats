---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-05-14 22:00 UTC**

For each operator the list of running relays is shown (relays are linked to [Relay Search](https://metrics.torproject.org/rs.html)).
Operators and relays are sorted from more relevant to less relevant. More relevant in terms of guard probability.
Guardonly relays have the guard flag but not the exit flag.
Since exits are less common than guards their guard probability is usually 0% even when they have the guard flag.
The number next to the contactinfo shows the number of relays running with the given ContactInfo (excluding middle-only relays).
Middle-only relays (no guard and exit flag) are excluded to reduce the size of this list.

At the end of this page you can find a comma separated list of fingerprints of all guard-only relays on this page.

## If your relay is listed here
Please configure MyFamily in your torrc configuration files.
This page should help you with debugging your MyFamily configuration. The number in the last column should equal to the number of
relays you operate (for every relay).

Once MyFamily is fixed the relays will automatically disappear from this page (within ~1-2 days).
If you need help with the MyFamily configuration you can reach out to the
[tor-relays mailing list](https://lists.torproject.org/cgi-bin/mailman/listinfo/tor-relays).
You can also use tools that handle MyFamily automatically (I maintain an ansible role - 
[relayor](https://medium.com/@nusenu/deploying-tor-relays-with-ansible-6612593fa34d))
If someone else is using your contactInfo please send an email to ```bad-relays AT lists DOT torproject DOT org```.


## ContactInfo: see https://www.artikel5ev.de/torcontact/ (24) {#see-httpswwwartikel5evdetorcontact}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [dc6jgk13](https://metrics.torproject.org/rs.html#details/E6D4332BF40FDEE7814F2DBC926650EF8032B643)      | 2020-08-28   | Yes         |                    38 |
| [dc6jgk12c](https://metrics.torproject.org/rs.html#details/BFC6E7F298D581344DFCE95BB7EE9EDE1FC0745B)     | 2020-08-28   | Yes         |                    38 |
| [dc6jgk7c](https://metrics.torproject.org/rs.html#details/F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A)      | 2016-11-04   | Yes         |                    38 |
| [dc6jgk11c](https://metrics.torproject.org/rs.html#details/7B700C0C207EBD0002E00F499BE265519AC3C25A)     | 2016-11-11   | Yes         |                    38 |
| [artikel5ev7](https://metrics.torproject.org/rs.html#details/22404A3E87F2D7FE2FC6359FDE71B6DC2D6E730F)   | 2017-08-30   | Yes         |                    32 |
| [H3rmi](https://metrics.torproject.org/rs.html#details/A690C6AA8102C027D297AF3401BFE16918CCF7A6)         | 2016-07-22   | Yes         |                    21 |
| [artikel5ev1](https://metrics.torproject.org/rs.html#details/0BC8BA32CC3CB0F598E0C92778F7C0946DFBCE91)   | 2016-10-19   | No          |                    32 |
| [artikel5ev1b](https://metrics.torproject.org/rs.html#details/166264168E8CCCBB2444ADE0F0A22E4E6DDEF6FD)  | 2022-05-13   | No          |                    29 |
| [artikel5ev3b](https://metrics.torproject.org/rs.html#details/195712E96FD1C1B18D14D09E9E4E7A6416E23B2C)  | 2017-12-05   | No          |                    32 |
| [artikel5ev2b](https://metrics.torproject.org/rs.html#details/1AA683E036EA10AA6E078D40498CC7234F6424B9)  | 2022-05-13   | No          |                    29 |
| [artikel5ev4](https://metrics.torproject.org/rs.html#details/26C28F29B611DF4DE23ACF5D9DC1EB4895EF5E8B)   | 2019-01-25   | No          |                    32 |
| [artikel5ev10b](https://metrics.torproject.org/rs.html#details/282CAAF0E11DAD47DD73D553DC20B51099A257BB) | 2022-05-13   | No          |                    29 |
| [artikel5ev8](https://metrics.torproject.org/rs.html#details/4D0DF468DC816F8096702C2DA2C6FD67561F81C8)   | 2019-12-29   | No          |                    32 |
| [artikel5ev12](https://metrics.torproject.org/rs.html#details/780D50DCCD7F3C831E5E750F41866497C1263F76)  | 2020-09-08   | No          |                    32 |
| [artikel5ev13](https://metrics.torproject.org/rs.html#details/89C7E852CC2FA537ED78775ADC3BEA24672B4154)  | 2020-09-07   | No          |                    32 |
| [artikel5ev10](https://metrics.torproject.org/rs.html#details/AF7094B62864DE941DCD88A2F0DBAFECF3997E47)  | 2020-04-12   | No          |                    32 |
| [artikel5ev13b](https://metrics.torproject.org/rs.html#details/B1F926DA3895A89AF288623F5A4F913979299C53) | 2022-05-13   | No          |                    29 |
| [artikel5ev3c](https://metrics.torproject.org/rs.html#details/C36C76992198329C0D8F34E01D092BF2ACE0B6B0)  | 2022-05-13   | No          |                    29 |
| [artikel5ev12b](https://metrics.torproject.org/rs.html#details/CE5EF4FB644544DB2F430A60CC6EB86FD7E29BA6) | 2022-05-13   | No          |                    29 |
| [artikel5ev8b](https://metrics.torproject.org/rs.html#details/D4CA7FD04DABF6E2CB679426F5AA3205B640D147)  | 2022-05-13   | No          |                    29 |
| [artikel5ev2](https://metrics.torproject.org/rs.html#details/DC2191663DD4BAECB34F949CCAC3FDA004CE5BCE)   | 2016-10-29   | No          |                    32 |
| [artikel5ev9b](https://metrics.torproject.org/rs.html#details/E22694E83DA7BCF30DDAF5780EEF394CD0370CC4)  | 2022-05-13   | No          |                    29 |
| [artikel5ev4b](https://metrics.torproject.org/rs.html#details/F3B2CC8C2AB331150E096DD1DB8810E4A43F399D)  | 2022-05-13   | No          |                    29 |
| [artikel5ev9](https://metrics.torproject.org/rs.html#details/FC077C25B8DBB3132D397D7DF03C92BFC14C9D76)   | 2020-01-11   | No          |                    32 |

## ContactInfo: &lt;nobody AT example dot com&gt; (3) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [node01](https://metrics.torproject.org/rs.html#details/D53AE170BF6650A2C6640484FE1B5DD1C0AB895B)     | 2019-12-14   | Yes         |                     1 |
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |

## ContactInfo: g at switchblad dot es tor-relay.co (2) {#gatswitchbladdotes-tor-relayco}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [socialsbionl](https://metrics.torproject.org/rs.html#details/74C11CE0CD6BFD1AEDA1BEC526ABBE10D95EB207) | 2022-05-03   | Yes         |                     1 |
| [socialsbio](https://metrics.torproject.org/rs.html#details/00843BC25EDD6ED738DC0159A24E6452A860C74A)   | 2022-05-03   | No          |                     1 |

## ContactInfo: gusntwrk.xyz (2) {#gusntwrkxyz}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [elhombre](https://metrics.torproject.org/rs.html#details/D7910C73B9092697D7D2AF14E5CA09112F0C6EA9) | 2021-12-11   | Yes         |                     1 |
| [rknchan](https://metrics.torproject.org/rs.html#details/A5B984C20AF47731B911CDF68032A36F8678C25B)  | 2022-02-19   | No          |                     1 |

## ContactInfo: torix aT=== protonmail&lt;dOT &gt;com (11) {#torixatprotonmaildotcom}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Aramis67](https://metrics.torproject.org/rs.html#details/53C9F4954E7A7332BB0C610C5B8E04CA065AF29B) | 2019-05-13   | Yes         |                    12 |
| [Aramis65](https://metrics.torproject.org/rs.html#details/99DB99DF22EE52B9B3A32749C12EDEA78F166B3F) | 2021-12-03   | Yes         |                    12 |
| [Aramis66](https://metrics.torproject.org/rs.html#details/39A18F31B312E5CB211781090766934C1CFDAB36) | 2020-07-10   | Yes         |                     8 |
| [Aramis](https://metrics.torproject.org/rs.html#details/17F41F8DAFA4B36AAB10E202ABA14601AAE1D616)   | 2022-05-10   | No          |                     7 |
| [Aramis](https://metrics.torproject.org/rs.html#details/2B3AAC97B269D59E6D642C8BFB174EDD13741C38)   | 2021-11-12   | No          |                     8 |
| [Aramis](https://metrics.torproject.org/rs.html#details/359C5231AC2452D365B64A23C27817A1DFEE56B4)   | 2022-05-10   | No          |                     7 |
| [Aramis](https://metrics.torproject.org/rs.html#details/4F9EFCF7689084E4C8EE993E123E32B75368804C)   | 2021-08-22   | No          |                     8 |
| [Aramis](https://metrics.torproject.org/rs.html#details/9EF49A075A79F657708F5EE00B05CE7B0B79DA35)   | 2022-05-10   | No          |                     7 |
| [Aramis](https://metrics.torproject.org/rs.html#details/A549E57FC2A060FA20051537E6738B3ED5B98463)   | 2022-05-10   | No          |                     7 |
| [Aramis](https://metrics.torproject.org/rs.html#details/D3F6616034448DEEE369782C96F84FE1407E4200)   | 2021-08-22   | No          |                     8 |
| [Aramis](https://metrics.torproject.org/rs.html#details/F314580EA22CB3DCB135D64E92108BFB8FD209AF)   | 2021-11-12   | No          |                     8 |


## Fingerprint List of Guard-only Relays in E2E Groups

22404A3E87F2D7FE2FC6359FDE71B6DC2D6E730F,7B700C0C207EBD0002E00F499BE265519AC3C25A,A690C6AA8102C027D297AF3401BFE16918CCF7A6,BFC6E7F298D581344DFCE95BB7EE9EDE1FC0745B,A9A4213EA3D707857368C683F2208C83B8755D8A,74C11CE0CD6BFD1AEDA1BEC526ABBE10D95EB207,39A18F31B312E5CB211781090766934C1CFDAB36,53C9F4954E7A7332BB0C610C5B8E04CA065AF29B,99DB99DF22EE52B9B3A32749C12EDEA78F166B3F,E6D4332BF40FDEE7814F2DBC926650EF8032B643,F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A,D53AE170BF6650A2C6640484FE1B5DD1C0AB895B,D7910C73B9092697D7D2AF14E5CA09112F0C6EA9