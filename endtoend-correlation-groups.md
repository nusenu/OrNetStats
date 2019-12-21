---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2019-12-21 06:00 UTC**

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


## ContactInfo: abuse-node49 AT posteo DOT de (13) {#abuse-node49-at-posteo-dot-de}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Hydra7](https://metrics.torproject.org/rs.html#details/C013F6A7A2297FA4CD00D05EF4A1C5222B844B25)  | 2019-08-21   | Yes         |                    14 |
| [Hydra4](https://metrics.torproject.org/rs.html#details/B3DA9D673321B92253DCCD38A9740F2C562C91EA)  | 2019-08-20   | Yes         |                    14 |
| [Hydra6](https://metrics.torproject.org/rs.html#details/63DE54637F349FD686CF1C036827B5BE826B9F7C)  | 2018-12-27   | Yes         |                    14 |
| [Hydra2](https://metrics.torproject.org/rs.html#details/B16D271047B18D29F62AE9F3CFC7094258506A03)  | 2017-01-08   | Yes         |                     2 |
| [Hydra5](https://metrics.torproject.org/rs.html#details/034AA4B30F77DF0FE183602EA7F8251FF2CF1BA2)  | 2019-11-23   | No          |                    14 |
| [Hydra2](https://metrics.torproject.org/rs.html#details/0443D98C0C44D3E0E6238790345DB5624DB41B28)  | 2019-12-05   | No          |                    13 |
| [Hydra1](https://metrics.torproject.org/rs.html#details/0647C3F8352BBFA0D57A1C3E0DCF67FC3E073D2C)  | 2017-01-06   | No          |                    14 |
| [Hydra12](https://metrics.torproject.org/rs.html#details/180A5BCC01866E09E4D229B6C084CD1E3C75636F) | 2019-12-15   | No          |                    14 |
| [Hydra3](https://metrics.torproject.org/rs.html#details/27D02579AD5F3E32895D99C38E482D1DC6CBAE5E)  | 2019-10-17   | No          |                    14 |
| [Hydra11](https://metrics.torproject.org/rs.html#details/70A4372ED8F5DDE3BA05A17491BB6032EAC02692) | 2019-11-15   | No          |                    14 |
| [Hydra8](https://metrics.torproject.org/rs.html#details/7716DE8030A56A80080446E0CBC59738605454E6)  | 2019-11-23   | No          |                    14 |
| [Hydra9](https://metrics.torproject.org/rs.html#details/CB28925DA61069A43584030D2610471F1FFD4100)  | 2019-02-10   | No          |                    14 |
| [Hydra10](https://metrics.torproject.org/rs.html#details/CD21B997AF3D30AD719C066C38C7FA8C8FE83C70) | 2019-02-13   | No          |                    14 |

## ContactInfo: bobs.house AT mail.ru 36j52chsdz962ivcpN1xfPXkJz (7) {#bobshouse-at-mailru-36j52chsdz962ivcpn1xfpxkjz}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [BobsHouseLU02](https://metrics.torproject.org/rs.html#details/5832668C21FF375C6B77A9BEB01E2BFDC7CD9C43) | 2019-09-29   | Yes         |                     1 |
| [BobsHouseLU03](https://metrics.torproject.org/rs.html#details/C0FB7C7ED8478AE78846B5C5585DD62E162222E1) | 2019-09-29   | Yes         |                     1 |
| [BobsHouseLU05](https://metrics.torproject.org/rs.html#details/65F56DD25EB283238BF6A10C10A8C50D7D83B931) | 2019-09-29   | Yes         |                     1 |
| [BobsHouseLU01](https://metrics.torproject.org/rs.html#details/52952860B81079DE731062216F0443DB89C14790) | 2019-09-29   | Yes         |                     1 |
| [BobsHouseRO06](https://metrics.torproject.org/rs.html#details/1F226CD8277DA2C28D15364E88D596F9FCCED98B) | 2019-11-13   | No          |                     1 |
| [BobsHouseRO05](https://metrics.torproject.org/rs.html#details/8574D4F76F44EBD2A274DA94732BD5791C08675B) | 2019-07-24   | No          |                     1 |
| [BobsHouseRO04](https://metrics.torproject.org/rs.html#details/B1BF289B965760D17B3508E3E48FF5DC8154FB70) | 2019-07-24   | No          |                     1 |

## ContactInfo: runtime-error at riseup dot net (3) {#runtime-erroratriseupdotnet}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Daenerys](https://metrics.torproject.org/rs.html#details/E312A938D71045BE3A5C1FF3AB87CF7464194861) | 2019-07-13   | Yes         |                     1 |
| [Viserion](https://metrics.torproject.org/rs.html#details/4C5B8134341E66CB09246985E4039F9BFC0ADCE3) | 2019-07-19   | No          |                     1 |
| [Visenya](https://metrics.torproject.org/rs.html#details/A339297680115D931FA2B98C311300E8492D83AA)  | 2019-07-10   | No          |                     1 |

## ContactInfo: Steven S &lt;katsalmovies@gmail.com&gt; (3) {#steven-s-katsalmoviesgmailcom}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [bigdaddyny](https://metrics.torproject.org/rs.html#details/0BCCF364C4EE7338B6E920E63E951922C85F91F7)  | 2019-07-15   | Yes         |                     1 |
| [bigdaddyny3](https://metrics.torproject.org/rs.html#details/AE236568ED01527850FA0D5BEFBBF6C6BDA47AF0) | 2019-07-28   | Yes         |                     1 |
| [bigdaddyny4](https://metrics.torproject.org/rs.html#details/5DD2D6DCB182AC058EB9A8F71C63B0525E1C6907) | 2019-10-04   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (2) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4) | 2019-10-25   | Yes         |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/71840F45C2478347B872321066F9805D1A1B79FD)  | 2019-10-25   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

0BCCF364C4EE7338B6E920E63E951922C85F91F7,52952860B81079DE731062216F0443DB89C14790,5832668C21FF375C6B77A9BEB01E2BFDC7CD9C43,63DE54637F349FD686CF1C036827B5BE826B9F7C,65F56DD25EB283238BF6A10C10A8C50D7D83B931,AE236568ED01527850FA0D5BEFBBF6C6BDA47AF0,B16D271047B18D29F62AE9F3CFC7094258506A03,B3DA9D673321B92253DCCD38A9740F2C562C91EA,C013F6A7A2297FA4CD00D05EF4A1C5222B844B25,C0FB7C7ED8478AE78846B5C5585DD62E162222E1,DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4,E312A938D71045BE3A5C1FF3AB87CF7464194861