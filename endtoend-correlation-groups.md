---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-12-11 20:00 UTC**

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
If someone else is using your contactInfo please send an email to ```bad-relays AT lists DOT torproject DOT org```.


## ContactInfo: abuse-node49 AT posteo DOT de (30) {#abuse-node49-at-posteo-dot-de}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Hydra7](https://metrics.torproject.org/rs.html#details/C013F6A7A2297FA4CD00D05EF4A1C5222B844B25)  | 2019-08-21   | Yes         |                    30 |
| [Hydra6](https://metrics.torproject.org/rs.html#details/63DE54637F349FD686CF1C036827B5BE826B9F7C)  | 2018-12-27   | Yes         |                     7 |
| [Hydra14](https://metrics.torproject.org/rs.html#details/01B70C7C497FC8667DB5EB82C40D8F9214D6A484) | 2019-12-29   | Yes         |                    30 |
| [Hydra4](https://metrics.torproject.org/rs.html#details/B3DA9D673321B92253DCCD38A9740F2C562C91EA)  | 2019-08-20   | Yes         |                     7 |
| [Hydra13](https://metrics.torproject.org/rs.html#details/8CDF2F3A8ABD834CF9F3E8FC202DF64625BFB443) | 2020-02-10   | Yes         |                     7 |
| [Hydra5](https://metrics.torproject.org/rs.html#details/034AA4B30F77DF0FE183602EA7F8251FF2CF1BA2)  | 2019-11-23   | No          |                    30 |
| [Hydra2](https://metrics.torproject.org/rs.html#details/0443D98C0C44D3E0E6238790345DB5624DB41B28)  | 2019-12-05   | No          |                    30 |
| [Hydra1](https://metrics.torproject.org/rs.html#details/0647C3F8352BBFA0D57A1C3E0DCF67FC3E073D2C)  | 2017-01-06   | No          |                    30 |
| [Hydra6](https://metrics.torproject.org/rs.html#details/1050FC79C5F1103B185300EF72DDF5B4EDC683C9)  | 2020-12-05   | No          |                    27 |
| [Hydra12](https://metrics.torproject.org/rs.html#details/180A5BCC01866E09E4D229B6C084CD1E3C75636F) | 2019-12-15   | No          |                    30 |
| [Hydra26](https://metrics.torproject.org/rs.html#details/1940398159C3C571939363DDE8044F3DB8B97394) | 2020-11-20   | No          |                    30 |
| [Hydra16](https://metrics.torproject.org/rs.html#details/1DFE397493D0791DE63F2D6EA5AB6EBCB7B9871A) | 2020-06-09   | No          |                    30 |
| [Hydra30](https://metrics.torproject.org/rs.html#details/22C1314867920DA37001DAD1A63F1D5CABF9DB11) | 2020-12-02   | No          |                    27 |
| [Hydra3](https://metrics.torproject.org/rs.html#details/27D02579AD5F3E32895D99C38E482D1DC6CBAE5E)  | 2019-10-17   | No          |                    30 |
| [Hydra29](https://metrics.torproject.org/rs.html#details/2DEF8010770472367EB2089CA0A50A17B211E78A) | 2020-12-02   | No          |                    27 |
| [Hydra13](https://metrics.torproject.org/rs.html#details/39C37AFC908D12BB79B34EB6298929BC51C2E651) | 2020-12-03   | No          |                    27 |
| [Hydra18](https://metrics.torproject.org/rs.html#details/3AD29FE1241B73595F99BA2C6D830AF0B6874043) | 2020-06-30   | No          |                    30 |
| [Hydra28](https://metrics.torproject.org/rs.html#details/427956E3F23EEBA31954CB0942AEA0ECD43A004A) | 2020-11-20   | No          |                    30 |
| [Hydra15](https://metrics.torproject.org/rs.html#details/4BA3C12B073B7E3F7977C46AF3638685BB89493F) | 2020-12-02   | No          |                    27 |
| [Hydra10](https://metrics.torproject.org/rs.html#details/4F68F1B23FCED9D17852FFFDE21637C284BCF107) | 2020-12-05   | No          |                    27 |
| [Hydra4](https://metrics.torproject.org/rs.html#details/6C0E4E223B1C7E4366FFABA33BF033636A867865)  | 2020-12-05   | No          |                    27 |
| [Hydra25](https://metrics.torproject.org/rs.html#details/6CB18098F50819DEAB22E369EC3A5661A552A66C) | 2020-11-20   | No          |                    30 |
| [Hydra11](https://metrics.torproject.org/rs.html#details/70A4372ED8F5DDE3BA05A17491BB6032EAC02692) | 2019-11-15   | No          |                    30 |
| [Hydra8](https://metrics.torproject.org/rs.html#details/7716DE8030A56A80080446E0CBC59738605454E6)  | 2019-11-23   | No          |                    30 |
| [Hydra24](https://metrics.torproject.org/rs.html#details/8F293A6484A0973167B15C4997AB9F24C21143FE) | 2020-11-11   | No          |                    30 |
| [Hydra27](https://metrics.torproject.org/rs.html#details/A0A91967046F7A9BC3154C7B3C3FDE34C02B1017) | 2020-11-20   | No          |                    30 |
| [Hydra22](https://metrics.torproject.org/rs.html#details/BD33EF180B1118B00BDF073E2771210E3BDDD8CD) | 2020-11-11   | No          |                    30 |
| [Hydra9](https://metrics.torproject.org/rs.html#details/CB28925DA61069A43584030D2610471F1FFD4100)  | 2019-02-10   | No          |                    30 |
| [Hydra17](https://metrics.torproject.org/rs.html#details/E3DAF067B028450B31CF5CE118F2F9AC53146ABD) | 2020-06-09   | No          |                    30 |
| [Hydra23](https://metrics.torproject.org/rs.html#details/F7ED4158B7114617E8F737C65DBE87EE6B83445B) | 2020-11-11   | No          |                    30 |

## ContactInfo: Privex Inc. https://www.privex.io (3) {#privex-inc-httpswwwprivexio}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [privexrelayde1](https://metrics.torproject.org/rs.html#details/C64EB4553AA308D8FBC314D73B44178E4CB11C35)  | 2020-11-22   | Yes         |                     2 |
| [privexrelayfin1](https://metrics.torproject.org/rs.html#details/C3ACB0492A644E27A549BC3CDF3B7A129186E3BF) | 2018-09-27   | Yes         |                     3 |
| [privexse1exit](https://metrics.torproject.org/rs.html#details/D8A1F5A8EA1AF53E3414B9C48FE6B10C31ACC9B2)   | 2019-06-26   | No          |                     2 |

## ContactInfo: abuse at yggdrasil dot ws (6) {#abuseatyggdrasildotws}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [BKA](https://metrics.torproject.org/rs.html#details/DA580E4EB2A453298D40F73ECFC78E896B001182)      | 2020-10-07   | Yes         |                     6 |
| [Loki](https://metrics.torproject.org/rs.html#details/0ADAC68F29875A1366F06762F2B305B0BFD11364)     | 2020-12-02   | No          |                     1 |
| [Ymir](https://metrics.torproject.org/rs.html#details/4AA0035604DF40E5BA20DBE88EF6D11432421BFA)     | 2020-10-27   | No          |                     6 |
| [Ganymed](https://metrics.torproject.org/rs.html#details/5AFF7583F5ED62A274823C83199F2E19083692EC)  | 2020-08-20   | No          |                     7 |
| [Freya](https://metrics.torproject.org/rs.html#details/85ED839A03D10C46219609625D7FEAE59EDCCFDD)    | 2020-05-27   | No          |                     6 |
| [Kallisto](https://metrics.torproject.org/rs.html#details/D4C5BAEA92CADCC02D64E0DD9F1A49024C57F05C) | 2020-09-11   | No          |                     6 |

## ContactInfo: Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w (20) {#nicholas-merrill-nick-at-calyx-dot-com-btc---14w}

| Nickname                                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CalyxInstitute07](https://metrics.torproject.org/rs.html#details/1B9FACF25E17D26E307EA7CFA7D455B144B032E5) | 2013-11-05   | Yes         |                    20 |
| [CalyxInstitute14](https://metrics.torproject.org/rs.html#details/0011BD2485AD45D984EC4159C88FC066E5E3300E) | 2014-12-23   | No          |                    20 |
| [CalyxInstitute08](https://metrics.torproject.org/rs.html#details/0B5E5E70FFEA9C7F9FFD13B8E16916A608F3E9EB) | 2013-11-12   | No          |                    20 |
| [CalyxInstitute10](https://metrics.torproject.org/rs.html#details/42ED91DD3768F6A2A194D094A7432CBE8DA004B1) | 2016-04-01   | No          |                    20 |
| [CalyxInstitute15](https://metrics.torproject.org/rs.html#details/47E49319DD67784F1E65B5793371BE467365979E) | 2015-08-21   | No          |                    20 |
| [CalyxInstitute22](https://metrics.torproject.org/rs.html#details/4B218691AF8BC02BAB4D856689652E958AF5DCF3) | 2020-12-03   | No          |                     1 |
| [CalyxInstitute04](https://metrics.torproject.org/rs.html#details/501B3DBF250B094A05CA5DBC424AD4C3D46721A2) | 2013-07-08   | No          |                    20 |
| [CalyxInstitute20](https://metrics.torproject.org/rs.html#details/673C081A9502D5D3AB9395FF4257274BE4C7A8A4) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute11](https://metrics.torproject.org/rs.html#details/6C143720FFF8469EF6A5C5B4066366340CF6C0D1) | 2014-11-24   | No          |                    20 |
| [CalyxInstitute06](https://metrics.torproject.org/rs.html#details/6F4E9FD00D4251D98BE96FB1AA546FE34676A95B) | 2013-11-23   | No          |                    20 |
| [CalyxInstitute21](https://metrics.torproject.org/rs.html#details/70ACA07D9276277B82E909C1439E19CCA2FB16CC) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute09](https://metrics.torproject.org/rs.html#details/7761DDC7EB1BE26D4155F74A15F12C32A36FE0F2) | 2013-11-19   | No          |                    20 |
| [CalyxInstitute17](https://metrics.torproject.org/rs.html#details/81EDFBC8F6F5C7CF0ADD5F8E08BC8FABA04089C6) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute03](https://metrics.torproject.org/rs.html#details/84D361B736A8CD1E8818D0FC186892E91AB76881) | 2013-06-23   | No          |                    20 |
| [CalyxInstitute13](https://metrics.torproject.org/rs.html#details/A7C7EB2A0DFB2E3FFFC12B7756707433DD550F9E) | 2014-12-20   | No          |                    20 |
| [CalyxInstitute12](https://metrics.torproject.org/rs.html#details/B34CC9056250847D1980F08285B01CF0B718C0B6) | 2014-12-16   | No          |                    20 |
| [CalyxInstitute01](https://metrics.torproject.org/rs.html#details/E4D1F25DFBE484208866BA4A1A958B73127CB0AD) | 2013-06-11   | No          |                    20 |
| [CalyxInstitute19](https://metrics.torproject.org/rs.html#details/E8663924FE2AAD4E081A17ED6976D0AE8010F47B) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute18](https://metrics.torproject.org/rs.html#details/EDEDB8797873D340328B5FEDBD7744A7D1DF151F) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute16](https://metrics.torproject.org/rs.html#details/F68A76522D356F89BEC286889A3822250567BE2E) | 2020-01-28   | No          |                    20 |

## ContactInfo: tor at a9 dot wtf (2) {#torata9dotwtf}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [a9TorRelay04](https://metrics.torproject.org/rs.html#details/BD0DBFEE1A5CBF890A68741339A6DE247896D276) | 2020-11-11   | Yes         |                     2 |
| [a9TorExit](https://metrics.torproject.org/rs.html#details/2DB8A946826D0CB4F5C3A8264628DD0F16F6612D)    | 2020-09-12   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

01B70C7C497FC8667DB5EB82C40D8F9214D6A484,63DE54637F349FD686CF1C036827B5BE826B9F7C,8CDF2F3A8ABD834CF9F3E8FC202DF64625BFB443,B3DA9D673321B92253DCCD38A9740F2C562C91EA,C013F6A7A2297FA4CD00D05EF4A1C5222B844B25,C3ACB0492A644E27A549BC3CDF3B7A129186E3BF,C64EB4553AA308D8FBC314D73B44178E4CB11C35,DA580E4EB2A453298D40F73ECFC78E896B001182,1B9FACF25E17D26E307EA7CFA7D455B144B032E5,BD0DBFEE1A5CBF890A68741339A6DE247896D276