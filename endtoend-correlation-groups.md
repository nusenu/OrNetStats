---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-11-15 16:00 UTC**

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


## ContactInfo: email:abuse-node49 posteo.de url:hydra-family.git (63) {#emailabuse-node49posteode-urlhydra-familygit}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Hydra71a](https://metrics.torproject.org/rs.html#details/9F95C68AACB67E6258EC7A6BA9406C227ABAD3F0) | 2021-09-19   | Yes         |                    80 |
| [Hydra73a](https://metrics.torproject.org/rs.html#details/391F278B2B55548B97410ADFBD055D079D798E04) | 2021-09-19   | Yes         |                    80 |
| [Hydra72a](https://metrics.torproject.org/rs.html#details/FB79B2BE707F272FBFE1584F44A3FA5156F7F1CF) | 2021-09-19   | Yes         |                    80 |
| [Hydra57a](https://metrics.torproject.org/rs.html#details/0F0F690AF1D32C7C3C72C543836625628887BA85) | 2021-06-05   | Yes         |                    80 |
| [Hydra52a](https://metrics.torproject.org/rs.html#details/9BF600D6C06A3FBE28216C58CD241A89931CBE7D) | 2021-03-14   | Yes         |                    80 |
| [Hydra51a](https://metrics.torproject.org/rs.html#details/3E610CDAB3B6993E5C31CC99CB10ED8E9CC6F612) | 2022-11-01   | Yes         |                     1 |
| [Hydra45](https://metrics.torproject.org/rs.html#details/01CFCC2545234EEE523D33ED25EF1E79807A18A7)  | 2021-03-04   | No          |                    80 |
| [Hydra82](https://metrics.torproject.org/rs.html#details/10A73078D3D71D01C4B007ED75AB27134E50F1D1)  | 2022-02-08   | No          |                    80 |
| [Hydra30](https://metrics.torproject.org/rs.html#details/22C1314867920DA37001DAD1A63F1D5CABF9DB11)  | 2020-12-02   | No          |                    80 |
| [Hydra3](https://metrics.torproject.org/rs.html#details/27D02579AD5F3E32895D99C38E482D1DC6CBAE5E)   | 2019-10-17   | No          |                    80 |
| [Hydra29](https://metrics.torproject.org/rs.html#details/2DEF8010770472367EB2089CA0A50A17B211E78A)  | 2020-12-02   | No          |                    80 |
| [Hydra62](https://metrics.torproject.org/rs.html#details/2FE81C1FD45AC593193F04DF781980257E4BCD03)  | 2021-06-24   | No          |                    80 |
| [Hydra53](https://metrics.torproject.org/rs.html#details/3383377B522204E69B1FA1A5627F95AF640E9108)  | 2021-06-24   | No          |                    80 |
| [Hydra55](https://metrics.torproject.org/rs.html#details/378AD3D089A01EC802F165A936122B60B5B1035E)  | 2021-06-06   | No          |                    80 |
| [Hydra13](https://metrics.torproject.org/rs.html#details/39C37AFC908D12BB79B34EB6298929BC51C2E651)  | 2020-12-03   | No          |                    80 |
| [Hydra5](https://metrics.torproject.org/rs.html#details/3C90CA5857705D7C6C176D475C592AF2789FDDA7)   | 2021-01-08   | No          |                    80 |
| [Hydra38](https://metrics.torproject.org/rs.html#details/3E596EDACBE91DCA3E7F26F0168C7648822D2A02)  | 2021-02-02   | No          |                    80 |
| [Hydra28](https://metrics.torproject.org/rs.html#details/427956E3F23EEBA31954CB0942AEA0ECD43A004A)  | 2020-11-20   | No          |                    80 |
| [Hydra80](https://metrics.torproject.org/rs.html#details/43BB145A8B0909EC542734EA2303D4EFBAD97E09)  | 2022-02-08   | No          |                    80 |
| [Hydra14](https://metrics.torproject.org/rs.html#details/43ED841926B5DA9487032D789A31B5E74A7525E2)  | 2021-01-08   | No          |                    80 |
| [Hydra59](https://metrics.torproject.org/rs.html#details/47FC19DBE2B42BB481C65191276670B3D589F075)  | 2021-04-09   | No          |                    80 |
| [Hydra15](https://metrics.torproject.org/rs.html#details/4BA3C12B073B7E3F7977C46AF3638685BB89493F)  | 2020-12-02   | No          |                    80 |
| [Hydra10](https://metrics.torproject.org/rs.html#details/4F68F1B23FCED9D17852FFFDE21637C284BCF107)  | 2020-12-05   | No          |                    80 |
| [Hydra37](https://metrics.torproject.org/rs.html#details/5058E7136283B4CE13F1897871F931CC41F41CC9)  | 2021-03-04   | No          |                    80 |
| [Hydra58](https://metrics.torproject.org/rs.html#details/512F27DD9A2937A8E3D65EDA13A88AE9483E9ACA)  | 2021-04-09   | No          |                    80 |
| [Hydra83](https://metrics.torproject.org/rs.html#details/590F6EDBA063ABACB08391CA3D7A2EC35FD20235)  | 2022-02-08   | No          |                    80 |
| [Hydra36](https://metrics.torproject.org/rs.html#details/5ACC59F3117F1F6FAD8C89F469823CB48BDB5D2F)  | 2021-03-04   | No          |                    80 |
| [Hydra43](https://metrics.torproject.org/rs.html#details/5D5DDFF29B96CC566AA746636868EB07F97DE60C)  | 2021-03-04   | No          |                    80 |
| [Hydra12](https://metrics.torproject.org/rs.html#details/62133EDB663C1C043B2A2DC24A19C351088EBD5C)  | 2021-01-11   | No          |                    80 |
| [Hydra79](https://metrics.torproject.org/rs.html#details/630F75D5AD741889C1BC46DC354A6320152A7B32)  | 2022-02-08   | No          |                    80 |
| [Hydra75](https://metrics.torproject.org/rs.html#details/63928D370B929EBDA54EF2ABDD4A63082085BF61)  | 2021-09-22   | No          |                    80 |
| [Hydra4](https://metrics.torproject.org/rs.html#details/6C0E4E223B1C7E4366FFABA33BF033636A867865)   | 2020-12-05   | No          |                    80 |
| [Hydra25](https://metrics.torproject.org/rs.html#details/6CB18098F50819DEAB22E369EC3A5661A552A66C)  | 2020-11-20   | No          |                    80 |
| [Hydra35](https://metrics.torproject.org/rs.html#details/7466057426018C41EDFC1465BE7F01E27155CFBF)  | 2021-01-02   | No          |                    80 |
| [Hydra81](https://metrics.torproject.org/rs.html#details/76CEF92770EB9D1BBA8025EE4E1751A420B00878)  | 2022-02-08   | No          |                    80 |
| [Hydra34](https://metrics.torproject.org/rs.html#details/7B972FDF84026AC52E41461F05DDBBE3A07598AF)  | 2021-01-02   | No          |                    80 |
| [Hydra54](https://metrics.torproject.org/rs.html#details/7E3230B8275047F7737E03314D86FEBC4F5778B6)  | 2021-06-05   | No          |                    80 |
| [Hydra32](https://metrics.torproject.org/rs.html#details/8D1117EFBC91270AE1FCE55E21F9D250985AFAB3)  | 2020-12-29   | No          |                    80 |
| [Hydra89](https://metrics.torproject.org/rs.html#details/900F54B1D483A668959E976F37E327C1122EC817)  | 2022-04-08   | No          |                    80 |
| [Hydra27](https://metrics.torproject.org/rs.html#details/A0A91967046F7A9BC3154C7B3C3FDE34C02B1017)  | 2020-11-20   | No          |                    80 |
| [Hydra77](https://metrics.torproject.org/rs.html#details/A54BF50C574AEEFE0EE3E7D3B2B0F1FAA695414A)  | 2021-11-30   | No          |                    80 |
| [Hydra65](https://metrics.torproject.org/rs.html#details/A62D8F7772A6C76DD07F431810CE68682DCDD2DC)  | 2021-09-09   | No          |                    80 |
| [Hydra31](https://metrics.torproject.org/rs.html#details/AF3511FA8B418C756BDBA97A6EDE970D1F74F27E)  | 2020-12-29   | No          |                    80 |
| [Hydra50](https://metrics.torproject.org/rs.html#details/B00579D1A23F1FFB13A20FD650EA60D367F36506)  | 2022-07-10   | No          |                    80 |
| [Hydra40](https://metrics.torproject.org/rs.html#details/B12536F2F1BBFE0B47FAAD0D5D05BFAEC6C2DE9F)  | 2021-02-02   | No          |                    80 |
| [Hydra2](https://metrics.torproject.org/rs.html#details/B3D84B209451D608A81F5E87189CE79E3DFA87BA)   | 2021-01-06   | No          |                    80 |
| [Hydra86](https://metrics.torproject.org/rs.html#details/BA77149B4EDA76543698F05104F5C2547E306D77)  | 2022-02-21   | No          |                    80 |
| [Hydra85](https://metrics.torproject.org/rs.html#details/BB000558F10C1D760D9C8C5655AA34DAA3869CAF)  | 2022-02-08   | No          |                    80 |
| [Hydra44](https://metrics.torproject.org/rs.html#details/BD140758135A15605996CCEE3BBFA4127F97B233)  | 2021-03-04   | No          |                    80 |
| [Hydra0](https://metrics.torproject.org/rs.html#details/C246FD9DF1C39730AA64E314CA5AA49CCE08871D)   | 2021-11-30   | No          |                    80 |
| [Hydra42](https://metrics.torproject.org/rs.html#details/C312C485A7E5595D917E1925BA15D550FB71A6F3)  | 2021-03-04   | No          |                    80 |
| [Hydra33](https://metrics.torproject.org/rs.html#details/C673AFE5CF9CC49E5F864F0F80D5FE2814A52233)  | 2020-12-29   | No          |                    80 |
| [Hydra66](https://metrics.torproject.org/rs.html#details/C85B30A8356E826418CB901254B7595FE1430619)  | 2021-09-09   | No          |                    80 |
| [Hydra9](https://metrics.torproject.org/rs.html#details/CB28925DA61069A43584030D2610471F1FFD4100)   | 2019-02-10   | No          |                    80 |
| [Hydra63](https://metrics.torproject.org/rs.html#details/CBFEF90E7A304E9515A044C61C4117CD9766050B)  | 2021-06-24   | No          |                    80 |
| [Hydra7](https://metrics.torproject.org/rs.html#details/E001D2724CEA5615E828D30111B866AB277E86C2)   | 2021-01-08   | No          |                    80 |
| [Hydra8](https://metrics.torproject.org/rs.html#details/E1D2328D0DB2A06EE85ABD9D8D75CC5DBDDFDA5C)   | 2021-01-08   | No          |                    80 |
| [Hydra39](https://metrics.torproject.org/rs.html#details/E27D3C0FB1E0049BE15B9B53D02905F41B0C0422)  | 2021-02-02   | No          |                    80 |
| [Hydra76](https://metrics.torproject.org/rs.html#details/E685733A4A2F184AB320846094651806A62627B5)  | 2021-09-27   | No          |                    80 |
| [Hydra78](https://metrics.torproject.org/rs.html#details/ED0C39728C0410A1A6173FE0F8C1C9667DDF7D66)  | 2021-11-30   | No          |                    80 |
| [Hydra41](https://metrics.torproject.org/rs.html#details/EFE8849D10519AB1750E1AF47410059522800D32)  | 2021-03-04   | No          |                    80 |
| [Hydra84](https://metrics.torproject.org/rs.html#details/F2657F6A17BE608FD94F565BC45648313D617B63)  | 2022-02-08   | No          |                    80 |
| [Hydra64](https://metrics.torproject.org/rs.html#details/F2DCADFB285DBAD7218E0EFA0598715DBAA8C18D)  | 2021-06-27   | No          |                    80 |

## ContactInfo: Random Person nobody@tor.org (7) {#random-person-nobodytororg}

| Nickname                                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [imherefortheparty](https://metrics.torproject.org/rs.html#details/3540A4DD39DCF318842B295CDDD49118924F2A57)  | 2022-04-08   | Yes         |                     1 |
| [maddy](https://metrics.torproject.org/rs.html#details/E79404C7477110F73863BC5908F3F1C70990B685)              | 2022-10-08   | Yes         |                     1 |
| [pooclown](https://metrics.torproject.org/rs.html#details/F7BB03BC77CEB6EF66478C58A343028958EB7693)           | 2022-09-20   | Yes         |                     1 |
| [ididnteditheconfig](https://metrics.torproject.org/rs.html#details/80F597A2715438BDD986E6F7AC8646EEA4E492F0) | 2020-10-21   | Yes         |                     1 |
| [ididreadtheconfig](https://metrics.torproject.org/rs.html#details/F96CBFC5C079D839E01902802A70029486D2AD82)  | 2022-08-09   | Yes         |                     1 |
| [ididnteditheconfig](https://metrics.torproject.org/rs.html#details/5EA46A3C23E4A3905DAAE9BD4801142E20AEA780) | 2022-10-05   | No          |                     1 |
| [theglowingones](https://metrics.torproject.org/rs.html#details/E399BF6C6EEB4D63A388911B84C16909CD84A13E)     | 2022-10-13   | No          |                     1 |

## ContactInfo: tor-relay-admin@carlos1001.com (3) {#tor-relay-admincarlos1001com}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [carlos1001](https://metrics.torproject.org/rs.html#details/299CC5D7A58E5B92B69DC333B28D926CD7B157D8)  | 2021-05-12   | Yes         |                     1 |
| [orion01](https://metrics.torproject.org/rs.html#details/0E0AF3656F3F7914752E013C10E7F46C651BA820)     | 2022-11-05   | No          |                     1 |
| [Triangulum1](https://metrics.torproject.org/rs.html#details/7417085A0CC99550CF82ADD3F7B1CD01E64AAADE) | 2022-11-11   | No          |                     1 |

## ContactInfo: cam632@gmx.com (2) {#cam632gmxcom}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Praktiker](https://metrics.torproject.org/rs.html#details/E99A1B54541518A8A6058D75762497AE0D3442DC) | 2022-09-23   | Yes         |                     1 |
| [Boro](https://metrics.torproject.org/rs.html#details/5F4BCBC6E20AE074340D0A743E6F2EA4B51B09C1)      | 2022-08-31   | No          |                     1 |

## ContactInfo: 96001reddit at protonmail dot com (2) {#96001redditatprotonmaildotcom}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [RelaysOfBabylon](https://metrics.torproject.org/rs.html#details/0C29BDA07390E89AC6DA4775FB102A1B8183F6C2) | 2022-09-20   | Yes         |                     1 |
| [imboredrelay](https://metrics.torproject.org/rs.html#details/654B364C24573B4631C8AD7C39C161C568C04A3C)    | 2022-09-14   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

0F0F690AF1D32C7C3C72C543836625628887BA85,391F278B2B55548B97410ADFBD055D079D798E04,3E610CDAB3B6993E5C31CC99CB10ED8E9CC6F612,9BF600D6C06A3FBE28216C58CD241A89931CBE7D,9F95C68AACB67E6258EC7A6BA9406C227ABAD3F0,FB79B2BE707F272FBFE1584F44A3FA5156F7F1CF,3540A4DD39DCF318842B295CDDD49118924F2A57,80F597A2715438BDD986E6F7AC8646EEA4E492F0,E79404C7477110F73863BC5908F3F1C70990B685,F7BB03BC77CEB6EF66478C58A343028958EB7693,F96CBFC5C079D839E01902802A70029486D2AD82,299CC5D7A58E5B92B69DC333B28D926CD7B157D8,E99A1B54541518A8A6058D75762497AE0D3442DC,0C29BDA07390E89AC6DA4775FB102A1B8183F6C2