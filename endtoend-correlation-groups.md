---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-05-06 09:00 UTC**

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


## ContactInfo: Brandon Kuschel &lt;kusch023 AT NOSPAM umn dot edu&gt; (22) {#brandon-kuschel-kusch023-at-nospam-umn-dot-edu}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Lamia](https://metrics.torproject.org/rs.html#details/C46548D44C0CA5855C175CE26F5817D38F833C9F)       | 2022-08-21   | Yes         |                    22 |
| [Charybdis3](https://metrics.torproject.org/rs.html#details/8BF4E024210FF5DB1D7A4AFEBE11B48C73BFE779)  | 2023-02-11   | Yes         |                    22 |
| [Lamia2](https://metrics.torproject.org/rs.html#details/786835D15C33DCD2B7FD9E70CACBCDA3D6187300)      | 2022-12-11   | Yes         |                    22 |
| [Charybdis2](https://metrics.torproject.org/rs.html#details/1DEECD906AFECF496B7DC1E40829F4563517B4CC)  | 2022-09-19   | Yes         |                    22 |
| [Minotaur3](https://metrics.torproject.org/rs.html#details/147CA31A3CD14F2EF7269BFDAE9A879E75295E2C)   | 2022-10-17   | Yes         |                    22 |
| [Lamia3](https://metrics.torproject.org/rs.html#details/09F4736B37FA72AC7399F71F917F895D3CF22685)      | 2023-04-28   | Yes         |                    22 |
| [Minotaur2](https://metrics.torproject.org/rs.html#details/6E586C8F62D0E153792095AFDA55D4E2E3F3421F)   | 2022-09-19   | Yes         |                    22 |
| [Echidna](https://metrics.torproject.org/rs.html#details/BA57222A0EC9ECDF003AED665DFB0B1287EA039D)     | 2022-08-21   | Yes         |                    21 |
| [Minotaur5](https://metrics.torproject.org/rs.html#details/A4789FA2F79E8EE39CFE3D272D6DBA599068EB28)   | 2023-02-11   | Yes         |                    22 |
| [Echidna2](https://metrics.torproject.org/rs.html#details/EA05F22892CE6B556DD5F1733248A84AD883C116)    | 2022-12-11   | Yes         |                    22 |
| [Echidna3](https://metrics.torproject.org/rs.html#details/CB1816F95D43D6805230ED63326E88B0D4A7ABD7)    | 2023-04-28   | Yes         |                    21 |
| [Minotaur4](https://metrics.torproject.org/rs.html#details/FFA371808475B05A9544E4A4BA413B486B049E74)   | 2023-02-11   | Yes         |                    22 |
| [Charybdis](https://metrics.torproject.org/rs.html#details/CBF59EC5B9FD108092AE9149EFDAE41F882DA669)   | 2022-08-19   | No          |                    22 |
| [Chimera2](https://metrics.torproject.org/rs.html#details/4E60DE549B3B4C063E6035BCDAA69DD4F3AE3C4D)    | 2022-12-11   | No          |                    22 |
| [Chimera](https://metrics.torproject.org/rs.html#details/2946159CF9D8EAEB8C4A27F6A54B01A459DEE164)     | 2022-08-21   | No          |                    22 |
| [Polyphemus2](https://metrics.torproject.org/rs.html#details/044428D910C037932A0763BB089769943F6BA648) | 2022-10-19   | No          |                    22 |
| [Polyphemus](https://metrics.torproject.org/rs.html#details/0CABED9159F1E4BE82879F5A34ED8D7349E931BD)  | 2022-09-14   | No          |                    22 |
| [Polyphemus3](https://metrics.torproject.org/rs.html#details/826C85481CCB8496EC3E67A4A477C24808D74011) | 2022-11-05   | No          |                    22 |
| [Polyphemus4](https://metrics.torproject.org/rs.html#details/41C106EAEB0B968C5E68927596500DC99B840367) | 2023-02-11   | No          |                    22 |
| [Polyphemus5](https://metrics.torproject.org/rs.html#details/0F3874C18BE50B83939D09AF2F6C362D1FC6C8CD) | 2023-02-11   | No          |                    22 |
| [Polyphemus6](https://metrics.torproject.org/rs.html#details/EDB75B4ED148C676B65A2631AC35682687F90BE7) | 2023-02-11   | No          |                    22 |
| [Minotaur](https://metrics.torproject.org/rs.html#details/8BDBE498180C41249D3230FC5092CB3EB5A62482)    | 2021-04-06   | No          |                    22 |

## ContactInfo: email:torix protonmail.com url:https://torix-rela (15) {#emailtorixprotonmailcom-urlhttpstorix-rela}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Aramis67](https://metrics.torproject.org/rs.html#details/53C9F4954E7A7332BB0C610C5B8E04CA065AF29B) | 2019-05-13   | Yes         |                     9 |
| [Aramis](https://metrics.torproject.org/rs.html#details/17F41F8DAFA4B36AAB10E202ABA14601AAE1D616)   | 2022-05-10   | No          |                    19 |
| [Aramis](https://metrics.torproject.org/rs.html#details/9EF49A075A79F657708F5EE00B05CE7B0B79DA35)   | 2022-05-10   | No          |                    19 |
| [Aramis](https://metrics.torproject.org/rs.html#details/A549E57FC2A060FA20051537E6738B3ED5B98463)   | 2022-05-10   | No          |                    19 |
| [Aramis](https://metrics.torproject.org/rs.html#details/359C5231AC2452D365B64A23C27817A1DFEE56B4)   | 2022-05-10   | No          |                    19 |
| [Aramis](https://metrics.torproject.org/rs.html#details/F3E6F01671C087AD318BBA47FCD08B65D1A4460E)   | 2022-06-18   | No          |                    14 |
| [Aramis](https://metrics.torproject.org/rs.html#details/C29FEF6A405E730DE07EC74CCF0623D95F0D3A4E)   | 2022-06-18   | No          |                    14 |
| [Aramis](https://metrics.torproject.org/rs.html#details/B5A65B997C898583F9C4CA16FE603B7347C89588)   | 2022-06-18   | No          |                    14 |
| [Aramis](https://metrics.torproject.org/rs.html#details/C528B22D4BA220639F9DCE86A50BB98BDD2FCFB9)   | 2022-06-18   | No          |                    14 |
| [Aramis](https://metrics.torproject.org/rs.html#details/9A8902B985E2F58BC740671040E7165AC904DD40)   | 2022-06-18   | No          |                    14 |
| [Aramis](https://metrics.torproject.org/rs.html#details/791DEA860D359D3A3D2F6F13B9856EB0507ED835)   | 2022-06-18   | No          |                    14 |
| [Aramis](https://metrics.torproject.org/rs.html#details/4F9EFCF7689084E4C8EE993E123E32B75368804C)   | 2021-08-22   | No          |                    14 |
| [Aramis](https://metrics.torproject.org/rs.html#details/D3F6616034448DEEE369782C96F84FE1407E4200)   | 2021-08-22   | No          |                    14 |
| [Aramis](https://metrics.torproject.org/rs.html#details/2B3AAC97B269D59E6D642C8BFB174EDD13741C38)   | 2021-11-12   | No          |                    14 |
| [Aramis](https://metrics.torproject.org/rs.html#details/F314580EA22CB3DCB135D64E92108BFB8FD209AF)   | 2021-11-12   | No          |                    14 |


## Fingerprint List of Guard-only Relays in E2E Groups

09F4736B37FA72AC7399F71F917F895D3CF22685,147CA31A3CD14F2EF7269BFDAE9A879E75295E2C,1DEECD906AFECF496B7DC1E40829F4563517B4CC,6E586C8F62D0E153792095AFDA55D4E2E3F3421F,786835D15C33DCD2B7FD9E70CACBCDA3D6187300,8BF4E024210FF5DB1D7A4AFEBE11B48C73BFE779,A4789FA2F79E8EE39CFE3D272D6DBA599068EB28,BA57222A0EC9ECDF003AED665DFB0B1287EA039D,C46548D44C0CA5855C175CE26F5817D38F833C9F,CB1816F95D43D6805230ED63326E88B0D4A7ABD7,EA05F22892CE6B556DD5F1733248A84AD883C116,FFA371808475B05A9544E4A4BA413B486B049E74