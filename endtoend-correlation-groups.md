---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-08-24 18:00 UTC**

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


## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; (32) {#neel-chauhan-neel-at-neelc-dot-org}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay1](https://metrics.torproject.org/rs.html#details/97011FAE9F14C820BEB31C467DEA11E6BFCCA0E1) | 2023-03-11   | Yes         |                    32 |
| [NeelTorRelay3](https://metrics.torproject.org/rs.html#details/BA3B3FBB7F23A9580A94DE811F1F2017CEFF52E1) | 2023-05-03   | Yes         |                    32 |
| [NeelTorRelay2](https://metrics.torproject.org/rs.html#details/6E21BB0F39095B207C45DBBD30A521F0CABBF6A7) | 2023-03-11   | Yes         |                    32 |
| [NeelTorRelay4](https://metrics.torproject.org/rs.html#details/66BCB27A28C3C98987C2F5A87E3F80282BE1DB32) | 2023-05-03   | Yes         |                    32 |
| [opsrelayE2](https://metrics.torproject.org/rs.html#details/01EC8FFBEBA761CC5A37C4AE4A572CFF252EBEED)    | 2023-08-18   | No          |                    29 |
| [opsrelayB6](https://metrics.torproject.org/rs.html#details/0601A2CBCFAE793E4A4D01B21282FA859DAEADB4)    | 2023-07-19   | No          |                    32 |
| [opsrelayA6](https://metrics.torproject.org/rs.html#details/096472DC09D4ACDD11DC032DA96376329E6962EC)    | 2023-07-19   | No          |                    32 |
| [opsrelayA4](https://metrics.torproject.org/rs.html#details/0A23830EF2CB5210CEB02125ED6A84E1D3B5E457)    | 2023-07-19   | No          |                    32 |
| [opsrelayC1](https://metrics.torproject.org/rs.html#details/16AF8E6C4FC3882B55B0B004F578FCD528A0C0D1)    | 2023-08-17   | No          |                    32 |
| [opsrelayC4](https://metrics.torproject.org/rs.html#details/2FBECCF951385053C630912B9142305383B7967F)    | 2023-08-17   | No          |                    32 |
| [opsrelayE4](https://metrics.torproject.org/rs.html#details/371D3109A3C750B39475E471B0650D580554D9E4)    | 2023-08-18   | No          |                    29 |
| [opsrelayB1](https://metrics.torproject.org/rs.html#details/429F6AC2CB4109264FC15FA2B5BE684948B23626)    | 2023-07-19   | No          |                    32 |
| [opsrelayD4](https://metrics.torproject.org/rs.html#details/50AFAA1BAF96733E3BA8988C986E379ACF6735BE)    | 2023-08-17   | No          |                    32 |
| [opsrelayD1](https://metrics.torproject.org/rs.html#details/511A1BD6D1F3F7622BAF2B9C9FBFAC0A6DCA7917)    | 2023-08-17   | No          |                    32 |
| [opsrelayB4](https://metrics.torproject.org/rs.html#details/518842E808C15E4E64CC4D2B1BE4AB655EE2BAA7)    | 2023-07-19   | No          |                    32 |
| [opsrelayA1](https://metrics.torproject.org/rs.html#details/52A0801DFD404DD1B9C4E6C2F633E79762DD4B86)    | 2023-07-19   | No          |                    32 |
| [opsrelayE1](https://metrics.torproject.org/rs.html#details/6082B5805CE95C3B84C9B0E1942098DEB5EEF2C6)    | 2023-08-18   | No          |                    29 |
| [opsrelayA8](https://metrics.torproject.org/rs.html#details/671FF484A7D244949522F08F1DFE9BDC5E663C11)    | 2023-07-19   | No          |                    32 |
| [opsrelayA3](https://metrics.torproject.org/rs.html#details/67CAE8CD5AFF7A0F90CF08BC7679D4626B2C8E6F)    | 2023-07-19   | No          |                    32 |
| [opsrelayB2](https://metrics.torproject.org/rs.html#details/683A38A43C32AF905447A247D121490665D5BA72)    | 2023-07-19   | No          |                    32 |
| [opsrelayB3](https://metrics.torproject.org/rs.html#details/69FCA578DDE9E16AA0D0A54ACE6623E65DC052DC)    | 2023-07-19   | No          |                    32 |
| [opsrelayA7](https://metrics.torproject.org/rs.html#details/6D7AD9A8CA05CBA7C41F6D091C352B46F3F0D087)    | 2023-07-19   | No          |                    32 |
| [opsrelayD2](https://metrics.torproject.org/rs.html#details/76DAB41B0DB692E70DF44DC2EA3ECD36000E390E)    | 2023-08-17   | No          |                    32 |
| [opsrelayE3](https://metrics.torproject.org/rs.html#details/7C3D6E96811A1A3F52EF72C0358BBF008303DBAA)    | 2023-08-18   | No          |                    29 |
| [opsrelayD3](https://metrics.torproject.org/rs.html#details/A23617B555C97723BE171B8BB14EF80BCD56D205)    | 2023-08-17   | No          |                    32 |
| [opsrelayB8](https://metrics.torproject.org/rs.html#details/A64C1EB191016B14AD3EC4A18F04777C7EC0C62D)    | 2023-07-19   | No          |                    32 |
| [opsrelayB7](https://metrics.torproject.org/rs.html#details/B046C7875331873C056525985ECFEB46422080AD)    | 2023-07-19   | No          |                    32 |
| [opsrelayC3](https://metrics.torproject.org/rs.html#details/C2AD153AE6A28427DA4ADC60646BDF25C57DFB9E)    | 2023-08-17   | No          |                    32 |
| [opsrelayC2](https://metrics.torproject.org/rs.html#details/C32B80AA92320EB2EDD6813082E5BFBD975D6C66)    | 2023-08-17   | No          |                    32 |
| [opsrelayA2](https://metrics.torproject.org/rs.html#details/E1E99C9C48054C988A124BE5678A45F883FC8E72)    | 2023-07-19   | No          |                    32 |
| [opsrelayB5](https://metrics.torproject.org/rs.html#details/E29727F1EC26F269E3122DABFD2BD71AC7CA35C4)    | 2023-07-19   | No          |                    32 |
| [opsrelayA5](https://metrics.torproject.org/rs.html#details/FED7827C761F18938D4CC8D8BDBECFC5BFFF95C7)    | 2023-07-19   | No          |                    32 |

## ContactInfo: abuse at riverside dot rocks (2) {#abuseatriversidedotrocks}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [BackInBlack](https://metrics.torproject.org/rs.html#details/6D04FFDA1E5E352B9F7477D3E15BB1B59B459691) | 2021-09-27   | Yes         |                     1 |
| [100UPSkid](https://metrics.torproject.org/rs.html#details/392505E115D4415674E731D6BE215E2AE5E56D59)   | 2022-05-19   | No          |                     2 |


## Fingerprint List of Guard-only Relays in E2E Groups

66BCB27A28C3C98987C2F5A87E3F80282BE1DB32,6E21BB0F39095B207C45DBBD30A521F0CABBF6A7,97011FAE9F14C820BEB31C467DEA11E6BFCCA0E1,BA3B3FBB7F23A9580A94DE811F1F2017CEFF52E1,6D04FFDA1E5E352B9F7477D3E15BB1B59B459691