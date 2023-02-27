---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-02-27 17:00 UTC**

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


## ContactInfo: email:abuse-node49 posteo.de url:hydra-family.git (28) {#emailabuse-node49posteode-urlhydra-familygit}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Hydra93a](https://metrics.torproject.org/rs.html#details/5D575ADD108DDBBF17E78AD8CB267D6C1F338206) | 2022-09-03   | Yes         |                    32 |
| [Hydra91a](https://metrics.torproject.org/rs.html#details/AEC8D545DDEDC0311FA7F9F9A885D674D1F1C2FF) | 2022-07-10   | Yes         |                    32 |
| [Hydra94a](https://metrics.torproject.org/rs.html#details/61866162CCDFE651B0D76AA57ECA90B9CC7C80DD) | 2022-09-03   | Yes         |                    32 |
| [Hydra90a](https://metrics.torproject.org/rs.html#details/21328917A9379E6B8ABCB49A0DBE3AAE885CFC15) | 2022-11-02   | Yes         |                     1 |
| [Hydra71a](https://metrics.torproject.org/rs.html#details/9F95C68AACB67E6258EC7A6BA9406C227ABAD3F0) | 2021-09-19   | Yes         |                    32 |
| [Hydra72a](https://metrics.torproject.org/rs.html#details/FB79B2BE707F272FBFE1584F44A3FA5156F7F1CF) | 2021-09-19   | Yes         |                    32 |
| [Hydra24a](https://metrics.torproject.org/rs.html#details/8F293A6484A0973167B15C4997AB9F24C21143FE) | 2020-11-11   | Yes         |                    32 |
| [Hydra73a](https://metrics.torproject.org/rs.html#details/391F278B2B55548B97410ADFBD055D079D798E04) | 2021-09-19   | Yes         |                    32 |
| [Hydra70a](https://metrics.torproject.org/rs.html#details/DCCBB9717CD8B1F031B9A38C721D2BD9615697AA) | 2021-09-09   | Yes         |                    32 |
| [Hydra69a](https://metrics.torproject.org/rs.html#details/7B3535760987464C8B5686F203B6EBE767C0873E) | 2021-09-09   | Yes         |                    32 |
| [Hydra17](https://metrics.torproject.org/rs.html#details/E3DAF067B028450B31CF5CE118F2F9AC53146ABD)  | 2020-06-09   | Yes         |                    32 |
| [Hydra57a](https://metrics.torproject.org/rs.html#details/0F0F690AF1D32C7C3C72C543836625628887BA85) | 2021-06-05   | Yes         |                    32 |
| [Hydra20](https://metrics.torproject.org/rs.html#details/86E479266EBB982E204009532ED460628689E5B5)  | 2020-10-07   | Yes         |                    32 |
| [Hydra19](https://metrics.torproject.org/rs.html#details/E465AD166798A3CD0A4866FA2A8BB5ADD157FBD5)  | 2020-06-30   | Yes         |                    32 |
| [Hydra52a](https://metrics.torproject.org/rs.html#details/9BF600D6C06A3FBE28216C58CD241A89931CBE7D) | 2021-03-14   | Yes         |                    32 |
| [Hydra51a](https://metrics.torproject.org/rs.html#details/3E610CDAB3B6993E5C31CC99CB10ED8E9CC6F612) | 2022-11-01   | Yes         |                     1 |
| [Hydra45](https://metrics.torproject.org/rs.html#details/01CFCC2545234EEE523D33ED25EF1E79807A18A7)  | 2021-03-04   | No          |                    32 |
| [Hydra55](https://metrics.torproject.org/rs.html#details/378AD3D089A01EC802F165A936122B60B5B1035E)  | 2021-06-06   | No          |                    32 |
| [Hydra28](https://metrics.torproject.org/rs.html#details/427956E3F23EEBA31954CB0942AEA0ECD43A004A)  | 2020-11-20   | No          |                    32 |
| [Hydra59](https://metrics.torproject.org/rs.html#details/47FC19DBE2B42BB481C65191276670B3D589F075)  | 2021-04-09   | No          |                    32 |
| [Hydra37](https://metrics.torproject.org/rs.html#details/5058E7136283B4CE13F1897871F931CC41F41CC9)  | 2021-03-04   | No          |                    32 |
| [Hydra58](https://metrics.torproject.org/rs.html#details/512F27DD9A2937A8E3D65EDA13A88AE9483E9ACA)  | 2021-04-09   | No          |                    32 |
| [Hydra36](https://metrics.torproject.org/rs.html#details/5ACC59F3117F1F6FAD8C89F469823CB48BDB5D2F)  | 2021-03-04   | No          |                    32 |
| [Hydra75](https://metrics.torproject.org/rs.html#details/63928D370B929EBDA54EF2ABDD4A63082085BF61)  | 2021-09-22   | No          |                    32 |
| [Hydra25](https://metrics.torproject.org/rs.html#details/6CB18098F50819DEAB22E369EC3A5661A552A66C)  | 2020-11-20   | No          |                    32 |
| [Hydra27](https://metrics.torproject.org/rs.html#details/A0A91967046F7A9BC3154C7B3C3FDE34C02B1017)  | 2020-11-20   | No          |                    32 |
| [Hydra65](https://metrics.torproject.org/rs.html#details/A62D8F7772A6C76DD07F431810CE68682DCDD2DC)  | 2021-09-09   | No          |                    32 |
| [Hydra66](https://metrics.torproject.org/rs.html#details/C85B30A8356E826418CB901254B7595FE1430619)  | 2021-09-09   | No          |                    32 |

## ContactInfo: email:sysop openinternet.io offlinemasterkey:y ci (8) {#emailsysopopeninternetio-offlinemasterkeyy-ci}

| Nickname                                                                                                     | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [UkranianStrong](https://metrics.torproject.org/rs.html#details/CE30CE396D62B6BC9DEFC8344DA89BFD60083665)    | 2022-07-25   | Yes         |                     1 |
| [AltAddress02](https://metrics.torproject.org/rs.html#details/5191E3F9A8B9B0C8F356FF0A7D0DA30D95652116)      | 2022-11-26   | Yes         |                     7 |
| [AltAddress01](https://metrics.torproject.org/rs.html#details/80CA806137BF939FBADF38B106A7BBF631FE0F76)      | 2022-11-26   | Yes         |                     7 |
| [OpenInternet](https://metrics.torproject.org/rs.html#details/F37191452612F22EFB6F6204C75A45BF0B11B366)      | 2022-11-22   | Yes         |                     1 |
| [AltAddress010](https://metrics.torproject.org/rs.html#details/A61B17D64D4B08FF75508893C180B2B41E055D40)     | 2023-02-15   | Yes         |                     7 |
| [UkranianStrong2](https://metrics.torproject.org/rs.html#details/655F75D0A03DF94298A8BAB663C60FB25D501760)   | 2022-12-01   | Yes         |                     7 |
| [Iter](https://metrics.torproject.org/rs.html#details/F3689448309B46A9B7A6612C54C205BAF0971E37)              | 2022-07-22   | Yes         |                     7 |
| [BeCarefulOutThere](https://metrics.torproject.org/rs.html#details/51BD25EE06C46E4466427D4ABF94F2964514EB2F) | 2020-09-10   | No          |                     7 |


## Fingerprint List of Guard-only Relays in E2E Groups

0F0F690AF1D32C7C3C72C543836625628887BA85,21328917A9379E6B8ABCB49A0DBE3AAE885CFC15,391F278B2B55548B97410ADFBD055D079D798E04,3E610CDAB3B6993E5C31CC99CB10ED8E9CC6F612,5D575ADD108DDBBF17E78AD8CB267D6C1F338206,61866162CCDFE651B0D76AA57ECA90B9CC7C80DD,7B3535760987464C8B5686F203B6EBE767C0873E,86E479266EBB982E204009532ED460628689E5B5,8F293A6484A0973167B15C4997AB9F24C21143FE,9BF600D6C06A3FBE28216C58CD241A89931CBE7D,9F95C68AACB67E6258EC7A6BA9406C227ABAD3F0,AEC8D545DDEDC0311FA7F9F9A885D674D1F1C2FF,DCCBB9717CD8B1F031B9A38C721D2BD9615697AA,E3DAF067B028450B31CF5CE118F2F9AC53146ABD,E465AD166798A3CD0A4866FA2A8BB5ADD157FBD5,FB79B2BE707F272FBFE1584F44A3FA5156F7F1CF,5191E3F9A8B9B0C8F356FF0A7D0DA30D95652116,655F75D0A03DF94298A8BAB663C60FB25D501760,80CA806137BF939FBADF38B106A7BBF631FE0F76,A61B17D64D4B08FF75508893C180B2B41E055D40,CE30CE396D62B6BC9DEFC8344DA89BFD60083665,F3689448309B46A9B7A6612C54C205BAF0971E37,F37191452612F22EFB6F6204C75A45BF0B11B366