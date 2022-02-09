---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-02-09 17:00 UTC**

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


## ContactInfo: email:abuse-node49 posteo.de url:hydra-family.git (85) {#emailabuse-node49posteode-urlhydra-familygit}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Hydra6](https://metrics.torproject.org/rs.html#details/1050FC79C5F1103B185300EF72DDF5B4EDC683C9)  | 2020-12-05   | Yes         |                    79 |
| [Hydra57](https://metrics.torproject.org/rs.html#details/0F0F690AF1D32C7C3C72C543836625628887BA85) | 2021-06-05   | Yes         |                    79 |
| [Hydra69](https://metrics.torproject.org/rs.html#details/7B3535760987464C8B5686F203B6EBE767C0873E) | 2021-09-09   | Yes         |                    79 |
| [Hydra24](https://metrics.torproject.org/rs.html#details/8F293A6484A0973167B15C4997AB9F24C21143FE) | 2020-11-11   | Yes         |                    79 |
| [Hydra23](https://metrics.torproject.org/rs.html#details/F7ED4158B7114617E8F737C65DBE87EE6B83445B) | 2020-11-11   | Yes         |                    79 |
| [Hydra70](https://metrics.torproject.org/rs.html#details/DCCBB9717CD8B1F031B9A38C721D2BD9615697AA) | 2021-09-09   | Yes         |                    79 |
| [Hydra71](https://metrics.torproject.org/rs.html#details/9F95C68AACB67E6258EC7A6BA9406C227ABAD3F0) | 2021-09-19   | Yes         |                    79 |
| [Hydra72](https://metrics.torproject.org/rs.html#details/FB79B2BE707F272FBFE1584F44A3FA5156F7F1CF) | 2021-09-19   | Yes         |                    79 |
| [Hydra22](https://metrics.torproject.org/rs.html#details/BD33EF180B1118B00BDF073E2771210E3BDDD8CD) | 2020-11-11   | Yes         |                    79 |
| [Hydra50](https://metrics.torproject.org/rs.html#details/4443A8D51422427AD26E0CE3FA3447B1B76F520A) | 2021-04-18   | Yes         |                    79 |
| [Hydra61](https://metrics.torproject.org/rs.html#details/7DFDF0314F9CF461F537C3069E820F99FC5AF055) | 2021-06-05   | Yes         |                    79 |
| [Hydra56](https://metrics.torproject.org/rs.html#details/C5509FCCEF72AC828382877ECE930119C5FAD625) | 2021-06-05   | Yes         |                    79 |
| [Hydra49](https://metrics.torproject.org/rs.html#details/1042FAC7C8048ACD9EAB365CF68B3F7C4350738A) | 2021-06-05   | Yes         |                    79 |
| [Hydra73](https://metrics.torproject.org/rs.html#details/391F278B2B55548B97410ADFBD055D079D798E04) | 2021-09-19   | Yes         |                    79 |
| [Hydra48](https://metrics.torproject.org/rs.html#details/387CFC0B90EACFFE4A80CD8AA057F364E9D1D573) | 2021-06-05   | Yes         |                    79 |
| [Hydra60](https://metrics.torproject.org/rs.html#details/DFA93C5829CF723CFF266E45B4ECA482F8D67E25) | 2021-06-05   | Yes         |                    79 |
| [Hydra68](https://metrics.torproject.org/rs.html#details/8C188E7122693566683807363B576D99C0B17386) | 2021-09-09   | Yes         |                    79 |
| [Hydra74](https://metrics.torproject.org/rs.html#details/C831CFEBA2407EF49D916F6890F7B9367AA8B49A) | 2021-09-19   | Yes         |                    79 |
| [Hydra67](https://metrics.torproject.org/rs.html#details/5A0643E452E143BE549BAB3BFE575F40DDBD527C) | 2021-09-09   | Yes         |                    79 |
| [Hydra52](https://metrics.torproject.org/rs.html#details/9BF600D6C06A3FBE28216C58CD241A89931CBE7D) | 2021-03-14   | Yes         |                    79 |
| [Hydra45](https://metrics.torproject.org/rs.html#details/01CFCC2545234EEE523D33ED25EF1E79807A18A7) | 2021-03-04   | No          |                    79 |
| [Hydra82](https://metrics.torproject.org/rs.html#details/10A73078D3D71D01C4B007ED75AB27134E50F1D1) | 2022-02-08   | No          |                     7 |
| [Hydra26](https://metrics.torproject.org/rs.html#details/1940398159C3C571939363DDE8044F3DB8B97394) | 2020-11-20   | No          |                    79 |
| [Hydra16](https://metrics.torproject.org/rs.html#details/1DFE397493D0791DE63F2D6EA5AB6EBCB7B9871A) | 2020-06-09   | No          |                    79 |
| [Hydra30](https://metrics.torproject.org/rs.html#details/22C1314867920DA37001DAD1A63F1D5CABF9DB11) | 2020-12-02   | No          |                    79 |
| [Hydra3](https://metrics.torproject.org/rs.html#details/27D02579AD5F3E32895D99C38E482D1DC6CBAE5E)  | 2019-10-17   | No          |                    79 |
| [Hydra29](https://metrics.torproject.org/rs.html#details/2DEF8010770472367EB2089CA0A50A17B211E78A) | 2020-12-02   | No          |                    79 |
| [Hydra62](https://metrics.torproject.org/rs.html#details/2FE81C1FD45AC593193F04DF781980257E4BCD03) | 2021-06-24   | No          |                    79 |
| [Hydra53](https://metrics.torproject.org/rs.html#details/3383377B522204E69B1FA1A5627F95AF640E9108) | 2021-06-24   | No          |                    79 |
| [Hydra55](https://metrics.torproject.org/rs.html#details/378AD3D089A01EC802F165A936122B60B5B1035E) | 2021-06-06   | No          |                    79 |
| [Hydra13](https://metrics.torproject.org/rs.html#details/39C37AFC908D12BB79B34EB6298929BC51C2E651) | 2020-12-03   | No          |                    79 |
| [Hydra18](https://metrics.torproject.org/rs.html#details/3AD29FE1241B73595F99BA2C6D830AF0B6874043) | 2020-06-30   | No          |                    79 |
| [Hydra5](https://metrics.torproject.org/rs.html#details/3C90CA5857705D7C6C176D475C592AF2789FDDA7)  | 2021-01-08   | No          |                    79 |
| [Hydra38](https://metrics.torproject.org/rs.html#details/3E596EDACBE91DCA3E7F26F0168C7648822D2A02) | 2021-02-02   | No          |                    79 |
| [Hydra46](https://metrics.torproject.org/rs.html#details/3F14EF80BCA7D3679491EB37C98ECFB786F644AE) | 2021-03-06   | No          |                    79 |
| [Hydra28](https://metrics.torproject.org/rs.html#details/427956E3F23EEBA31954CB0942AEA0ECD43A004A) | 2020-11-20   | No          |                    79 |
| [Hydra80](https://metrics.torproject.org/rs.html#details/43BB145A8B0909EC542734EA2303D4EFBAD97E09) | 2022-02-08   | No          |                     7 |
| [Hydra14](https://metrics.torproject.org/rs.html#details/43ED841926B5DA9487032D789A31B5E74A7525E2) | 2021-01-08   | No          |                    79 |
| [Hydra59](https://metrics.torproject.org/rs.html#details/47FC19DBE2B42BB481C65191276670B3D589F075) | 2021-04-09   | No          |                    79 |
| [Hydra15](https://metrics.torproject.org/rs.html#details/4BA3C12B073B7E3F7977C46AF3638685BB89493F) | 2020-12-02   | No          |                    79 |
| [Hydra10](https://metrics.torproject.org/rs.html#details/4F68F1B23FCED9D17852FFFDE21637C284BCF107) | 2020-12-05   | No          |                    79 |
| [Hydra37](https://metrics.torproject.org/rs.html#details/5058E7136283B4CE13F1897871F931CC41F41CC9) | 2021-03-04   | No          |                    79 |
| [Hydra58](https://metrics.torproject.org/rs.html#details/512F27DD9A2937A8E3D65EDA13A88AE9483E9ACA) | 2021-04-09   | No          |                    79 |
| [Hydra83](https://metrics.torproject.org/rs.html#details/590F6EDBA063ABACB08391CA3D7A2EC35FD20235) | 2022-02-08   | No          |                     7 |
| [Hydra36](https://metrics.torproject.org/rs.html#details/5ACC59F3117F1F6FAD8C89F469823CB48BDB5D2F) | 2021-03-04   | No          |                    79 |
| [Hydra21](https://metrics.torproject.org/rs.html#details/5B7C577DDEBC6B2C39B55364F4EAD69FE8181067) | 2020-10-05   | No          |                    79 |
| [Hydra43](https://metrics.torproject.org/rs.html#details/5D5DDFF29B96CC566AA746636868EB07F97DE60C) | 2021-03-04   | No          |                    79 |
| [Hydra12](https://metrics.torproject.org/rs.html#details/62133EDB663C1C043B2A2DC24A19C351088EBD5C) | 2021-01-11   | No          |                    79 |
| [Hydra79](https://metrics.torproject.org/rs.html#details/630F75D5AD741889C1BC46DC354A6320152A7B32) | 2022-02-08   | No          |                     7 |
| [Hydra75](https://metrics.torproject.org/rs.html#details/63928D370B929EBDA54EF2ABDD4A63082085BF61) | 2021-09-22   | No          |                    79 |
| [Hydra4](https://metrics.torproject.org/rs.html#details/6C0E4E223B1C7E4366FFABA33BF033636A867865)  | 2020-12-05   | No          |                    79 |
| [Hydra25](https://metrics.torproject.org/rs.html#details/6CB18098F50819DEAB22E369EC3A5661A552A66C) | 2020-11-20   | No          |                    79 |
| [Hydra35](https://metrics.torproject.org/rs.html#details/7466057426018C41EDFC1465BE7F01E27155CFBF) | 2021-01-02   | No          |                    79 |
| [Hydra81](https://metrics.torproject.org/rs.html#details/76CEF92770EB9D1BBA8025EE4E1751A420B00878) | 2022-02-08   | No          |                     7 |
| [Hydra34](https://metrics.torproject.org/rs.html#details/7B972FDF84026AC52E41461F05DDBBE3A07598AF) | 2021-01-02   | No          |                    79 |
| [Hydra54](https://metrics.torproject.org/rs.html#details/7E3230B8275047F7737E03314D86FEBC4F5778B6) | 2021-06-05   | No          |                    79 |
| [Hydra20](https://metrics.torproject.org/rs.html#details/86E479266EBB982E204009532ED460628689E5B5) | 2020-10-07   | No          |                    79 |
| [Hydra32](https://metrics.torproject.org/rs.html#details/8D1117EFBC91270AE1FCE55E21F9D250985AFAB3) | 2020-12-29   | No          |                    79 |
| [Hydra47](https://metrics.torproject.org/rs.html#details/9CD386BB804FB9BEE92FA11E60E9241555CCB79A) | 2021-03-06   | No          |                    79 |
| [Hydra27](https://metrics.torproject.org/rs.html#details/A0A91967046F7A9BC3154C7B3C3FDE34C02B1017) | 2020-11-20   | No          |                    79 |
| [Hydra77](https://metrics.torproject.org/rs.html#details/A54BF50C574AEEFE0EE3E7D3B2B0F1FAA695414A) | 2021-11-30   | No          |                    79 |
| [Hydra65](https://metrics.torproject.org/rs.html#details/A62D8F7772A6C76DD07F431810CE68682DCDD2DC) | 2021-09-09   | No          |                    79 |
| [Hydra31](https://metrics.torproject.org/rs.html#details/AF3511FA8B418C756BDBA97A6EDE970D1F74F27E) | 2020-12-29   | No          |                    79 |
| [Hydra40](https://metrics.torproject.org/rs.html#details/B12536F2F1BBFE0B47FAAD0D5D05BFAEC6C2DE9F) | 2021-02-02   | No          |                    79 |
| [Hydra2](https://metrics.torproject.org/rs.html#details/B3D84B209451D608A81F5E87189CE79E3DFA87BA)  | 2021-01-06   | No          |                    79 |
| [Hydra85](https://metrics.torproject.org/rs.html#details/BB000558F10C1D760D9C8C5655AA34DAA3869CAF) | 2022-02-08   | No          |                     7 |
| [Hydra44](https://metrics.torproject.org/rs.html#details/BD140758135A15605996CCEE3BBFA4127F97B233) | 2021-03-04   | No          |                    79 |
| [Hydra0](https://metrics.torproject.org/rs.html#details/C246FD9DF1C39730AA64E314CA5AA49CCE08871D)  | 2021-11-30   | No          |                    79 |
| [Hydra42](https://metrics.torproject.org/rs.html#details/C312C485A7E5595D917E1925BA15D550FB71A6F3) | 2021-03-04   | No          |                    79 |
| [Hydra33](https://metrics.torproject.org/rs.html#details/C673AFE5CF9CC49E5F864F0F80D5FE2814A52233) | 2020-12-29   | No          |                    79 |
| [Hydra66](https://metrics.torproject.org/rs.html#details/C85B30A8356E826418CB901254B7595FE1430619) | 2021-09-09   | No          |                    79 |
| [Hydra9](https://metrics.torproject.org/rs.html#details/CB28925DA61069A43584030D2610471F1FFD4100)  | 2019-02-10   | No          |                    79 |
| [Hydra63](https://metrics.torproject.org/rs.html#details/CBFEF90E7A304E9515A044C61C4117CD9766050B) | 2021-06-24   | No          |                    79 |
| [Hydra11](https://metrics.torproject.org/rs.html#details/D9D2DBEAC776215B33E99D4EBFFE8FBA5C100DB7) | 2021-01-13   | No          |                    79 |
| [Hydra7](https://metrics.torproject.org/rs.html#details/E001D2724CEA5615E828D30111B866AB277E86C2)  | 2021-01-08   | No          |                    79 |
| [Hydra8](https://metrics.torproject.org/rs.html#details/E1D2328D0DB2A06EE85ABD9D8D75CC5DBDDFDA5C)  | 2021-01-08   | No          |                    79 |
| [Hydra39](https://metrics.torproject.org/rs.html#details/E27D3C0FB1E0049BE15B9B53D02905F41B0C0422) | 2021-02-02   | No          |                    79 |
| [Hydra17](https://metrics.torproject.org/rs.html#details/E3DAF067B028450B31CF5CE118F2F9AC53146ABD) | 2020-06-09   | No          |                    79 |
| [Hydra19](https://metrics.torproject.org/rs.html#details/E465AD166798A3CD0A4866FA2A8BB5ADD157FBD5) | 2020-06-30   | No          |                    79 |
| [Hydra76](https://metrics.torproject.org/rs.html#details/E685733A4A2F184AB320846094651806A62627B5) | 2021-09-27   | No          |                    79 |
| [Hydra78](https://metrics.torproject.org/rs.html#details/ED0C39728C0410A1A6173FE0F8C1C9667DDF7D66) | 2021-11-30   | No          |                    79 |
| [Hydra41](https://metrics.torproject.org/rs.html#details/EFE8849D10519AB1750E1AF47410059522800D32) | 2021-03-04   | No          |                    79 |
| [Hydra84](https://metrics.torproject.org/rs.html#details/F2657F6A17BE608FD94F565BC45648313D617B63) | 2022-02-08   | No          |                     7 |
| [Hydra64](https://metrics.torproject.org/rs.html#details/F2DCADFB285DBAD7218E0EFA0598715DBAA8C18D) | 2021-06-27   | No          |                    79 |
| [Hydra1](https://metrics.torproject.org/rs.html#details/FF7C2604EFEE8B5898FDE1145A4CA35C8E5E5607)  | 2021-01-13   | No          |                    79 |

## ContactInfo: tor at xtom dot com (6) {#toratxtomdotcom}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [XTOMLON](https://metrics.torproject.org/rs.html#details/5ABC7AAFA86CA890242DE79582125B18C3B0E541)     | 2021-12-03   | Yes         |                     1 |
| [XTOMAMS](https://metrics.torproject.org/rs.html#details/A41A8317A5BD4DD10BE9925277DB332395F50F17)     | 2021-12-07   | Yes         |                     1 |
| [XTOMDUS](https://metrics.torproject.org/rs.html#details/955F15325D6F3E3350EA8A70EB5C49C5BF95C5A0)     | 2021-12-03   | Yes         |                     1 |
| [XTOMFRA](https://metrics.torproject.org/rs.html#details/AB12F88E52C439769EDB592B89AA36D8AF5A1C0C)     | 2021-12-07   | Yes         |                     1 |
| [XTOMSJC](https://metrics.torproject.org/rs.html#details/280F26E75C5ED7C292DD5AC5A9695C47B7784DC8)     | 2021-12-09   | Yes         |                     1 |
| [XTOMLONEXIT](https://metrics.torproject.org/rs.html#details/9331E29298E40EB28A01C780E73954CD73237F50) | 2022-02-03   | No          |                     1 |

## ContactInfo: ContactInfo email:abuse stormycloud.org url:storm (24) {#contactinfo-emailabusestormycloudorg-urlstorm}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/A7348BE96DF5BD080A9BA6F87454706BFD75371A) | 2021-12-09   | Yes         |                    22 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/4E6515A5E941C1C5517FB2952972BEB458640BCF) | 2021-12-09   | Yes         |                    22 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/00B211F85E145B50890633CA9CB6B18262E51CD7) | 2022-01-24   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/037A9B1EF680151D1977B52CFFA948819B2F867A) | 2022-01-23   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/0A5EE342140AF65850A0D1CCEF0ECB3223AFA24F) | 2022-02-09   | No          |                    21 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/166443CA1BE8020A9479B117E7ADB061CF8F7852) | 2022-01-25   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/2BC1779CF325C5E4A6C0A5F958E458ED104CCEA7) | 2022-01-25   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/3AD93704B1EFFA79F2BF09CAB7ADCC334D0BEF7A) | 2022-01-24   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/3EF489E1F8EDA383286769CBF90E3CB18B0F71CF) | 2022-01-24   | No          |                    24 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/4B0BC0CD47B93EB98CB2D624C634143F5BD62BF6) | 2022-02-09   | No          |                    21 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/6EA904BE17DB5CF37EB9416ECB73C24A7FED057E) | 2022-01-23   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/76B3B62839BC59822FC09C0E80435DD0524083D3) | 2022-01-24   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/7E7737831BEEB5EE423F37E127112F1E3C5419CF) | 2022-01-24   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/85422BC1612840FA70EB70ECCD9F66D0D397719B) | 2022-01-25   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/8F32C089CD71D6FB1012FD6EC1EC0438A57F32C5) | 2022-01-25   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/8FFA62DEB796D18DA8CAA9A95E0B1F60CDDDCB50) | 2022-01-23   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/A00FAA3F0F84F8B118D337660FF0AA4E3E32AE5A) | 2022-01-25   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/A88CE4546B3165A03E4099260B93294BE750532A) | 2022-01-25   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/BC7ACE7298DF5BC8FFCEA4CF0CB88C97902E4582) | 2022-01-25   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/D8773C1BAA890CDEF3B48B5EC5B6AA610735DCAB) | 2022-01-25   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/DDE988A745422A4BBFF0C1ABFD1777D74BFBC40E) | 2022-01-23   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/EDD507B5CAAAABFB0F343CF621A202F93CB57CE4) | 2022-01-23   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/EFF54875CFED77DDB6260A1A4AD2B0608E3807A1) | 2022-01-24   | No          |                    27 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/F8BDA076BAA2452B7CD885B58863D956883605D6) | 2022-01-25   | No          |                    27 |


## Fingerprint List of Guard-only Relays in E2E Groups

0F0F690AF1D32C7C3C72C543836625628887BA85,1042FAC7C8048ACD9EAB365CF68B3F7C4350738A,1050FC79C5F1103B185300EF72DDF5B4EDC683C9,387CFC0B90EACFFE4A80CD8AA057F364E9D1D573,391F278B2B55548B97410ADFBD055D079D798E04,4443A8D51422427AD26E0CE3FA3447B1B76F520A,5A0643E452E143BE549BAB3BFE575F40DDBD527C,7B3535760987464C8B5686F203B6EBE767C0873E,7DFDF0314F9CF461F537C3069E820F99FC5AF055,8C188E7122693566683807363B576D99C0B17386,8F293A6484A0973167B15C4997AB9F24C21143FE,9BF600D6C06A3FBE28216C58CD241A89931CBE7D,9F95C68AACB67E6258EC7A6BA9406C227ABAD3F0,BD33EF180B1118B00BDF073E2771210E3BDDD8CD,C5509FCCEF72AC828382877ECE930119C5FAD625,C831CFEBA2407EF49D916F6890F7B9367AA8B49A,280F26E75C5ED7C292DD5AC5A9695C47B7784DC8,5ABC7AAFA86CA890242DE79582125B18C3B0E541,955F15325D6F3E3350EA8A70EB5C49C5BF95C5A0,A41A8317A5BD4DD10BE9925277DB332395F50F17,AB12F88E52C439769EDB592B89AA36D8AF5A1C0C,4E6515A5E941C1C5517FB2952972BEB458640BCF,A7348BE96DF5BD080A9BA6F87454706BFD75371A,DCCBB9717CD8B1F031B9A38C721D2BD9615697AA,DFA93C5829CF723CFF266E45B4ECA482F8D67E25,F7ED4158B7114617E8F737C65DBE87EE6B83445B,FB79B2BE707F272FBFE1584F44A3FA5156F7F1CF