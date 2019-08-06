---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2019-08-06 16:00 UTC**

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


## ContactInfo: abuse@to-surf-and-protect.net (59) {#abuseto-surf-and-protectnet}

| Nickname                                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [niftylinkrat](https://metrics.torproject.org/rs.html#details/5DE37A3371AAE7638748EB43C9F1CE66E09D4470)        | 2019-01-31   | Yes         |                    58 |
| [niftydiatomys](https://metrics.torproject.org/rs.html#details/A016192D0A87FC9354A7523A211BBD9CF859708B)       | 2019-01-05   | Yes         |                    58 |
| [niftywatersgerbil](https://metrics.torproject.org/rs.html#details/E97DAC45ED2AB46DD830A279BDCC7AFCE10EE674)   | 2019-01-30   | Yes         |                    58 |
| [niftyalloeumyarion](https://metrics.torproject.org/rs.html#details/96CFE178A1D12489D9D59A0CAE17FE86F5A3A79F)  | 2019-01-05   | Yes         |                    58 |
| [niftyflorescaverat](https://metrics.torproject.org/rs.html#details/0677DF0B05ECDA2EF45F26C3332731043BB89AB8)  | 2019-01-05   | Yes         |                    58 |
| [niftycastoroides](https://metrics.torproject.org/rs.html#details/9EEDBAD7EE351996DFC91578E882BEF4FE5EDBFA)    | 2019-01-05   | Yes         |                    58 |
| [niftyleastgerbil](https://metrics.torproject.org/rs.html#details/6FBD65C22C2996B2038A090BF5E55AA7AEDEE120)    | 2019-01-30   | Yes         |                    58 |
| [niftycongogerbil](https://metrics.torproject.org/rs.html#details/85A3AC041E3FCD796AF5D653953D5E27A56E3719)    | 2019-01-31   | Yes         |                    58 |
| [niftyhornedgopher](https://metrics.torproject.org/rs.html#details/6C64AE6D7EFDA52A463FB6ADCDAE2D2DDE0677C3)   | 2019-01-05   | Yes         |                    58 |
| [niftyphoberomys](https://metrics.torproject.org/rs.html#details/87D73471FDC64BD9CEDF84435D20CA4EB5C36FE8)     | 2019-01-05   | Yes         |                    58 |
| [niftyspinymouse](https://metrics.torproject.org/rs.html#details/986E29FB17C8C7A1FEAFF203F012D5930BA079DB)     | 2019-01-31   | Yes         |                    58 |
| [niftytelicomys](https://metrics.torproject.org/rs.html#details/D27208881BBDB5EA56EFD1D1799187519591E325)      | 2019-01-05   | Yes         |                    58 |
| [niftymastomys](https://metrics.torproject.org/rs.html#details/24E1C6412183972BFD76D838AC04D1ED261743D3)       | 2019-01-31   | Yes         |                    58 |
| [niftyredrockrat](https://metrics.torproject.org/rs.html#details/9B94A776DA2C0B974BF4E06A352133EDFE62036C)     | 2019-01-31   | Yes         |                    58 |
| [niftyneochoerus](https://metrics.torproject.org/rs.html#details/2A231A5CA7AF91029B7475511D7D16DF85EC9221)     | 2019-01-05   | Yes         |                    58 |
| [niftyleithia](https://metrics.torproject.org/rs.html#details/F8E9C0C3A4B61E7599AA7A23D7ADE77E5BAB2663)        | 2019-01-05   | Yes         |                    58 |
| [wabbitseason1](https://metrics.torproject.org/rs.html#details/B4DD1F46C6E5B43D9654FF56BD32333D6586E536)       | 2019-06-24   | Yes         |                     1 |
| [wabbitseason2](https://metrics.torproject.org/rs.html#details/50B787A9FB21417BFD7B5067707DBF82D71DB11C)       | 2019-06-24   | Yes         |                     1 |
| [wabbitseason3](https://metrics.torproject.org/rs.html#details/A3901DDB7799A11E9BAB90BD1DDA734DBA196337)       | 2019-06-24   | Yes         |                     1 |
| [wabbitseason4](https://metrics.torproject.org/rs.html#details/283312BB249FCB6633A7C7E1E8241461000E6004)       | 2019-06-24   | Yes         |                     1 |
| [niftyboglemming](https://metrics.torproject.org/rs.html#details/0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)     | 2019-01-25   | No          |                    58 |
| [niftyhazelmouse](https://metrics.torproject.org/rs.html#details/0FB2EDAB99D10A2B708370E625323C76EB895FA2)     | 2019-01-31   | No          |                    58 |
| [niftyhedgehog](https://metrics.torproject.org/rs.html#details/1084200B44021D308EA4253F256794671B1D099A)       | 2016-08-23   | No          |                    58 |
| [niftywoodmouse](https://metrics.torproject.org/rs.html#details/14877C6384A9E793F422C8D1DDA447CACA4F7C4B)      | 2016-09-18   | No          |                    58 |
| [niftylagurus](https://metrics.torproject.org/rs.html#details/1D89A810BDF84522B6036034F499A766EF294DB1)        | 2019-01-26   | No          |                    58 |
| [niftymouse](https://metrics.torproject.org/rs.html#details/24E91955D969AEA1D80413C64FE106FAE7FD2EA9)          | 2016-07-27   | No          |                    58 |
| [niftyrabbitrat](https://metrics.torproject.org/rs.html#details/25526E61B8BC22B662E3D4A50504021CC3D9873D)      | 2018-01-12   | No          |                    58 |
| [niftycottonmouse](https://metrics.torproject.org/rs.html#details/28F4F392F8F19E3FBDE09616D9DB8143A1E2DDD3)    | 2016-10-23   | No          |                    58 |
| [niftysquirrel](https://metrics.torproject.org/rs.html#details/348B89013EDDD99E4755951D1EC284D9FED71226)       | 2016-09-20   | No          |                    58 |
| [niftywoodlemming](https://metrics.torproject.org/rs.html#details/3F129FB71EB2B019B47403A5552EB2D40E5369F2)    | 2019-01-25   | No          |                    58 |
| [niftyeuropeanrabbit](https://metrics.torproject.org/rs.html#details/4031460683AE9E0512D3620C2758D98758AC6C93) | 2017-12-30   | No          |                    58 |
| [niftysugarglider](https://metrics.torproject.org/rs.html#details/47C42E2094EE482E7C9B586B10BABFB67557030B)    | 2016-08-30   | No          |                    58 |
| [niftysteppemarmot](https://metrics.torproject.org/rs.html#details/48BE372CA2104D2422D49CD321060E7F697B52D9)   | 2019-01-31   | No          |                    58 |
| [niftychipmunk](https://metrics.torproject.org/rs.html#details/609E598FB6A00BCF7872906B602B705B64541C50)       | 2016-08-28   | No          |                    58 |
| [niftytucotuco](https://metrics.torproject.org/rs.html#details/619349D82424C601CAEB94161A4CF778993DAEE7)       | 2016-10-20   | No          |                    58 |
| [niftyhutia](https://metrics.torproject.org/rs.html#details/6CADB707B2E0170B5F13557E42DB7E5C151CC0BC)          | 2018-09-13   | No          |                    58 |
| [niftybeaver](https://metrics.torproject.org/rs.html#details/6E94866ED8CA098BACDFD36D4E8E2B459B8A734E)         | 2016-11-23   | No          |                    58 |
| [niftyllipika](https://metrics.torproject.org/rs.html#details/7DC52AE6667A30536BA2383CD102CFC24F20AD71)        | 2016-12-02   | No          |                    58 |
| [niftyporcupine](https://metrics.torproject.org/rs.html#details/7E281CD2C315C4F7A84BC7C8721C3BC974DDBFA3)      | 2016-11-25   | No          |                    58 |
| [niftytamiasaristus](https://metrics.torproject.org/rs.html#details/88AE3BC088396F1D3FCC4F2F588C0DC837599D20)  | 2018-12-16   | No          |                    58 |
| [niftyjerboa](https://metrics.torproject.org/rs.html#details/8EE0534532EA31AA5172B1892F53B2F25C76EB02)         | 2016-08-30   | No          |                    58 |
| [niftyquokka](https://metrics.torproject.org/rs.html#details/906DCB390F2BA987AE258D745E60BAAABAD31DE8)         | 2016-08-03   | No          |                    58 |
| [niftypedetes](https://metrics.torproject.org/rs.html#details/92A6085EABAADD928B6F8E871540A1A41CBC08BA)        | 2016-08-24   | No          |                    58 |
| [niftytamiasatsali](https://metrics.torproject.org/rs.html#details/957354D72042719C310A907FBFE42A3232C78757)   | 2019-01-26   | No          |                    58 |
| [niftyredsquirrel](https://metrics.torproject.org/rs.html#details/97D2A26EA5C9972E66D23F4698E94DBDBA8F6C18)    | 2019-01-31   | No          |                    58 |
| [niftypygmyjerboa](https://metrics.torproject.org/rs.html#details/9B816A5B3EB20B8E4E9B9D1FBA299BD3F40F0320)    | 2017-12-27   | No          |                    58 |
| [niftybunny](https://metrics.torproject.org/rs.html#details/B740BCECC4A9569232CDD45C0E1330BA0D030D33)          | 2017-12-27   | No          |                    58 |
| [niftypika](https://metrics.torproject.org/rs.html#details/B771AA877687F88E6F1CA5354756DF6C8A7B6B24)           | 2016-01-25   | No          |                    58 |
| [niftybankvole](https://metrics.torproject.org/rs.html#details/C00C28C2B1A7D8038517626CECA9BCB23B0A31D2)       | 2019-01-25   | No          |                    58 |
| [niftyvolcanorabbit](https://metrics.torproject.org/rs.html#details/C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)  | 2016-02-06   | No          |                    58 |
| [niftyjackrabbit](https://metrics.torproject.org/rs.html#details/CA37CD46799449D83B6B98B8C22C649906307888)     | 2017-12-27   | No          |                    58 |
| [niftychionomy](https://metrics.torproject.org/rs.html#details/CD97DD0842A79184A7D057ECACEF7408C239C710)       | 2019-01-25   | No          |                    58 |
| [niftygerbil](https://metrics.torproject.org/rs.html#details/CDA2EA326E2272C57ACB26773D7252C211795B78)         | 2016-05-22   | No          |                    58 |
| [niftyblythsvole](https://metrics.torproject.org/rs.html#details/E013CC98CCC1E6AFDCFC9681A53DC2DEFE5D4CCC)     | 2019-01-25   | No          |                    58 |
| [niftydormouse](https://metrics.torproject.org/rs.html#details/E6FAC9A7F33EE66F03C55C119770B2D45D3C576B)       | 2016-11-25   | No          |                    58 |
| [niftyguineapig](https://metrics.torproject.org/rs.html#details/EC1997D51892E4607C68E800549A1E7E4694005A)      | 2016-05-25   | No          |                    58 |
| [niftyjunipervole](https://metrics.torproject.org/rs.html#details/EDC4243F57F9B856B400398D5F6C354F8408EEA9)    | 2019-01-25   | No          |                    58 |
| [niftytreerat](https://metrics.torproject.org/rs.html#details/FAEC86A9A37152F0371D67917ABA398467DFBD9C)        | 2018-01-11   | No          |                    58 |
| [niftyrat](https://metrics.torproject.org/rs.html#details/FDA70EC93DB01E3CB418CB6943B0C68464B18B4C)            | 2016-09-17   | No          |                    58 |

## ContactInfo: samam &lt; at &gt; protonmail.com (2) {#samam--at--protonmailcom-}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [uzieka](https://metrics.torproject.org/rs.html#details/54DE63F4587058B79152A75A0238D7F7A0279215)    | 2016-03-28   | Yes         |                     1 |
| [herlitzka](https://metrics.torproject.org/rs.html#details/A9F5135AE18C7E25C7C79117CD8C7619BFEB85ED) | 2016-02-03   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://metrics.torproject.org/rs.html#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: Steven S &lt;katsalmovies@gmail.com&gt; (2) {#steven-s-katsalmoviesgmailcom}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [bigdaddyny](https://metrics.torproject.org/rs.html#details/0BCCF364C4EE7338B6E920E63E951922C85F91F7)  | 2019-07-15   | Yes         |                     1 |
| [bigdaddyny2](https://metrics.torproject.org/rs.html#details/25AA19700404E2B482B60B9F52AED83E3E73B5FC) | 2019-07-21   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

0677DF0B05ECDA2EF45F26C3332731043BB89AB8,0BCCF364C4EE7338B6E920E63E951922C85F91F7,24E1C6412183972BFD76D838AC04D1ED261743D3,283312BB249FCB6633A7C7E1E8241461000E6004,2A231A5CA7AF91029B7475511D7D16DF85EC9221,50B787A9FB21417BFD7B5067707DBF82D71DB11C,54DE63F4587058B79152A75A0238D7F7A0279215,5DE37A3371AAE7638748EB43C9F1CE66E09D4470,6C64AE6D7EFDA52A463FB6ADCDAE2D2DDE0677C3,6FBD65C22C2996B2038A090BF5E55AA7AEDEE120,85A3AC041E3FCD796AF5D653953D5E27A56E3719,87D73471FDC64BD9CEDF84435D20CA4EB5C36FE8,96CFE178A1D12489D9D59A0CAE17FE86F5A3A79F,986E29FB17C8C7A1FEAFF203F012D5930BA079DB,9B94A776DA2C0B974BF4E06A352133EDFE62036C,9EEDBAD7EE351996DFC91578E882BEF4FE5EDBFA,A016192D0A87FC9354A7523A211BBD9CF859708B,A3901DDB7799A11E9BAB90BD1DDA734DBA196337,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,B4DD1F46C6E5B43D9654FF56BD32333D6586E536,D27208881BBDB5EA56EFD1D1799187519591E325,E97DAC45ED2AB46DD830A279BDCC7AFCE10EE674,F8E9C0C3A4B61E7599AA7A23D7ADE77E5BAB2663