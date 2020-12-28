---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-12-28 12:00 UTC**

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

## ContactInfo: &lt;admin AT my-mail dot rocks&gt; (4) {#admin-at-my-mail-dot-rocks}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/5B57662F90717DADC37C857BC595F13473B8550F) | 2020-12-18   | Yes         |                     1 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/5152F22FD8215F0C78373A96248F05169B5CB563) | 2020-12-13   | Yes         |                     1 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/784F16D7257C40002998EE54454D2264BA4B67EB) | 2020-12-20   | No          |                     1 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/D1B853ED27E4DFDCA3A54D3F2E269C4D94677F66) | 2018-04-16   | No          |                     1 |

## ContactInfo: abuse at yggdrasil dot ws (6) {#abuseatyggdrasildotws}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [BKA](https://metrics.torproject.org/rs.html#details/DA580E4EB2A453298D40F73ECFC78E896B001182)      | 2020-10-07   | Yes         |                     5 |
| [Loki](https://metrics.torproject.org/rs.html#details/0ADAC68F29875A1366F06762F2B305B0BFD11364)     | 2020-12-02   | No          |                     1 |
| [Ymir](https://metrics.torproject.org/rs.html#details/4AA0035604DF40E5BA20DBE88EF6D11432421BFA)     | 2020-10-27   | No          |                     5 |
| [Ganymed](https://metrics.torproject.org/rs.html#details/5AFF7583F5ED62A274823C83199F2E19083692EC)  | 2020-08-20   | No          |                     5 |
| [Freya](https://metrics.torproject.org/rs.html#details/85ED839A03D10C46219609625D7FEAE59EDCCFDD)    | 2020-05-27   | No          |                     5 |
| [Kallisto](https://metrics.torproject.org/rs.html#details/D4C5BAEA92CADCC02D64E0DD9F1A49024C57F05C) | 2020-09-11   | No          |                     5 |

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

## ContactInfo: citizen17 at tutamail dot com (5) {#citizen17attutamaildotcom}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [citizen17](https://metrics.torproject.org/rs.html#details/5B6F8535D0DFB1C26FE54E15FA3C82D8D8AB380B) | 2020-09-06   | No          |                     1 |
| [citizen17](https://metrics.torproject.org/rs.html#details/271C445DEAA2E0DB1E740CDBC61D77BA9133155B) | 2020-09-06   | No          |                     1 |
| [citizen17](https://metrics.torproject.org/rs.html#details/53887FD502CE6CF4FE10592D1D74D9480251AF1E) | 2020-09-06   | No          |                     1 |
| [citizen17](https://metrics.torproject.org/rs.html#details/A959D9E66BA7366915F4C1C08980398D824C7D6A) | 2020-09-06   | No          |                     1 |
| [citizen17](https://metrics.torproject.org/rs.html#details/D37318440E1A94D1C2055A43B536ECC9406994CD) | 2020-09-06   | No          |                     1 |

## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; (6) {#neel-chauhan-neel-at-neelc-dot-org}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelayB](https://metrics.torproject.org/rs.html#details/DB710B14D7329B7289CFCC547F48EF53F812C40D) | 2020-06-14   | Yes         |                     4 |
| [NeelTorRelayA](https://metrics.torproject.org/rs.html#details/B0F9BA27944FA59E3B1A182208FF7C0CFF5497B2) | 2020-06-14   | Yes         |                     4 |
| [NeelTorExitE](https://metrics.torproject.org/rs.html#details/02AB0923AFF5A47DD011C343F79864C45E9FFB34)  | 2020-05-30   | No          |                     4 |
| [NeelTorExitA](https://metrics.torproject.org/rs.html#details/156AAC3FAD1ACC8906316519DCB444B8C77E4EBF)  | 2020-07-28   | No          |                     4 |
| [NeelTorExitF](https://metrics.torproject.org/rs.html#details/16AD4988F437D3478B72DAD0C1A20E61847FEF3C)  | 2020-06-15   | No          |                     4 |
| [NeelTorExitB](https://metrics.torproject.org/rs.html#details/A69CEB30328B1E85C6B167FECAF2F509CBD9517F)  | 2020-07-28   | No          |                     4 |

## ContactInfo: tor at a9 dot wtf (2) {#torata9dotwtf}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [a9TorRelay04](https://metrics.torproject.org/rs.html#details/BD0DBFEE1A5CBF890A68741339A6DE247896D276) | 2020-11-11   | Yes         |                     2 |
| [a9TorExit](https://metrics.torproject.org/rs.html#details/2DB8A946826D0CB4F5C3A8264628DD0F16F6612D)    | 2020-09-12   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

C3ACB0492A644E27A549BC3CDF3B7A129186E3BF,C64EB4553AA308D8FBC314D73B44178E4CB11C35,5152F22FD8215F0C78373A96248F05169B5CB563,5B57662F90717DADC37C857BC595F13473B8550F,DA580E4EB2A453298D40F73ECFC78E896B001182,1B9FACF25E17D26E307EA7CFA7D455B144B032E5,B0F9BA27944FA59E3B1A182208FF7C0CFF5497B2,DB710B14D7329B7289CFCC547F48EF53F812C40D,BD0DBFEE1A5CBF890A68741339A6DE247896D276