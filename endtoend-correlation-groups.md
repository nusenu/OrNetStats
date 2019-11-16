---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2019-11-16 07:00 UTC**

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


## ContactInfo: abuse-node49 AT posteo DOT de (11) {#abuse-node49-at-posteo-dot-de}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Hydra6](https://metrics.torproject.org/rs.html#details/63DE54637F349FD686CF1C036827B5BE826B9F7C)  | 2018-12-27   | Yes         |                    11 |
| [Hydra7](https://metrics.torproject.org/rs.html#details/C013F6A7A2297FA4CD00D05EF4A1C5222B844B25)  | 2019-08-21   | Yes         |                    11 |
| [Hydra8](https://metrics.torproject.org/rs.html#details/6AEDDEC1146B00B99B87092FBAD7FB75799865C6)  | 2019-09-08   | Yes         |                    11 |
| [Hydra4](https://metrics.torproject.org/rs.html#details/B3DA9D673321B92253DCCD38A9740F2C562C91EA)  | 2019-08-20   | Yes         |                    11 |
| [Hydra5](https://metrics.torproject.org/rs.html#details/3E76E15E6BE6CFF409D44CCC40281AB5BB0B61C2)  | 2018-05-03   | Yes         |                    11 |
| [Hydra1](https://metrics.torproject.org/rs.html#details/0647C3F8352BBFA0D57A1C3E0DCF67FC3E073D2C)  | 2017-01-06   | No          |                    11 |
| [Hydra3](https://metrics.torproject.org/rs.html#details/27D02579AD5F3E32895D99C38E482D1DC6CBAE5E)  | 2019-10-17   | No          |                    11 |
| [Hydra11](https://metrics.torproject.org/rs.html#details/70A4372ED8F5DDE3BA05A17491BB6032EAC02692) | 2019-11-15   | No          |                     1 |
| [Hydra2](https://metrics.torproject.org/rs.html#details/B16D271047B18D29F62AE9F3CFC7094258506A03)  | 2017-01-08   | No          |                    11 |
| [Hydra9](https://metrics.torproject.org/rs.html#details/CB28925DA61069A43584030D2610471F1FFD4100)  | 2019-02-10   | No          |                    11 |
| [Hydra10](https://metrics.torproject.org/rs.html#details/CD21B997AF3D30AD719C066C38C7FA8C8FE83C70) | 2019-02-13   | No          |                    11 |

## ContactInfo: Kristoffer Rath Hansen &lt;kristoffer AT rathhansen d (3) {#kristoffer-rath-hansen-kristoffer-at-rathhansen-d}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [rathhansenrelay](https://metrics.torproject.org/rs.html#details/EA51EA501AB8703D4A9C1355BFDD05CFDE9A1522) | 2018-11-26   | Yes         |                     3 |
| [rathhansenexit2](https://metrics.torproject.org/rs.html#details/DF73CBB5147F7C47AAC783ABFED5C947D07FA28F) | 2019-11-07   | No          |                     2 |
| [duckduckgo](https://metrics.torproject.org/rs.html#details/EA5A01079B0207A5B7D90665C79E5322210EA091)      | 2019-11-14   | No          |                     1 |

## ContactInfo: runtime-error at riseup dot net (3) {#runtime-erroratriseupdotnet}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Daenerys](https://metrics.torproject.org/rs.html#details/E312A938D71045BE3A5C1FF3AB87CF7464194861) | 2019-07-13   | Yes         |                     1 |
| [Viserion](https://metrics.torproject.org/rs.html#details/4C5B8134341E66CB09246985E4039F9BFC0ADCE3) | 2019-07-19   | No          |                     1 |
| [Visenya](https://metrics.torproject.org/rs.html#details/A339297680115D931FA2B98C311300E8492D83AA)  | 2019-07-10   | No          |                     1 |

## ContactInfo: Steven S &lt;katsalmovies@gmail.com&gt; (3) {#steven-s-katsalmoviesgmailcom}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [bigdaddyny3](https://metrics.torproject.org/rs.html#details/AE236568ED01527850FA0D5BEFBBF6C6BDA47AF0) | 2019-07-28   | Yes         |                     1 |
| [bigdaddyny](https://metrics.torproject.org/rs.html#details/0BCCF364C4EE7338B6E920E63E951922C85F91F7)  | 2019-07-15   | Yes         |                     1 |
| [bigdaddyny4](https://metrics.torproject.org/rs.html#details/5DD2D6DCB182AC058EB9A8F71C63B0525E1C6907) | 2019-10-04   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4) | 2019-10-25   | Yes         |                     1 |
| [Mercury](https://metrics.torproject.org/rs.html#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/71840F45C2478347B872321066F9805D1A1B79FD)  | 2019-10-25   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

0BCCF364C4EE7338B6E920E63E951922C85F91F7,3E76E15E6BE6CFF409D44CCC40281AB5BB0B61C2,63DE54637F349FD686CF1C036827B5BE826B9F7C,6AEDDEC1146B00B99B87092FBAD7FB75799865C6,AE236568ED01527850FA0D5BEFBBF6C6BDA47AF0,B3DA9D673321B92253DCCD38A9740F2C562C91EA,C013F6A7A2297FA4CD00D05EF4A1C5222B844B25,DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4,E312A938D71045BE3A5C1FF3AB87CF7464194861,EA51EA501AB8703D4A9C1355BFDD05CFDE9A1522