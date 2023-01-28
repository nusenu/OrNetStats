---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-01-28 20:00 UTC**

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


## ContactInfo: email:abuse-node49 posteo.de url:hydra-family.git (43) {#emailabuse-node49posteode-urlhydra-familygit}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Hydra90a](https://metrics.torproject.org/rs.html#details/21328917A9379E6B8ABCB49A0DBE3AAE885CFC15) | 2022-11-02   | Yes         |                     1 |
| [Hydra91a](https://metrics.torproject.org/rs.html#details/AEC8D545DDEDC0311FA7F9F9A885D674D1F1C2FF) | 2022-07-10   | Yes         |                    53 |
| [Hydra93a](https://metrics.torproject.org/rs.html#details/5D575ADD108DDBBF17E78AD8CB267D6C1F338206) | 2022-09-03   | Yes         |                    53 |
| [Hydra94a](https://metrics.torproject.org/rs.html#details/61866162CCDFE651B0D76AA57ECA90B9CC7C80DD) | 2022-09-03   | Yes         |                    53 |
| [Hydra57a](https://metrics.torproject.org/rs.html#details/0F0F690AF1D32C7C3C72C543836625628887BA85) | 2021-06-05   | Yes         |                    53 |
| [Hydra71a](https://metrics.torproject.org/rs.html#details/9F95C68AACB67E6258EC7A6BA9406C227ABAD3F0) | 2021-09-19   | Yes         |                    53 |
| [Hydra72a](https://metrics.torproject.org/rs.html#details/FB79B2BE707F272FBFE1584F44A3FA5156F7F1CF) | 2021-09-19   | Yes         |                    53 |
| [Hydra73a](https://metrics.torproject.org/rs.html#details/391F278B2B55548B97410ADFBD055D079D798E04) | 2021-09-19   | Yes         |                    53 |
| [Hydra24a](https://metrics.torproject.org/rs.html#details/8F293A6484A0973167B15C4997AB9F24C21143FE) | 2020-11-11   | Yes         |                    53 |
| [Hydra69a](https://metrics.torproject.org/rs.html#details/7B3535760987464C8B5686F203B6EBE767C0873E) | 2021-09-09   | Yes         |                    53 |
| [Hydra70a](https://metrics.torproject.org/rs.html#details/DCCBB9717CD8B1F031B9A38C721D2BD9615697AA) | 2021-09-09   | Yes         |                    53 |
| [Hydra52a](https://metrics.torproject.org/rs.html#details/9BF600D6C06A3FBE28216C58CD241A89931CBE7D) | 2021-03-14   | Yes         |                    53 |
| [Hydra51a](https://metrics.torproject.org/rs.html#details/3E610CDAB3B6993E5C31CC99CB10ED8E9CC6F612) | 2022-11-01   | Yes         |                     1 |
| [Hydra45](https://metrics.torproject.org/rs.html#details/01CFCC2545234EEE523D33ED25EF1E79807A18A7)  | 2021-03-04   | No          |                    53 |
| [Hydra82](https://metrics.torproject.org/rs.html#details/10A73078D3D71D01C4B007ED75AB27134E50F1D1)  | 2022-02-08   | No          |                    53 |
| [Hydra55](https://metrics.torproject.org/rs.html#details/378AD3D089A01EC802F165A936122B60B5B1035E)  | 2021-06-06   | No          |                    53 |
| [Hydra38](https://metrics.torproject.org/rs.html#details/3E596EDACBE91DCA3E7F26F0168C7648822D2A02)  | 2021-02-02   | No          |                    53 |
| [Hydra28](https://metrics.torproject.org/rs.html#details/427956E3F23EEBA31954CB0942AEA0ECD43A004A)  | 2020-11-20   | No          |                    53 |
| [Hydra80](https://metrics.torproject.org/rs.html#details/43BB145A8B0909EC542734EA2303D4EFBAD97E09)  | 2022-02-08   | No          |                    53 |
| [Hydra59](https://metrics.torproject.org/rs.html#details/47FC19DBE2B42BB481C65191276670B3D589F075)  | 2021-04-09   | No          |                    53 |
| [Hydra10](https://metrics.torproject.org/rs.html#details/4F68F1B23FCED9D17852FFFDE21637C284BCF107)  | 2020-12-05   | No          |                    53 |
| [Hydra37](https://metrics.torproject.org/rs.html#details/5058E7136283B4CE13F1897871F931CC41F41CC9)  | 2021-03-04   | No          |                    53 |
| [Hydra58](https://metrics.torproject.org/rs.html#details/512F27DD9A2937A8E3D65EDA13A88AE9483E9ACA)  | 2021-04-09   | No          |                    53 |
| [Hydra83](https://metrics.torproject.org/rs.html#details/590F6EDBA063ABACB08391CA3D7A2EC35FD20235)  | 2022-02-08   | No          |                    53 |
| [Hydra36](https://metrics.torproject.org/rs.html#details/5ACC59F3117F1F6FAD8C89F469823CB48BDB5D2F)  | 2021-03-04   | No          |                    53 |
| [Hydra43](https://metrics.torproject.org/rs.html#details/5D5DDFF29B96CC566AA746636868EB07F97DE60C)  | 2021-03-04   | No          |                    53 |
| [Hydra79](https://metrics.torproject.org/rs.html#details/630F75D5AD741889C1BC46DC354A6320152A7B32)  | 2022-02-08   | No          |                    53 |
| [Hydra75](https://metrics.torproject.org/rs.html#details/63928D370B929EBDA54EF2ABDD4A63082085BF61)  | 2021-09-22   | No          |                    53 |
| [Hydra25](https://metrics.torproject.org/rs.html#details/6CB18098F50819DEAB22E369EC3A5661A552A66C)  | 2020-11-20   | No          |                    53 |
| [Hydra81](https://metrics.torproject.org/rs.html#details/76CEF92770EB9D1BBA8025EE4E1751A420B00878)  | 2022-02-08   | No          |                    53 |
| [Hydra89](https://metrics.torproject.org/rs.html#details/900F54B1D483A668959E976F37E327C1122EC817)  | 2022-04-08   | No          |                    53 |
| [Hydra27](https://metrics.torproject.org/rs.html#details/A0A91967046F7A9BC3154C7B3C3FDE34C02B1017)  | 2020-11-20   | No          |                    53 |
| [Hydra65](https://metrics.torproject.org/rs.html#details/A62D8F7772A6C76DD07F431810CE68682DCDD2DC)  | 2021-09-09   | No          |                    53 |
| [Hydra40](https://metrics.torproject.org/rs.html#details/B12536F2F1BBFE0B47FAAD0D5D05BFAEC6C2DE9F)  | 2021-02-02   | No          |                    53 |
| [Hydra86](https://metrics.torproject.org/rs.html#details/BA77149B4EDA76543698F05104F5C2547E306D77)  | 2022-02-21   | No          |                    53 |
| [Hydra85](https://metrics.torproject.org/rs.html#details/BB000558F10C1D760D9C8C5655AA34DAA3869CAF)  | 2022-02-08   | No          |                    53 |
| [Hydra44](https://metrics.torproject.org/rs.html#details/BD140758135A15605996CCEE3BBFA4127F97B233)  | 2021-03-04   | No          |                    53 |
| [Hydra42](https://metrics.torproject.org/rs.html#details/C312C485A7E5595D917E1925BA15D550FB71A6F3)  | 2021-03-04   | No          |                    53 |
| [Hydra66](https://metrics.torproject.org/rs.html#details/C85B30A8356E826418CB901254B7595FE1430619)  | 2021-09-09   | No          |                    53 |
| [Hydra9](https://metrics.torproject.org/rs.html#details/CB28925DA61069A43584030D2610471F1FFD4100)   | 2019-02-10   | No          |                    53 |
| [Hydra39](https://metrics.torproject.org/rs.html#details/E27D3C0FB1E0049BE15B9B53D02905F41B0C0422)  | 2021-02-02   | No          |                    53 |
| [Hydra41](https://metrics.torproject.org/rs.html#details/EFE8849D10519AB1750E1AF47410059522800D32)  | 2021-03-04   | No          |                    53 |
| [Hydra84](https://metrics.torproject.org/rs.html#details/F2657F6A17BE608FD94F565BC45648313D617B63)  | 2022-02-08   | No          |                    53 |

## ContactInfo: email:sysop openinternet.io offlinemasterkey:y ci (7) {#emailsysopopeninternetio-offlinemasterkeyy-ci}

| Nickname                                                                                                     | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [UkranianStrong](https://metrics.torproject.org/rs.html#details/CE30CE396D62B6BC9DEFC8344DA89BFD60083665)    | 2022-07-25   | Yes         |                     2 |
| [OpenInternet](https://metrics.torproject.org/rs.html#details/F37191452612F22EFB6F6204C75A45BF0B11B366)      | 2022-11-22   | Yes         |                     2 |
| [AltAddress02](https://metrics.torproject.org/rs.html#details/5191E3F9A8B9B0C8F356FF0A7D0DA30D95652116)      | 2022-11-26   | Yes         |                     5 |
| [AltAddress01](https://metrics.torproject.org/rs.html#details/80CA806137BF939FBADF38B106A7BBF631FE0F76)      | 2022-11-26   | Yes         |                     5 |
| [Iter](https://metrics.torproject.org/rs.html#details/F3689448309B46A9B7A6612C54C205BAF0971E37)              | 2022-07-22   | Yes         |                     6 |
| [UkranianStrong2](https://metrics.torproject.org/rs.html#details/655F75D0A03DF94298A8BAB663C60FB25D501760)   | 2022-12-01   | Yes         |                     5 |
| [BeCarefulOutThere](https://metrics.torproject.org/rs.html#details/51BD25EE06C46E4466427D4ABF94F2964514EB2F) | 2020-09-10   | No          |                     5 |

## ContactInfo: &lt;nobody AT example dot com&gt; (2) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

0F0F690AF1D32C7C3C72C543836625628887BA85,21328917A9379E6B8ABCB49A0DBE3AAE885CFC15,391F278B2B55548B97410ADFBD055D079D798E04,3E610CDAB3B6993E5C31CC99CB10ED8E9CC6F612,5D575ADD108DDBBF17E78AD8CB267D6C1F338206,61866162CCDFE651B0D76AA57ECA90B9CC7C80DD,7B3535760987464C8B5686F203B6EBE767C0873E,8F293A6484A0973167B15C4997AB9F24C21143FE,9BF600D6C06A3FBE28216C58CD241A89931CBE7D,9F95C68AACB67E6258EC7A6BA9406C227ABAD3F0,AEC8D545DDEDC0311FA7F9F9A885D674D1F1C2FF,DCCBB9717CD8B1F031B9A38C721D2BD9615697AA,FB79B2BE707F272FBFE1584F44A3FA5156F7F1CF,5191E3F9A8B9B0C8F356FF0A7D0DA30D95652116,655F75D0A03DF94298A8BAB663C60FB25D501760,80CA806137BF939FBADF38B106A7BBF631FE0F76,CE30CE396D62B6BC9DEFC8344DA89BFD60083665,F3689448309B46A9B7A6612C54C205BAF0971E37,F37191452612F22EFB6F6204C75A45BF0B11B366,A9A4213EA3D707857368C683F2208C83B8755D8A