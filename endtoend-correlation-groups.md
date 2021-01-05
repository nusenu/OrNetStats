---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-01-05 10:00 UTC**

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


## ContactInfo: Privex Inc. https://www.privex.io (3) {#privex-inc-httpswwwprivexio}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [privexrelayde1](https://metrics.torproject.org/rs.html#details/C64EB4553AA308D8FBC314D73B44178E4CB11C35)  | 2020-11-22   | Yes         |                     2 |
| [privexrelayfin1](https://metrics.torproject.org/rs.html#details/C3ACB0492A644E27A549BC3CDF3B7A129186E3BF) | 2018-09-27   | Yes         |                     3 |
| [privexse1exit](https://metrics.torproject.org/rs.html#details/D8A1F5A8EA1AF53E3414B9C48FE6B10C31ACC9B2)   | 2019-06-26   | No          |                     2 |

## ContactInfo: shebangs@yopmail.fr (15) {#shebangsyopmailfr}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Shebangs](https://metrics.torproject.org/rs.html#details/F5F9B6B40E4D7AFCECDFB1F4503D56D522C7EFAA) | 2020-09-13   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/CEA2E066A7F8EC0F235F5190E25DD3C9F86F084B) | 2020-06-06   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/453E51CBAA4C2169EBCB05583247DD6201E87FAD) | 2020-06-05   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/A4A79E2B8294AA2572B46C5C772E149F84FAF763) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/AC990FD1FF5058EFA43A809E948B23EF998D021B) | 2020-06-05   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/3688001D75469101F74A5D551A49B0EF410F0E26) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/F3A3461889BF97250F50A7BAAAE4A2B92062F6D7) | 2020-07-03   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/E4A8BC82E660528D5B0B8D36C08AB44B77351736) | 2020-12-17   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/BA8546AE9B27F0C81F98A6C12D96B7DAB0814991) | 2020-06-06   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/328ED3A92D1CD621659B4DA6E210FCAED813174B) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/072E4EC47D640118D5438BFFDFF1AF7BB4E2AD2B) | 2020-10-05   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/0794E378A1EE9337D917BEE88607A1C12AC7F906) | 2020-10-03   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/C8B5B2186A2DED8F419EAA933EFB5FFE2D412CF4) | 2020-09-25   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/E9272A28DAFABAE4F3D07233A16D13BDD5F58D4A) | 2020-12-25   | No          |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/5A8918BCA6B05FC780CFBDD66703BEF60DE53DA6) | 2020-12-25   | No          |                     1 |

## ContactInfo: contact at torbox dot org bc1qswtwvvjscschje9gql6a (4) {#contactattorboxdotorg-bc1qswtwvvjscschje9gql6a}

| Nickname                                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [TorboxProjectRelay](https://metrics.torproject.org/rs.html#details/AD5FE3E205AE09162D466C80E27BCB208305A5FD) | 2020-12-20   | Yes         |                     1 |
| [TorboxProjectExit3](https://metrics.torproject.org/rs.html#details/440510C88DF8F959F0018CA23131254BD18BCAFB) | 2020-12-20   | No          |                     1 |
| [TorboxProjectExit2](https://metrics.torproject.org/rs.html#details/35A659EBE04BE828054262426D4A9FD0494E0A9F) | 2020-12-20   | No          |                     1 |
| [TorboxProjectExit](https://metrics.torproject.org/rs.html#details/43323C80668E28E81E61845A5CA98A52AE97A4C5)  | 2020-12-20   | No          |                     1 |

## ContactInfo: https://www.torservers.net/donate.html &lt;support .A (17) {#httpswwwtorserversnetdonatehtml-support-a}

| Nickname                                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [HaveHeart](https://metrics.torproject.org/rs.html#details/204DFD2A2C6A0DC1FA0EACB495218E0B661704FD)        | 2017-10-03   | No          |                    17 |
| [CriticalMass](https://metrics.torproject.org/rs.html#details/77131D7E2EC1CA9B8D737502256DA9103599CE51)     | 2017-10-03   | No          |                    17 |
| [sofia](https://metrics.torproject.org/rs.html#details/7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)            | 2017-10-03   | No          |                    17 |
| [dorrisdeebrown](https://metrics.torproject.org/rs.html#details/FDAED15C98CFE7A416E5676F614254F78406105C)   | 2016-12-23   | No          |                    17 |
| [criticalmass](https://metrics.torproject.org/rs.html#details/1D3174338A1131A53E098443E76E1103CDED00DC)     | 2016-12-30   | No          |                    17 |
| [amazonas](https://metrics.torproject.org/rs.html#details/5974B3F4C66D83BBC9622E0F0F023FE48428DB9B)         | 2017-11-01   | No          |                    17 |
| [weizenbaum2](https://metrics.torproject.org/rs.html#details/8A2D71CBCA33F13A3EA9614DE28AE3F669D84987)      | 2019-01-12   | No          |                    17 |
| [amartysen](https://metrics.torproject.org/rs.html#details/8EF8766E1645A41A2AE1565EB673A4957C8D5AD2)        | 2017-11-01   | No          |                    17 |
| [politkovskaja](https://metrics.torproject.org/rs.html#details/0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88)    | 2018-02-19   | No          |                    17 |
| [freeKleptikov](https://metrics.torproject.org/rs.html#details/F4594608272C82407E9D137F1AE89A408CCFD285)    | 2017-11-01   | No          |                    17 |
| [weizenbaum3](https://metrics.torproject.org/rs.html#details/D729C688382CC2A576089716BE10490D2D66FCE4)      | 2019-02-06   | No          |                     1 |
| [iVPN](https://metrics.torproject.org/rs.html#details/A2534EF23390CAE079B1586F0FDF9CE11F556062)             | 2016-12-30   | No          |                    17 |
| [weizenbaum](https://metrics.torproject.org/rs.html#details/0E5522CB4F79E36C0BB263BABC861CFC686929AE)       | 2019-01-12   | No          |                    17 |
| [renewablefreedom](https://metrics.torproject.org/rs.html#details/CA94704217260E7483DA88719CACD7A94C564D5C) | 2018-05-22   | No          |                    17 |
| [HSLtor](https://metrics.torproject.org/rs.html#details/E43A346CB81DDF364B6FF68235AFADBA0E8692B8)           | 2017-01-22   | No          |                    17 |
| [AnosognosiaRedux](https://metrics.torproject.org/rs.html#details/D6D6B6614C9EF2DAD13AC0C94487AD8ED3B6877F) | 2018-06-15   | No          |                    17 |
| [hackeriet1](https://metrics.torproject.org/rs.html#details/E379A6CACEFAFE1B8EA68503BFCFF1215BF1EE7F)       | 2015-12-02   | No          |                     1 |

## ContactInfo: Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w (20) {#nicholas-merrill-nick-at-calyx-dot-com-btc---14w}

| Nickname                                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CalyxInstitute07](https://metrics.torproject.org/rs.html#details/1B9FACF25E17D26E307EA7CFA7D455B144B032E5) | 2013-11-05   | Yes         |                    20 |
| [CalyxInstitute06](https://metrics.torproject.org/rs.html#details/6F4E9FD00D4251D98BE96FB1AA546FE34676A95B) | 2013-11-23   | No          |                    20 |
| [CalyxInstitute10](https://metrics.torproject.org/rs.html#details/42ED91DD3768F6A2A194D094A7432CBE8DA004B1) | 2016-04-01   | No          |                    20 |
| [CalyxInstitute11](https://metrics.torproject.org/rs.html#details/6C143720FFF8469EF6A5C5B4066366340CF6C0D1) | 2014-11-24   | No          |                    20 |
| [CalyxInstitute09](https://metrics.torproject.org/rs.html#details/7761DDC7EB1BE26D4155F74A15F12C32A36FE0F2) | 2013-11-19   | No          |                    20 |
| [CalyxInstitute08](https://metrics.torproject.org/rs.html#details/0B5E5E70FFEA9C7F9FFD13B8E16916A608F3E9EB) | 2013-11-12   | No          |                    20 |
| [CalyxInstitute03](https://metrics.torproject.org/rs.html#details/84D361B736A8CD1E8818D0FC186892E91AB76881) | 2013-06-23   | No          |                    20 |
| [CalyxInstitute14](https://metrics.torproject.org/rs.html#details/0011BD2485AD45D984EC4159C88FC066E5E3300E) | 2014-12-23   | No          |                    20 |
| [CalyxInstitute13](https://metrics.torproject.org/rs.html#details/A7C7EB2A0DFB2E3FFFC12B7756707433DD550F9E) | 2014-12-20   | No          |                    20 |
| [CalyxInstitute22](https://metrics.torproject.org/rs.html#details/4B218691AF8BC02BAB4D856689652E958AF5DCF3) | 2020-12-03   | No          |                     1 |
| [CalyxInstitute20](https://metrics.torproject.org/rs.html#details/673C081A9502D5D3AB9395FF4257274BE4C7A8A4) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute15](https://metrics.torproject.org/rs.html#details/47E49319DD67784F1E65B5793371BE467365979E) | 2015-08-21   | No          |                    20 |
| [CalyxInstitute21](https://metrics.torproject.org/rs.html#details/70ACA07D9276277B82E909C1439E19CCA2FB16CC) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute12](https://metrics.torproject.org/rs.html#details/B34CC9056250847D1980F08285B01CF0B718C0B6) | 2014-12-16   | No          |                    20 |
| [CalyxInstitute04](https://metrics.torproject.org/rs.html#details/501B3DBF250B094A05CA5DBC424AD4C3D46721A2) | 2013-07-08   | No          |                    20 |
| [CalyxInstitute17](https://metrics.torproject.org/rs.html#details/81EDFBC8F6F5C7CF0ADD5F8E08BC8FABA04089C6) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute16](https://metrics.torproject.org/rs.html#details/F68A76522D356F89BEC286889A3822250567BE2E) | 2020-01-28   | No          |                    20 |
| [CalyxInstitute01](https://metrics.torproject.org/rs.html#details/E4D1F25DFBE484208866BA4A1A958B73127CB0AD) | 2013-06-11   | No          |                    20 |
| [CalyxInstitute19](https://metrics.torproject.org/rs.html#details/E8663924FE2AAD4E081A17ED6976D0AE8010F47B) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute18](https://metrics.torproject.org/rs.html#details/EDEDB8797873D340328B5FEDBD7744A7D1DF151F) | 2020-01-30   | No          |                    20 |

## ContactInfo: abuse-node49 AT posteo DOT de (33) {#abuse-node49-at-posteo-dot-de}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Hydra7a](https://metrics.torproject.org/rs.html#details/C013F6A7A2297FA4CD00D05EF4A1C5222B844B25)  | 2019-08-21   | No          |                    33 |
| [Hydra6a](https://metrics.torproject.org/rs.html#details/63DE54637F349FD686CF1C036827B5BE826B9F7C)  | 2018-12-27   | No          |                     3 |
| [Hydra4a](https://metrics.torproject.org/rs.html#details/B3DA9D673321B92253DCCD38A9740F2C562C91EA)  | 2019-08-20   | No          |                     3 |
| [Hydra6](https://metrics.torproject.org/rs.html#details/1050FC79C5F1103B185300EF72DDF5B4EDC683C9)   | 2020-12-05   | No          |                    30 |
| [Hydra23](https://metrics.torproject.org/rs.html#details/F7ED4158B7114617E8F737C65DBE87EE6B83445B)  | 2020-11-11   | No          |                    30 |
| [Hydra14a](https://metrics.torproject.org/rs.html#details/01B70C7C497FC8667DB5EB82C40D8F9214D6A484) | 2019-12-29   | No          |                    33 |
| [Hydra22](https://metrics.torproject.org/rs.html#details/BD33EF180B1118B00BDF073E2771210E3BDDD8CD)  | 2020-11-11   | No          |                    30 |
| [Hydra13a](https://metrics.torproject.org/rs.html#details/8CDF2F3A8ABD834CF9F3E8FC202DF64625BFB443) | 2020-02-10   | No          |                     3 |
| [Hydra24](https://metrics.torproject.org/rs.html#details/8F293A6484A0973167B15C4997AB9F24C21143FE)  | 2020-11-11   | No          |                    30 |
| [Hydra4](https://metrics.torproject.org/rs.html#details/6C0E4E223B1C7E4366FFABA33BF033636A867865)   | 2020-12-05   | No          |                    30 |
| [Hydra28](https://metrics.torproject.org/rs.html#details/427956E3F23EEBA31954CB0942AEA0ECD43A004A)  | 2020-11-20   | No          |                    33 |
| [Hydra30](https://metrics.torproject.org/rs.html#details/22C1314867920DA37001DAD1A63F1D5CABF9DB11)  | 2020-12-02   | No          |                    30 |
| [Hydra15](https://metrics.torproject.org/rs.html#details/4BA3C12B073B7E3F7977C46AF3638685BB89493F)  | 2020-12-02   | No          |                    33 |
| [Hydra27](https://metrics.torproject.org/rs.html#details/A0A91967046F7A9BC3154C7B3C3FDE34C02B1017)  | 2020-11-20   | No          |                    33 |
| [Hydra1](https://metrics.torproject.org/rs.html#details/0647C3F8352BBFA0D57A1C3E0DCF67FC3E073D2C)   | 2017-01-06   | No          |                    33 |
| [Hydra25](https://metrics.torproject.org/rs.html#details/6CB18098F50819DEAB22E369EC3A5661A552A66C)  | 2020-11-20   | No          |                    33 |
| [Hydra26](https://metrics.torproject.org/rs.html#details/1940398159C3C571939363DDE8044F3DB8B97394)  | 2020-11-20   | No          |                    33 |
| [Hydra29](https://metrics.torproject.org/rs.html#details/2DEF8010770472367EB2089CA0A50A17B211E78A)  | 2020-12-02   | No          |                    30 |
| [Hydra13](https://metrics.torproject.org/rs.html#details/39C37AFC908D12BB79B34EB6298929BC51C2E651)  | 2020-12-03   | No          |                    30 |
| [Hydra18](https://metrics.torproject.org/rs.html#details/3AD29FE1241B73595F99BA2C6D830AF0B6874043)  | 2020-06-30   | No          |                    30 |
| [Hydra16](https://metrics.torproject.org/rs.html#details/1DFE397493D0791DE63F2D6EA5AB6EBCB7B9871A)  | 2020-06-09   | No          |                    30 |
| [Hydra17](https://metrics.torproject.org/rs.html#details/E3DAF067B028450B31CF5CE118F2F9AC53146ABD)  | 2020-06-09   | No          |                    30 |
| [Hydra19](https://metrics.torproject.org/rs.html#details/E465AD166798A3CD0A4866FA2A8BB5ADD157FBD5)  | 2020-06-30   | No          |                    30 |
| [Hydra20](https://metrics.torproject.org/rs.html#details/86E479266EBB982E204009532ED460628689E5B5)  | 2020-10-07   | No          |                    30 |
| [Hydra10](https://metrics.torproject.org/rs.html#details/4F68F1B23FCED9D17852FFFDE21637C284BCF107)  | 2020-12-05   | No          |                    30 |
| [Hydra9](https://metrics.torproject.org/rs.html#details/CB28925DA61069A43584030D2610471F1FFD4100)   | 2019-02-10   | No          |                    30 |
| [Hydra3](https://metrics.torproject.org/rs.html#details/27D02579AD5F3E32895D99C38E482D1DC6CBAE5E)   | 2019-10-17   | No          |                    30 |
| [Hydra21](https://metrics.torproject.org/rs.html#details/5B7C577DDEBC6B2C39B55364F4EAD69FE8181067)  | 2020-10-05   | No          |                    30 |
| [Hydra35](https://metrics.torproject.org/rs.html#details/7466057426018C41EDFC1465BE7F01E27155CFBF)  | 2021-01-02   | No          |                     2 |
| [Hydra34](https://metrics.torproject.org/rs.html#details/7B972FDF84026AC52E41461F05DDBBE3A07598AF)  | 2021-01-02   | No          |                     2 |
| [Hydra32](https://metrics.torproject.org/rs.html#details/8D1117EFBC91270AE1FCE55E21F9D250985AFAB3)  | 2020-12-29   | No          |                     9 |
| [Hydra31](https://metrics.torproject.org/rs.html#details/AF3511FA8B418C756BDBA97A6EDE970D1F74F27E)  | 2020-12-29   | No          |                     9 |
| [Hydra33](https://metrics.torproject.org/rs.html#details/C673AFE5CF9CC49E5F864F0F80D5FE2814A52233)  | 2020-12-29   | No          |                     9 |


## Fingerprint List of Guard-only Relays in E2E Groups

C3ACB0492A644E27A549BC3CDF3B7A129186E3BF,C64EB4553AA308D8FBC314D73B44178E4CB11C35,072E4EC47D640118D5438BFFDFF1AF7BB4E2AD2B,0794E378A1EE9337D917BEE88607A1C12AC7F906,328ED3A92D1CD621659B4DA6E210FCAED813174B,3688001D75469101F74A5D551A49B0EF410F0E26,453E51CBAA4C2169EBCB05583247DD6201E87FAD,A4A79E2B8294AA2572B46C5C772E149F84FAF763,AC990FD1FF5058EFA43A809E948B23EF998D021B,BA8546AE9B27F0C81F98A6C12D96B7DAB0814991,C8B5B2186A2DED8F419EAA933EFB5FFE2D412CF4,CEA2E066A7F8EC0F235F5190E25DD3C9F86F084B,E4A8BC82E660528D5B0B8D36C08AB44B77351736,F3A3461889BF97250F50A7BAAAE4A2B92062F6D7,F5F9B6B40E4D7AFCECDFB1F4503D56D522C7EFAA,AD5FE3E205AE09162D466C80E27BCB208305A5FD,1B9FACF25E17D26E307EA7CFA7D455B144B032E5