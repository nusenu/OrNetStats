---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-07-16 16:00 UTC**

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


## ContactInfo: abuse@torrelays.ru (35) {#abusetorrelaysru}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Reshiram](https://metrics.torproject.org/rs.html#details/07007CB632002FC92FB11DE78C72C44B5160A1A3)     | 2021-04-28   | Yes         |                    38 |
| [Eristof](https://metrics.torproject.org/rs.html#details/DC4349041B89D9FDD4DC53BD680B42B37A9CB195)      | 2021-05-03   | Yes         |                    38 |
| [Geodude](https://metrics.torproject.org/rs.html#details/51BD782616C3EBA543B0D4EE34D7C1CE1ED2291D)      | 2021-03-20   | Yes         |                    38 |
| [Reshiram](https://metrics.torproject.org/rs.html#details/9F1687D0D79A74F2C6F9FB918089405565BA5329)     | 2021-04-28   | Yes         |                    38 |
| [Tepig](https://metrics.torproject.org/rs.html#details/751EDB5D969C72479270D223823A8ED4E578C070)        | 2021-03-19   | Yes         |                    38 |
| [SunnyShiner](https://metrics.torproject.org/rs.html#details/1A647701D0368E8F073FF38773986F43A24C60CA)  | 2021-05-13   | Yes         |                    38 |
| [Chespin](https://metrics.torproject.org/rs.html#details/DC862F7BBF619EA3FA4FB667A4D8118652922FC8)      | 2021-03-19   | Yes         |                    38 |
| [MoonLoon](https://metrics.torproject.org/rs.html#details/261A7D651D319021D7141B7CE3ECA6E9DA983540)     | 2021-03-02   | Yes         |                    38 |
| [Bulbasaur](https://metrics.torproject.org/rs.html#details/E789DDCFDF2F92F3A6548796A22D5C8E64EE1A1B)    | 2021-03-08   | Yes         |                    38 |
| [Oshawott](https://metrics.torproject.org/rs.html#details/55ED11C6B5A35D40CD07F5A8DC12B82F0B7AADDF)     | 2021-03-18   | Yes         |                    38 |
| [Moonshine](https://metrics.torproject.org/rs.html#details/3326C64CD86258ACA4657E3501BE6BECA672DB18)    | 2021-02-12   | Yes         |                    38 |
| [Chimchar](https://metrics.torproject.org/rs.html#details/ED967A94B73BF678660EAA91890F450250CA0575)     | 2021-03-16   | Yes         |                    38 |
| [Snivy](https://metrics.torproject.org/rs.html#details/D4C733CA1FF5D85C3571FF39DBC7DB431966A47D)        | 2021-03-19   | Yes         |                    38 |
| [Moonpie](https://metrics.torproject.org/rs.html#details/096DE80D4C1E457680C23B56B6DABE9AA6A6260C)      | 2021-02-18   | Yes         |                    38 |
| [Rowlet](https://metrics.torproject.org/rs.html#details/690FC3ACBBBC970309A9A0993EE12AF44C0C8E62)       | 2021-03-16   | Yes         |                    38 |
| [MoonBeam](https://metrics.torproject.org/rs.html#details/B08504ABC6BBA71D78163EADDB8D8248D7DB53F4)     | 2021-03-05   | Yes         |                    38 |
| [Moonlight](https://metrics.torproject.org/rs.html#details/9546182589B1E4BF6B025875FAEBE309E7359D56)    | 2021-03-05   | Yes         |                    38 |
| [Charmander](https://metrics.torproject.org/rs.html#details/45DC9BCF0E44A22D246ECC02234B216EAA02155E)   | 2021-03-08   | Yes         |                    38 |
| [Piplup](https://metrics.torproject.org/rs.html#details/62F65E6377F0647CE0F0EE2AAE1641EC4AA2BD3B)       | 2021-03-07   | Yes         |                    38 |
| [Rachmaninoff](https://metrics.torproject.org/rs.html#details/DF187D0E3481F6C6FE60836C28AE4948A77A4761) | 2021-05-05   | Yes         |                    38 |
| [Squirtle](https://metrics.torproject.org/rs.html#details/ADDFC1F6208B4C59A6FF3DAAA5A93B481720595A)     | 2021-03-08   | Yes         |                    38 |
| [greaseball](https://metrics.torproject.org/rs.html#details/B4EE5535230F742EE53A523E505296850F8FE0C9)   | 2021-06-03   | Yes         |                    38 |
| [Litten](https://metrics.torproject.org/rs.html#details/F1C4F08DE356EFC6495B40E3E7698F0ACAD4C5AC)       | 2021-05-19   | Yes         |                    38 |
| [Chikorita](https://metrics.torproject.org/rs.html#details/55566C567D7F9E9EE70368AEFA29593EC34FB0A5)    | 2021-03-09   | Yes         |                    38 |
| [Pickachu](https://metrics.torproject.org/rs.html#details/34F2DBF5595FF8323665BEC7DD8D2D28F9697B2C)     | 2021-03-07   | Yes         |                    38 |
| [Cyndaquil](https://metrics.torproject.org/rs.html#details/ADA98E1C50E0635BDDECB4C9D448C72040275045)    | 2021-03-09   | Yes         |                    38 |
| [Totodile](https://metrics.torproject.org/rs.html#details/BF8A9BCA68F14B49939063B7BD3D32E23533C125)     | 2021-03-09   | Yes         |                    38 |
| [FreeTshirt](https://metrics.torproject.org/rs.html#details/CACEAEC72943BB2AE8C36C4751989F9E4F2E5178)   | 2021-05-28   | Yes         |                    38 |
| [Bastion](https://metrics.torproject.org/rs.html#details/E9EF002E8D2911AFAB1121EF281858484F3ECA73)      | 2021-05-28   | Yes         |                    34 |
| [FreePants](https://metrics.torproject.org/rs.html#details/FD4281E65C32BFC1096FCA73645F589408067149)    | 2021-05-28   | Yes         |                    38 |
| [dragonbleu](https://metrics.torproject.org/rs.html#details/24DC6F435824B3D82BFD7841D6FC2216BA11B8BC)   | 2021-05-05   | No          |                    39 |
| [saturn](https://metrics.torproject.org/rs.html#details/5ECBA2DDE6403E0F0B73E452F65EA2606929332A)       | 2021-05-09   | No          |                    38 |
| [Mudkip](https://metrics.torproject.org/rs.html#details/75983F5660D894FCF2BE452DB35F3E594ADE4B08)       | 2021-03-13   | No          |                    38 |
| [Torchick](https://metrics.torproject.org/rs.html#details/91D129CEBBC3F1BE27BCF8019F1F7A8B0F27E1C2)     | 2021-03-13   | No          |                    38 |
| [Treecko](https://metrics.torproject.org/rs.html#details/E0F4900D063080D44AB4C043FBAB4C2F964CB612)      | 2021-03-11   | No          |                    38 |

## ContactInfo: xKek Operations &lt;system@lysergic.dev&gt; (8) {#xkek-operations-systemlysergicdev}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [cynthia](https://metrics.torproject.org/rs.html#details/519137667154E62261381ED5B912898E7DBDC60C)  | 2021-06-10   | Yes         |                     7 |
| [thetrip](https://metrics.torproject.org/rs.html#details/424F9C80A25843A2E60EDACCD3092D31D300FD74)  | 2021-06-10   | Yes         |                     7 |
| [centauri](https://metrics.torproject.org/rs.html#details/BA45EB745D44E7FEA375AFF45A4C82C51E4C2B71) | 2021-06-10   | Yes         |                     6 |
| [makemake](https://metrics.torproject.org/rs.html#details/C1768D9F00A12189BAAC9B61C5B9854392271CAF) | 2021-06-10   | Yes         |                     7 |
| [cashew](https://metrics.torproject.org/rs.html#details/8063D1DCE54116090DD1B03E0D602E4AABE281F1)   | 2021-06-20   | No          |                     1 |
| [puddle](https://metrics.torproject.org/rs.html#details/9AF0C9EB3BDE62145DCE690CC82B9B8D79987E10)   | 2021-06-11   | No          |                     6 |
| [cuddle](https://metrics.torproject.org/rs.html#details/C1734E8C2D2DC1A579794DFA209C7CBCFA2B26F7)   | 2021-06-11   | No          |                     7 |
| [peanuts](https://metrics.torproject.org/rs.html#details/F62B74728AC72A495C986255199D9AF19CCA5B51)  | 2021-06-10   | No          |                     7 |

## ContactInfo: 4punk7 AT mailbox dot org (4) {#4punk7-at-mailbox-dot-org}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [4punk7r1](https://metrics.torproject.org/rs.html#details/ABA31795BAD2AB8097F3AD0FE1A920E518D3D3F3) | 2020-04-02   | Yes         |                     1 |
| [4punk7r2](https://metrics.torproject.org/rs.html#details/CB2DBDB2D9422D57AD85148EF9511AF4CE4D6052) | 2020-04-04   | Yes         |                     1 |
| [4punk7e1](https://metrics.torproject.org/rs.html#details/2E0C69E59B5B6AA15BB1C269690722607663416C) | 2020-11-27   | No          |                     1 |
| [4punk7e3](https://metrics.torproject.org/rs.html#details/F42FF0E095F23AD253622272F984649DDEEB402C) | 2020-10-26   | No          |                     1 |

## ContactInfo: potlatch protonmail com (7) {#potlatch-protonmail-com}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [TorExitAlbania2](https://metrics.torproject.org/rs.html#details/D78D1B4489CF4FFB0FD74014BDF2D600D8EE5B05) | 2020-06-13   | Yes         |                     8 |
| [TorExitLatvia](https://metrics.torproject.org/rs.html#details/08CD9D4224058DC97A1F27679A5BEE5724C4C6EC)   | 2020-08-15   | Yes         |                     8 |
| [TorExitBulgaria](https://metrics.torproject.org/rs.html#details/961B9D86125A08FAA9F7E742B228307EF7E2E082) | 2021-06-30   | Yes         |                     1 |
| [TorExitRomania](https://metrics.torproject.org/rs.html#details/4061C553CA88021B8302F0814365070AAE617270)  | 2016-03-02   | No          |                     8 |
| [TorExitMoldova2](https://metrics.torproject.org/rs.html#details/742C45F2D9004AADE0077E528A4418A6A81BC2BA) | 2019-01-01   | No          |                     8 |
| [TorExitFinland](https://metrics.torproject.org/rs.html#details/9B31F1F1C1554F9FFB3455911F82E818EF7C7883)  | 2015-12-31   | No          |                     8 |
| [TorExitMoldova](https://metrics.torproject.org/rs.html#details/B06F093A3D4DFAD3E923F4F28A74901BD4F74EB1)  | 2017-05-24   | No          |                     8 |

## ContactInfo: torix aT=== protonmail&lt;dOT &gt;com (8) {#torixatprotonmaildotcom}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Aramis67](https://metrics.torproject.org/rs.html#details/53C9F4954E7A7332BB0C610C5B8E04CA065AF29B) | 2019-05-13   | Yes         |                     7 |
| [Aramis72](https://metrics.torproject.org/rs.html#details/F5FD7EF4307F8C5C398147877F32A9F9F71E2092) | 2020-05-27   | Yes         |                     7 |
| [Aramis66](https://metrics.torproject.org/rs.html#details/39A18F31B312E5CB211781090766934C1CFDAB36) | 2020-07-10   | Yes         |                     2 |
| [Aramis75](https://metrics.torproject.org/rs.html#details/4D2A4831BB67853A6FA01517A61B810D4480AE2F) | 2020-10-30   | No          |                     7 |
| [Aramis73](https://metrics.torproject.org/rs.html#details/5FCB4186E2BCD4E8E510EACEC7AABE2194CA36BC) | 2020-10-30   | No          |                     6 |
| [Aramis71](https://metrics.torproject.org/rs.html#details/AB32B2EA350C10888144A7ECCA7FFACA844C2052) | 2020-04-27   | No          |                     7 |
| [Aramis74](https://metrics.torproject.org/rs.html#details/B8F6C6A0F6D0ACBEB3D39B1D99161EFACCE27E6F) | 2020-10-30   | No          |                     7 |
| [Aramis70](https://metrics.torproject.org/rs.html#details/DEAA89B5B8D9CEAD5CE0F9281D482A4EACC30592) | 2020-05-02   | No          |                     7 |


## Fingerprint List of Guard-only Relays in E2E Groups

07007CB632002FC92FB11DE78C72C44B5160A1A3,096DE80D4C1E457680C23B56B6DABE9AA6A6260C,1A647701D0368E8F073FF38773986F43A24C60CA,261A7D651D319021D7141B7CE3ECA6E9DA983540,3326C64CD86258ACA4657E3501BE6BECA672DB18,34F2DBF5595FF8323665BEC7DD8D2D28F9697B2C,45DC9BCF0E44A22D246ECC02234B216EAA02155E,51BD782616C3EBA543B0D4EE34D7C1CE1ED2291D,55566C567D7F9E9EE70368AEFA29593EC34FB0A5,55ED11C6B5A35D40CD07F5A8DC12B82F0B7AADDF,62F65E6377F0647CE0F0EE2AAE1641EC4AA2BD3B,690FC3ACBBBC970309A9A0993EE12AF44C0C8E62,751EDB5D969C72479270D223823A8ED4E578C070,8B9110B997437724115CFCDB1B2495463F77669B,9546182589B1E4BF6B025875FAEBE309E7359D56,9F1687D0D79A74F2C6F9FB918089405565BA5329,ADA98E1C50E0635BDDECB4C9D448C72040275045,ADDFC1F6208B4C59A6FF3DAAA5A93B481720595A,B08504ABC6BBA71D78163EADDB8D8248D7DB53F4,B4EE5535230F742EE53A523E505296850F8FE0C9,BF8A9BCA68F14B49939063B7BD3D32E23533C125,C1C239582DDDA2DFCE674D365861FB2C1A96D8B9,CACEAEC72943BB2AE8C36C4751989F9E4F2E5178,D4C733CA1FF5D85C3571FF39DBC7DB431966A47D,DC4349041B89D9FDD4DC53BD680B42B37A9CB195,DC862F7BBF619EA3FA4FB667A4D8118652922FC8,DF187D0E3481F6C6FE60836C28AE4948A77A4761,E789DDCFDF2F92F3A6548796A22D5C8E64EE1A1B,E9EF002E8D2911AFAB1121EF281858484F3ECA73,ED967A94B73BF678660EAA91890F450250CA0575,F1C4F08DE356EFC6495B40E3E7698F0ACAD4C5AC,424F9C80A25843A2E60EDACCD3092D31D300FD74,519137667154E62261381ED5B912898E7DBDC60C,BA45EB745D44E7FEA375AFF45A4C82C51E4C2B71,C1768D9F00A12189BAAC9B61C5B9854392271CAF,ABA31795BAD2AB8097F3AD0FE1A920E518D3D3F3,CB2DBDB2D9422D57AD85148EF9511AF4CE4D6052,08CD9D4224058DC97A1F27679A5BEE5724C4C6EC,373BF7A2CD16E86D4C5BEC591A41945C9AED392D,961B9D86125A08FAA9F7E742B228307EF7E2E082,D78D1B4489CF4FFB0FD74014BDF2D600D8EE5B05,39A18F31B312E5CB211781090766934C1CFDAB36,53C9F4954E7A7332BB0C610C5B8E04CA065AF29B,F5FD7EF4307F8C5C398147877F32A9F9F71E2092,FD4281E65C32BFC1096FCA73645F589408067149