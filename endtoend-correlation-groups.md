---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-05-15 20:00 UTC**

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


## ContactInfo: &lt;nobody AT example dot com&gt; (3) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [node01](https://metrics.torproject.org/rs.html#details/D53AE170BF6650A2C6640484FE1B5DD1C0AB895B)     | 2019-12-14   | Yes         |                     1 |
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |

## ContactInfo: g at switchblad dot es tor-relay.co (2) {#gatswitchbladdotes-tor-relayco}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [socialsbionl](https://metrics.torproject.org/rs.html#details/74C11CE0CD6BFD1AEDA1BEC526ABBE10D95EB207) | 2022-05-03   | Yes         |                     1 |
| [socialsbio](https://metrics.torproject.org/rs.html#details/00843BC25EDD6ED738DC0159A24E6452A860C74A)   | 2022-05-03   | No          |                     1 |

## ContactInfo: gusntwrk.xyz (2) {#gusntwrkxyz}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [elhombre](https://metrics.torproject.org/rs.html#details/D7910C73B9092697D7D2AF14E5CA09112F0C6EA9) | 2021-12-11   | Yes         |                     1 |
| [rknchan](https://metrics.torproject.org/rs.html#details/A5B984C20AF47731B911CDF68032A36F8678C25B)  | 2022-02-19   | No          |                     1 |

## ContactInfo: torix aT=== protonmail&lt;dOT &gt;com (11) {#torixatprotonmaildotcom}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Aramis67](https://metrics.torproject.org/rs.html#details/53C9F4954E7A7332BB0C610C5B8E04CA065AF29B) | 2019-05-13   | Yes         |                    12 |
| [Aramis65](https://metrics.torproject.org/rs.html#details/99DB99DF22EE52B9B3A32749C12EDEA78F166B3F) | 2021-12-03   | Yes         |                    12 |
| [Aramis66](https://metrics.torproject.org/rs.html#details/39A18F31B312E5CB211781090766934C1CFDAB36) | 2020-07-10   | Yes         |                     8 |
| [Aramis](https://metrics.torproject.org/rs.html#details/17F41F8DAFA4B36AAB10E202ABA14601AAE1D616)   | 2022-05-10   | No          |                     7 |
| [Aramis](https://metrics.torproject.org/rs.html#details/2B3AAC97B269D59E6D642C8BFB174EDD13741C38)   | 2021-11-12   | No          |                     8 |
| [Aramis](https://metrics.torproject.org/rs.html#details/359C5231AC2452D365B64A23C27817A1DFEE56B4)   | 2022-05-10   | No          |                     7 |
| [Aramis](https://metrics.torproject.org/rs.html#details/4F9EFCF7689084E4C8EE993E123E32B75368804C)   | 2021-08-22   | No          |                     8 |
| [Aramis](https://metrics.torproject.org/rs.html#details/9EF49A075A79F657708F5EE00B05CE7B0B79DA35)   | 2022-05-10   | No          |                     7 |
| [Aramis](https://metrics.torproject.org/rs.html#details/A549E57FC2A060FA20051537E6738B3ED5B98463)   | 2022-05-10   | No          |                     7 |
| [Aramis](https://metrics.torproject.org/rs.html#details/D3F6616034448DEEE369782C96F84FE1407E4200)   | 2021-08-22   | No          |                     8 |
| [Aramis](https://metrics.torproject.org/rs.html#details/F314580EA22CB3DCB135D64E92108BFB8FD209AF)   | 2021-11-12   | No          |                     8 |


## Fingerprint List of Guard-only Relays in E2E Groups

A9A4213EA3D707857368C683F2208C83B8755D8A,74C11CE0CD6BFD1AEDA1BEC526ABBE10D95EB207,39A18F31B312E5CB211781090766934C1CFDAB36,53C9F4954E7A7332BB0C610C5B8E04CA065AF29B,99DB99DF22EE52B9B3A32749C12EDEA78F166B3F,D53AE170BF6650A2C6640484FE1B5DD1C0AB895B,D7910C73B9092697D7D2AF14E5CA09112F0C6EA9