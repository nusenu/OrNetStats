---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-03-20 09:00 UTC**

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


## ContactInfo: concept@protonmail.ch (16) {#conceptprotonmailch}

| Nickname                                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Unnamed](https://metrics.torproject.org/rs.html#details/D032BD6C16B44F4E8A93A3AB0874435EF5B1CF2A)          | 2022-01-06   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/C71D833CE0B43F8CAD39DD8AD1A441E6F07F758B)          | 2022-01-06   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/B5C44D74017C98E8666DBA6B9D01AF127E21C9C1)          | 2022-01-04   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/E6FB13F2E0F6B89D8F4548D3B7A96A30F9410CBE)          | 2022-01-04   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/BAE07C406FE5872AF8CFDD9EFEC8F2EB4B56F2B2)          | 2022-01-19   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/CD73F85BD3B0F6517E5498F68FA61D4D791DB4D1)          | 2022-01-19   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/AA8510CE7B5D13147E048F39B5BF51346B3C676F)          | 2022-02-02   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/14C87FC26BFB1C96175FBCA3FECDF30A495C446F)          | 2022-02-02   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/A1C34F92FD799ABBDFD02904B3FED31B2006EECC)          | 2022-03-12   | Yes         |                    14 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/676F39FEFEBC206078DAD5A68994CC3E49F15C19)          | 2022-01-06   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/4A90398043DAC7DCB800F8A5BD9BC4B80A052F2D)          | 2022-01-06   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/BA2F71EAFDDB4DDE64FB9CAA819775CDEE9A144A)          | 2022-03-12   | Yes         |                    14 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/D0E11C28CC772C736B5B95079B638FFC4CAA203D)          | 2022-02-16   | Yes         |                    16 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/ACE7AC8CFDB1E2222FCF490BD8ED0F1384F26950)          | 2022-02-16   | Yes         |                    16 |
| [conceptexitrelay](https://metrics.torproject.org/rs.html#details/76EB3AD90935077F9E63085CE6A56EEDAEF14DD0) | 2021-12-25   | No          |                    14 |
| [conceptexitrelay](https://metrics.torproject.org/rs.html#details/B1101A4EB7A09BB58351B146630C06F46A617703) | 2021-12-25   | No          |                    14 |

## ContactInfo: &lt;nobody AT example dot com&gt; (3) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [node01](https://metrics.torproject.org/rs.html#details/D53AE170BF6650A2C6640484FE1B5DD1C0AB895B)     | 2019-12-14   | Yes         |                     1 |
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |

## ContactInfo: gusntwrk.xyz (2) {#gusntwrkxyz}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [elhombre](https://metrics.torproject.org/rs.html#details/D7910C73B9092697D7D2AF14E5CA09112F0C6EA9) | 2021-12-11   | Yes         |                     1 |
| [rknchan](https://metrics.torproject.org/rs.html#details/A5B984C20AF47731B911CDF68032A36F8678C25B)  | 2022-02-19   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

14C87FC26BFB1C96175FBCA3FECDF30A495C446F,4A90398043DAC7DCB800F8A5BD9BC4B80A052F2D,676F39FEFEBC206078DAD5A68994CC3E49F15C19,A1C34F92FD799ABBDFD02904B3FED31B2006EECC,AA8510CE7B5D13147E048F39B5BF51346B3C676F,ACE7AC8CFDB1E2222FCF490BD8ED0F1384F26950,B5C44D74017C98E8666DBA6B9D01AF127E21C9C1,BA2F71EAFDDB4DDE64FB9CAA819775CDEE9A144A,BAE07C406FE5872AF8CFDD9EFEC8F2EB4B56F2B2,C71D833CE0B43F8CAD39DD8AD1A441E6F07F758B,CD73F85BD3B0F6517E5498F68FA61D4D791DB4D1,A9A4213EA3D707857368C683F2208C83B8755D8A,D032BD6C16B44F4E8A93A3AB0874435EF5B1CF2A,D0E11C28CC772C736B5B95079B638FFC4CAA203D,E6FB13F2E0F6B89D8F4548D3B7A96A30F9410CBE,D53AE170BF6650A2C6640484FE1B5DD1C0AB895B,D7910C73B9092697D7D2AF14E5CA09112F0C6EA9