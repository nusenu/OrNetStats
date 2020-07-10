---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-07-09 16:00 UTC**

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


## ContactInfo: abuse-contact@to-surf-and-protect.net (136) {#abuse-contactto-surf-and-protectnet}

| Nickname                                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [niftycongogerbil](https://metrics.torproject.org/rs.html#details/85A3AC041E3FCD796AF5D653953D5E27A56E3719)    | 2019-01-31   | Yes         |                     1 |
| [niftymastomys](https://metrics.torproject.org/rs.html#details/24E1C6412183972BFD76D838AC04D1ED261743D3)       | 2019-01-31   | Yes         |                     1 |
| [niftyshrew](https://metrics.torproject.org/rs.html#details/A39721D284AA1ED1AE87AE63523535484AA14FB5)          | 2019-12-01   | Yes         |                     1 |
| [niftyphoberomys](https://metrics.torproject.org/rs.html#details/87D73471FDC64BD9CEDF84435D20CA4EB5C36FE8)     | 2019-01-05   | Yes         |                   142 |
| [niftyalloeumyarion](https://metrics.torproject.org/rs.html#details/96CFE178A1D12489D9D59A0CAE17FE86F5A3A79F)  | 2019-01-05   | Yes         |                   142 |
| [niftywatersgerbil](https://metrics.torproject.org/rs.html#details/E97DAC45ED2AB46DD830A279BDCC7AFCE10EE674)   | 2019-01-30   | Yes         |                     2 |
| [niftylinkrat](https://metrics.torproject.org/rs.html#details/5DE37A3371AAE7638748EB43C9F1CE66E09D4470)        | 2019-01-31   | Yes         |                     1 |
| [niftydiatomys](https://metrics.torproject.org/rs.html#details/A016192D0A87FC9354A7523A211BBD9CF859708B)       | 2019-01-05   | Yes         |                   142 |
| [niftyleastgerbil](https://metrics.torproject.org/rs.html#details/6FBD65C22C2996B2038A090BF5E55AA7AEDEE120)    | 2019-01-30   | Yes         |                     2 |
| [niftyflorescaverat](https://metrics.torproject.org/rs.html#details/0677DF0B05ECDA2EF45F26C3332731043BB89AB8)  | 2019-01-05   | Yes         |                   142 |
| [niftyentry116](https://metrics.torproject.org/rs.html#details/02758CD398E3F842EF82478078AAAE0273770DB2)       | 2020-03-27   | Yes         |                   142 |
| [niftyentry100](https://metrics.torproject.org/rs.html#details/7ED3D8AFAC750F8CC0BDF8C87FE3BCBA2BBE2209)       | 2020-03-27   | Yes         |                   142 |
| [niftyentry117](https://metrics.torproject.org/rs.html#details/BCDE75725B927738B6FD34EA2D78F4FA77B99848)       | 2020-03-27   | Yes         |                   142 |
| [niftyentry115](https://metrics.torproject.org/rs.html#details/5CCC3569C67B7F1BB733664D43DF4645F2A4B04D)       | 2020-03-27   | Yes         |                   142 |
| [niftywabbit8](https://metrics.torproject.org/rs.html#details/FDFD675D05216549EB7DA545E32ECFCEEAE805F2)        | 2020-02-02   | Yes         |                   142 |
| [niftyentrynice](https://metrics.torproject.org/rs.html#details/7B7C7F31205D7AEB5DFFEDA08E00282A78CD76E0)      | 2020-03-27   | Yes         |                   142 |
| [niftyentry99](https://metrics.torproject.org/rs.html#details/8CA736F332937E4FA0F5F48488B823F31883123C)        | 2020-03-27   | Yes         |                   142 |
| [niftyentry80](https://metrics.torproject.org/rs.html#details/8BE58BA7A28DC6B4F211CE8EE86783B85133488D)        | 2020-03-27   | Yes         |                   142 |
| [niftyexit8](https://metrics.torproject.org/rs.html#details/2E44E8EB8C7711C1157BD8025F07165CFF8FA2B6)          | 2020-03-19   | Yes         |                   142 |
| [niftywabbit14](https://metrics.torproject.org/rs.html#details/24352D30196BEFE5BB29A50923F79A2804527611)       | 2020-03-26   | Yes         |                   142 |
| [niftyentry103](https://metrics.torproject.org/rs.html#details/7226BE09B7A81000BBF7D959E360B2FE41CCC639)       | 2020-03-27   | Yes         |                   142 |
| [niftyentry95](https://metrics.torproject.org/rs.html#details/863FDDA3CA537CE03646B3AEBD3FD1CC6B077FBE)        | 2020-03-27   | Yes         |                   142 |
| [niftyguard49](https://metrics.torproject.org/rs.html#details/8839E8FBE28219B85392EEA5A4DBC41D315F4B83)        | 2020-03-26   | Yes         |                   142 |
| [niftyguard09](https://metrics.torproject.org/rs.html#details/31F373571AA6ECB4D73266E114D58B0AF7227369)        | 2020-03-26   | Yes         |                   142 |
| [niftyexit1](https://metrics.torproject.org/rs.html#details/EEB8F7554A54A96B51245AB47EB7B7DD99A98493)          | 2020-03-20   | Yes         |                   142 |
| [niftyentry108](https://metrics.torproject.org/rs.html#details/28A4C64C34120E075701B0415D74906EC687F21F)       | 2020-03-27   | Yes         |                   142 |
| [niftywabbit15](https://metrics.torproject.org/rs.html#details/4AD9C116A1942D58A714433CA24F087F18036A7E)       | 2020-03-26   | Yes         |                   142 |
| [niftyentry77](https://metrics.torproject.org/rs.html#details/01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)        | 2020-03-27   | No          |                   142 |
| [niftyguard15](https://metrics.torproject.org/rs.html#details/05F5BB75DA007361CE03770393033D4D52836D8A)        | 2020-03-26   | No          |                   142 |
| [niftyguard19](https://metrics.torproject.org/rs.html#details/0A4ED4C74020740A904F3A9936030B7A4C6170BB)        | 2020-03-26   | No          |                   142 |
| [niftyboglemming](https://metrics.torproject.org/rs.html#details/0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)     | 2019-01-25   | No          |                   142 |
| [niftyhazelmouse](https://metrics.torproject.org/rs.html#details/0FB2EDAB99D10A2B708370E625323C76EB895FA2)     | 2019-01-31   | No          |                   142 |
| [niftywabbit](https://metrics.torproject.org/rs.html#details/10644CF3D7F555F10FE28EB1D520111F56FE7180)         | 2020-02-02   | No          |                   142 |
| [niftyhedgehog](https://metrics.torproject.org/rs.html#details/1084200B44021D308EA4253F256794671B1D099A)       | 2016-08-23   | No          |                   142 |
| [niftywoodmouse](https://metrics.torproject.org/rs.html#details/14877C6384A9E793F422C8D1DDA447CACA4F7C4B)      | 2016-09-18   | No          |                   142 |
| [niftywabbit13](https://metrics.torproject.org/rs.html#details/1B605B2751279B152CA098ED76B1EBCC9ADCA239)       | 2020-03-26   | No          |                   142 |
| [niftyguard36](https://metrics.torproject.org/rs.html#details/1B9235656503E80E913E9C9A139AD89D36E2DFFD)        | 2020-03-26   | No          |                   142 |
| [niftylagurus](https://metrics.torproject.org/rs.html#details/1D89A810BDF84522B6036034F499A766EF294DB1)        | 2019-01-26   | No          |                   142 |
| [niftymouse](https://metrics.torproject.org/rs.html#details/24E91955D969AEA1D80413C64FE106FAE7FD2EA9)          | 2016-07-27   | No          |                   142 |
| [niftyrabbitrat](https://metrics.torproject.org/rs.html#details/25526E61B8BC22B662E3D4A50504021CC3D9873D)      | 2018-01-12   | No          |                   142 |
| [niftywoodlandvole](https://metrics.torproject.org/rs.html#details/283312BB249FCB6633A7C7E1E8241461000E6004)   | 2019-06-24   | No          |                   142 |
| [niftycottonmouse](https://metrics.torproject.org/rs.html#details/28F4F392F8F19E3FBDE09616D9DB8143A1E2DDD3)    | 2016-10-23   | No          |                   142 |
| [niftyneochoerus](https://metrics.torproject.org/rs.html#details/2A231A5CA7AF91029B7475511D7D16DF85EC9221)     | 2019-01-05   | No          |                   142 |
| [niftywabbit2](https://metrics.torproject.org/rs.html#details/2F64EA527C4AA6F99E261318DD1FF127828E2525)        | 2020-02-02   | No          |                   142 |
| [niftywabbit](https://metrics.torproject.org/rs.html#details/30DBF7A773F4EE3BF6D1B7407DAECF40220AC8CD)         | 2020-02-02   | No          |                   142 |
| [niftysquirrel](https://metrics.torproject.org/rs.html#details/348B89013EDDD99E4755951D1EC284D9FED71226)       | 2016-09-20   | No          |                   142 |
| [niftyentry78](https://metrics.torproject.org/rs.html#details/380F79145FF9C2332CBF41313062C99DBA9B0E50)        | 2020-03-27   | No          |                   142 |
| [niftywoodlemming](https://metrics.torproject.org/rs.html#details/3F129FB71EB2B019B47403A5552EB2D40E5369F2)    | 2019-01-25   | No          |                   142 |
| [niftyeuropeanrabbit](https://metrics.torproject.org/rs.html#details/4031460683AE9E0512D3620C2758D98758AC6C93) | 2017-12-30   | No          |                   142 |
| [niftyguard](https://metrics.torproject.org/rs.html#details/456F6E4998EB17B975DB5A19273607868E5F8AFA)          | 2020-03-26   | No          |                   142 |
| [niftywabbit20](https://metrics.torproject.org/rs.html#details/470BC5C6A8BD1D9FDBB55689FB3030310181EAE2)       | 2020-03-26   | No          |                   142 |
| [niftysugarglider](https://metrics.torproject.org/rs.html#details/47C42E2094EE482E7C9B586B10BABFB67557030B)    | 2016-08-30   | No          |                   142 |
| [niftysteppemarmot](https://metrics.torproject.org/rs.html#details/48BE372CA2104D2422D49CD321060E7F697B52D9)   | 2019-01-31   | No          |                   142 |
| [niftyguard41](https://metrics.torproject.org/rs.html#details/4AD0B40B0FC679CC300F398BCEBE9D000833F62C)        | 2020-03-26   | No          |                   142 |
| [niftyguard54](https://metrics.torproject.org/rs.html#details/4C07CB3365CF3E06A56FD2DC8ECA4E97A6521983)        | 2020-03-26   | No          |                   142 |
| [niftywabbit18](https://metrics.torproject.org/rs.html#details/50A0CFB654D39F420F52D362B1DF50A12B33D5A0)       | 2020-03-26   | No          |                   142 |
| [niftydiatomys](https://metrics.torproject.org/rs.html#details/50B787A9FB21417BFD7B5067707DBF82D71DB11C)       | 2019-06-24   | No          |                   142 |
| [niftywabbit9](https://metrics.torproject.org/rs.html#details/50D1473A213DB343E97664C71C09D28EC2692CB3)        | 2020-02-02   | No          |                   142 |
| [niftywabbit11](https://metrics.torproject.org/rs.html#details/520C85ABE6E731CECC28B1055854053FAA28061B)       | 2020-03-26   | No          |                   142 |
| [niftywabbit4](https://metrics.torproject.org/rs.html#details/53CBD4285918F168B92D05CAA9BC0CF499DF72C7)        | 2020-02-02   | No          |                   142 |
| [niftyentry83](https://metrics.torproject.org/rs.html#details/562C61C7F885741D599DB7A1235791D928BEADFD)        | 2020-03-27   | No          |                   142 |
| [niftyafricagiantrat](https://metrics.torproject.org/rs.html#details/56850752096EE63711F99B2FA5A812477561697D) | 2019-10-26   | No          |                   142 |
| [niftyguard26](https://metrics.torproject.org/rs.html#details/583CEFCFF76B3189D3A37C81A49D1619D04DCB34)        | 2020-03-26   | No          |                   142 |
| [niftyguard44](https://metrics.torproject.org/rs.html#details/5B9BB7A543C2C035A423A6B411780E50645782C0)        | 2020-03-26   | No          |                   142 |
| [niftychipmunk](https://metrics.torproject.org/rs.html#details/609E598FB6A00BCF7872906B602B705B64541C50)       | 2016-08-28   | No          |                   142 |
| [niftytucotuco](https://metrics.torproject.org/rs.html#details/619349D82424C601CAEB94161A4CF778993DAEE7)       | 2016-10-20   | No          |                   142 |
| [niftyentry75](https://metrics.torproject.org/rs.html#details/621EA822CEAC095845A0CFFFA503D2993AB10FF3)        | 2020-03-27   | No          |                   142 |
| [niftyguard52](https://metrics.torproject.org/rs.html#details/6372CADE2B9A608E5114002A7A825AF0D11B449A)        | 2020-03-26   | No          |                   142 |
| [niftyhutia](https://metrics.torproject.org/rs.html#details/644DECC5A1879C0FE23DE927DD7049F58BBDF349)          | 2016-09-22   | No          |                   142 |
| [niftyhare](https://metrics.torproject.org/rs.html#details/6781471814DF164C2A6F17CD1F2584923FDE2101)           | 2018-02-03   | No          |                   142 |
| [niftyhornedgopher](https://metrics.torproject.org/rs.html#details/6C64AE6D7EFDA52A463FB6ADCDAE2D2DDE0677C3)   | 2019-01-05   | No          |                   142 |
| [niftyguard56](https://metrics.torproject.org/rs.html#details/6CB7D0F355B60EF166439E96876BCDEBF8FD8E0F)        | 2020-03-26   | No          |                   142 |
| [niftybeaver](https://metrics.torproject.org/rs.html#details/6E94866ED8CA098BACDFD36D4E8E2B459B8A734E)         | 2016-11-23   | No          |                   142 |
| [niftyentry79](https://metrics.torproject.org/rs.html#details/71730F1BEB5372C9A6FF36704FF1A6A48AEE7813)        | 2020-03-27   | No          |                   142 |
| [niftycottontail](https://metrics.torproject.org/rs.html#details/71AB4726D830FAE776D74AEF790CF04D8E0151B4)     | 2016-02-05   | No          |                   142 |
| [niftyguard21](https://metrics.torproject.org/rs.html#details/7404DC4E6B17D5B751BF343E509F6D4B940FC104)        | 2020-03-26   | No          |                   142 |
| [niftywabbit6](https://metrics.torproject.org/rs.html#details/7C7FFB1C48B7E0C5C9B3D11FEC2F8500F464786A)        | 2020-02-02   | No          |                   142 |
| [niftymuskrat](https://metrics.torproject.org/rs.html#details/7D921363817BE896B5462E90033DA937BEF7CE3F)        | 2019-08-09   | No          |                   142 |
| [niftyllipika](https://metrics.torproject.org/rs.html#details/7DC52AE6667A30536BA2383CD102CFC24F20AD71)        | 2016-12-02   | No          |                   142 |
| [niftyporcupine](https://metrics.torproject.org/rs.html#details/7E281CD2C315C4F7A84BC7C8721C3BC974DDBFA3)      | 2016-11-25   | No          |                   142 |
| [niftyguard02](https://metrics.torproject.org/rs.html#details/7F7BE7926AF718D6A3DED24D694D94C1D5FACF28)        | 2020-03-26   | No          |                   142 |
| [niftyguard57](https://metrics.torproject.org/rs.html#details/8054F105829438B029E7265BB1070F9258705112)        | 2020-03-26   | No          |                   142 |
| [niftytamiasaristus](https://metrics.torproject.org/rs.html#details/88AE3BC088396F1D3FCC4F2F588C0DC837599D20)  | 2018-12-16   | No          |                   142 |
| [niftyjerboa](https://metrics.torproject.org/rs.html#details/8EE0534532EA31AA5172B1892F53B2F25C76EB02)         | 2016-08-30   | No          |                   142 |
| [niftyentry74](https://metrics.torproject.org/rs.html#details/8FF2896A94BCAA5F0A7C5A56AD6586492CD448AF)        | 2020-03-27   | No          |                   142 |
| [niftywabbit12](https://metrics.torproject.org/rs.html#details/902E21BC05A7B1EC8CE85D78C47C3D8EAD5EFE6F)       | 2020-03-26   | No          |                   142 |
| [niftyquokka](https://metrics.torproject.org/rs.html#details/906DCB390F2BA987AE258D745E60BAAABAD31DE8)         | 2016-08-03   | No          |                   142 |
| [niftypedetes](https://metrics.torproject.org/rs.html#details/92A6085EABAADD928B6F8E871540A1A41CBC08BA)        | 2016-08-24   | No          |                   142 |
| [niftytamiasatsali](https://metrics.torproject.org/rs.html#details/957354D72042719C310A907FBFE42A3232C78757)   | 2019-01-26   | No          |                   142 |
| [niftyentry92](https://metrics.torproject.org/rs.html#details/95B9052EECDB4B833F130ABD564E720643BA7952)        | 2020-03-27   | No          |                   142 |
| [niftyguard71](https://metrics.torproject.org/rs.html#details/9634E9F53EB46828AE7E06839FEE595950286B1D)        | 2020-03-26   | No          |                   142 |
| [niftywabbit16](https://metrics.torproject.org/rs.html#details/9664A7EFB405F555F3C0079FA7618B2EE6CE6D2A)       | 2020-03-26   | No          |                   142 |
| [niftyredsquirrel](https://metrics.torproject.org/rs.html#details/97D2A26EA5C9972E66D23F4698E94DBDBA8F6C18)    | 2019-01-31   | No          |                   142 |
| [niftyspinymouse](https://metrics.torproject.org/rs.html#details/986E29FB17C8C7A1FEAFF203F012D5930BA079DB)     | 2019-01-31   | No          |                   142 |
| [niftyfoxsquirrel](https://metrics.torproject.org/rs.html#details/9910C6DEEA9907EE7AEFCE0DA072F94F86EBFD48)    | 2019-10-23   | No          |                   142 |
| [niftypygmyjerboa](https://metrics.torproject.org/rs.html#details/9B816A5B3EB20B8E4E9B9D1FBA299BD3F40F0320)    | 2017-12-27   | No          |                   142 |
| [niftyredrockrat](https://metrics.torproject.org/rs.html#details/9B94A776DA2C0B974BF4E06A352133EDFE62036C)     | 2019-01-31   | No          |                   142 |
| [niftycastoroides](https://metrics.torproject.org/rs.html#details/9EEDBAD7EE351996DFC91578E882BEF4FE5EDBFA)    | 2019-01-05   | No          |                   142 |
| [niftywabbit10](https://metrics.torproject.org/rs.html#details/A14F90953AE9462CF3A862C4CA95F73BF94A6F8B)       | 2020-02-02   | No          |                   142 |
| [niftysnowshoehare](https://metrics.torproject.org/rs.html#details/A3901DDB7799A11E9BAB90BD1DDA734DBA196337)   | 2019-06-24   | No          |                   142 |
| [niftyguard74](https://metrics.torproject.org/rs.html#details/A78E86015376B3F2507E2E6602FDFD278F2871B3)        | 2020-03-26   | No          |                   142 |
| [niftyguard46](https://metrics.torproject.org/rs.html#details/AD1359B9D74D526FEF3F58AF41105C623A3A8C18)        | 2020-03-26   | No          |                   142 |
| [niftyguard60](https://metrics.torproject.org/rs.html#details/AF022F351A4B6F2514A09F9245F9FF5ACA729735)        | 2020-03-26   | No          |                   142 |
| [niftywabbit17](https://metrics.torproject.org/rs.html#details/B36006D88E2CCEF2E1EF0826C7F1B0EDC8DE6C06)       | 2020-03-26   | No          |                   142 |
| [niftyalloumyraion](https://metrics.torproject.org/rs.html#details/B4DD1F46C6E5B43D9654FF56BD32333D6586E536)   | 2019-06-24   | No          |                   142 |
| [niftybunny](https://metrics.torproject.org/rs.html#details/B740BCECC4A9569232CDD45C0E1330BA0D030D33)          | 2017-12-27   | No          |                   142 |
| [niftypika](https://metrics.torproject.org/rs.html#details/B771AA877687F88E6F1CA5354756DF6C8A7B6B24)           | 2016-01-25   | No          |                   142 |
| [niftyguard59](https://metrics.torproject.org/rs.html#details/BC38744FD82618B37EE6A5A61BBCCE8788D55E3D)        | 2020-03-26   | No          |                   142 |
| [niftybankvole](https://metrics.torproject.org/rs.html#details/C00C28C2B1A7D8038517626CECA9BCB23B0A31D2)       | 2019-01-25   | No          |                   142 |
| [niftyvolcanorabbit](https://metrics.torproject.org/rs.html#details/C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)  | 2016-02-06   | No          |                   142 |
| [niftywabbit3](https://metrics.torproject.org/rs.html#details/C47E8F025645C621BE8BF8B5F6C8564A41259F7B)        | 2020-02-02   | No          |                   142 |
| [niftyentry85](https://metrics.torproject.org/rs.html#details/C6E184C0983C68B7E8BFC6215E7289E09E97AA0E)        | 2020-03-27   | No          |                   142 |
| [niftywabbit19](https://metrics.torproject.org/rs.html#details/C74469EC04787CC458FB1DCDF456C5092CF08B19)       | 2020-03-26   | No          |                   142 |
| [niftyguard07](https://metrics.torproject.org/rs.html#details/C8F6F6C1834454F1E927A4A05E8E54EB623D4B73)        | 2020-03-26   | No          |                   142 |
| [niftyjackrabbit](https://metrics.torproject.org/rs.html#details/CA37CD46799449D83B6B98B8C22C649906307888)     | 2017-12-27   | No          |                   142 |
| [niftychionomy](https://metrics.torproject.org/rs.html#details/CD97DD0842A79184A7D057ECACEF7408C239C710)       | 2019-01-25   | No          |                   142 |
| [niftygerbil](https://metrics.torproject.org/rs.html#details/CDA2EA326E2272C57ACB26773D7252C211795B78)         | 2016-05-22   | No          |                   142 |
| [niftytelicomys](https://metrics.torproject.org/rs.html#details/D27208881BBDB5EA56EFD1D1799187519591E325)      | 2019-01-05   | No          |                   142 |
| [niftyentry64](https://metrics.torproject.org/rs.html#details/D286ED33FCB28385BAD9DA3D6B12A604C0834313)        | 2020-03-27   | No          |                   142 |
| [niftywabbit5](https://metrics.torproject.org/rs.html#details/DFAA86AD46BEA875D5018CC1CECD77C9F979FB0E)        | 2020-02-02   | No          |                   142 |
| [niftyblythsvole](https://metrics.torproject.org/rs.html#details/E013CC98CCC1E6AFDCFC9681A53DC2DEFE5D4CCC)     | 2019-01-25   | No          |                   142 |
| [niftyentry88](https://metrics.torproject.org/rs.html#details/E2B9BA96723C59E65AE07E82B74C7A31AF874225)        | 2020-03-27   | No          |                   142 |
| [niftyexit](https://metrics.torproject.org/rs.html#details/E321D0118DAD44BBC74A5C26FE7CFDBAAF3DA077)           | 2020-03-19   | No          |                   142 |
| [niftyentry71](https://metrics.torproject.org/rs.html#details/E330A88754840629644527394FD43001D5B89C7A)        | 2020-03-27   | No          |                   142 |
| [niftyhousemouse](https://metrics.torproject.org/rs.html#details/E4B04C7D734B2294E8ECE057303E89B91EE88462)     | 2019-08-09   | No          |                   142 |
| [niftydormouse](https://metrics.torproject.org/rs.html#details/E6FAC9A7F33EE66F03C55C119770B2D45D3C576B)       | 2016-11-25   | No          |                   142 |
| [niftyguineapig](https://metrics.torproject.org/rs.html#details/EC1997D51892E4607C68E800549A1E7E4694005A)      | 2016-05-25   | No          |                   142 |
| [niftyentry70](https://metrics.torproject.org/rs.html#details/ED6AF8CE8CF4126A6F33572376B6D8977FED2DD9)        | 2020-03-27   | No          |                   142 |
| [niftyjunipervole](https://metrics.torproject.org/rs.html#details/EDC4243F57F9B856B400398D5F6C354F8408EEA9)    | 2019-01-25   | No          |                   142 |
| [niftyentry67](https://metrics.torproject.org/rs.html#details/EE859849E8D8EF083EEF2025555396A6C3552A8E)        | 2020-03-27   | No          |                   142 |
| [niftyguard42](https://metrics.torproject.org/rs.html#details/F8AEA2825629E4383599FD2A4BD5740CD1322CBC)        | 2020-03-26   | No          |                   142 |
| [niftyleithia](https://metrics.torproject.org/rs.html#details/F8E9C0C3A4B61E7599AA7A23D7ADE77E5BAB2663)        | 2019-01-05   | No          |                   142 |
| [niftytreerat](https://metrics.torproject.org/rs.html#details/FAEC86A9A37152F0371D67917ABA398467DFBD9C)        | 2018-01-11   | No          |                   142 |
| [niftyguard43](https://metrics.torproject.org/rs.html#details/FB8796036069BB4787D639F92681ECC2FD7AEB22)        | 2020-03-26   | No          |                   142 |
| [niftyrat](https://metrics.torproject.org/rs.html#details/FDA70EC93DB01E3CB418CB6943B0C68464B18B4C)            | 2016-09-17   | No          |                   142 |
| [niftyguard11](https://metrics.torproject.org/rs.html#details/FDBF608F9A2ECD0C600CAF96398A7D5B08D46CA9)        | 2020-03-26   | No          |                   142 |

## ContactInfo: tomas.vanagas@knf.vu.lt tor-relay.co (2) {#tomasvanagasknfvult-tor-relayco}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [SatoshiNakamoto](https://metrics.torproject.org/rs.html#details/64B43A6198B6C1F97D9ED8929F5A8913C3815935) | 2020-04-28   | Yes         |                     1 |
| [SatoshiNakamoto](https://metrics.torproject.org/rs.html#details/1939CC1B41298A49C0684878813DED5CD1A9EE98) | 2019-03-29   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

02758CD398E3F842EF82478078AAAE0273770DB2,0677DF0B05ECDA2EF45F26C3332731043BB89AB8,24352D30196BEFE5BB29A50923F79A2804527611,24E1C6412183972BFD76D838AC04D1ED261743D3,28A4C64C34120E075701B0415D74906EC687F21F,2E44E8EB8C7711C1157BD8025F07165CFF8FA2B6,31F373571AA6ECB4D73266E114D58B0AF7227369,4AD9C116A1942D58A714433CA24F087F18036A7E,5CCC3569C67B7F1BB733664D43DF4645F2A4B04D,5DE37A3371AAE7638748EB43C9F1CE66E09D4470,64B43A6198B6C1F97D9ED8929F5A8913C3815935,6FBD65C22C2996B2038A090BF5E55AA7AEDEE120,7226BE09B7A81000BBF7D959E360B2FE41CCC639,7B7C7F31205D7AEB5DFFEDA08E00282A78CD76E0,7ED3D8AFAC750F8CC0BDF8C87FE3BCBA2BBE2209,85A3AC041E3FCD796AF5D653953D5E27A56E3719,863FDDA3CA537CE03646B3AEBD3FD1CC6B077FBE,87D73471FDC64BD9CEDF84435D20CA4EB5C36FE8,8839E8FBE28219B85392EEA5A4DBC41D315F4B83,8BE58BA7A28DC6B4F211CE8EE86783B85133488D,8CA736F332937E4FA0F5F48488B823F31883123C,96CFE178A1D12489D9D59A0CAE17FE86F5A3A79F,A016192D0A87FC9354A7523A211BBD9CF859708B,A39721D284AA1ED1AE87AE63523535484AA14FB5,BCDE75725B927738B6FD34EA2D78F4FA77B99848