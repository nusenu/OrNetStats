---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-07-14 16:00 UTC**

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


## ContactInfo: Brandon Kuschel &lt;kusch023 AT NOSPAM umn dot edu&gt; (34) {#brandon-kuschel-kusch023-at-nospam-umn-dot-edu}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Lamia2](https://metrics.torproject.org/rs.html#details/786835D15C33DCD2B7FD9E70CACBCDA3D6187300)       | 2022-12-11   | Yes         |                    34 |
| [Lamia](https://metrics.torproject.org/rs.html#details/C46548D44C0CA5855C175CE26F5817D38F833C9F)        | 2022-08-21   | Yes         |                    34 |
| [Charybdis4](https://metrics.torproject.org/rs.html#details/4B6A58C6E678F2B0F422D229F20284AB35194223)   | 2023-06-10   | Yes         |                    34 |
| [Charybdis5](https://metrics.torproject.org/rs.html#details/65369D044C659CD299E35763914FFD0FC9AD4509)   | 2023-06-10   | Yes         |                    34 |
| [Charybdis2](https://metrics.torproject.org/rs.html#details/1DEECD906AFECF496B7DC1E40829F4563517B4CC)   | 2022-09-19   | Yes         |                    34 |
| [Lamia3](https://metrics.torproject.org/rs.html#details/09F4736B37FA72AC7399F71F917F895D3CF22685)       | 2023-04-28   | Yes         |                    34 |
| [Charybdis3](https://metrics.torproject.org/rs.html#details/8BF4E024210FF5DB1D7A4AFEBE11B48C73BFE779)   | 2023-02-11   | Yes         |                    34 |
| [Minotaur3](https://metrics.torproject.org/rs.html#details/147CA31A3CD14F2EF7269BFDAE9A879E75295E2C)    | 2022-10-17   | Yes         |                    34 |
| [Echidna](https://metrics.torproject.org/rs.html#details/BA57222A0EC9ECDF003AED665DFB0B1287EA039D)      | 2022-08-21   | Yes         |                    32 |
| [Minotaur2](https://metrics.torproject.org/rs.html#details/6E586C8F62D0E153792095AFDA55D4E2E3F3421F)    | 2022-09-19   | Yes         |                    34 |
| [Minotaur7](https://metrics.torproject.org/rs.html#details/B207494B6E471AB65C84891639D15F93750481E5)    | 2023-06-10   | Yes         |                    34 |
| [Minotaur5](https://metrics.torproject.org/rs.html#details/A4789FA2F79E8EE39CFE3D272D6DBA599068EB28)    | 2023-02-11   | Yes         |                    34 |
| [Echidna2](https://metrics.torproject.org/rs.html#details/EA05F22892CE6B556DD5F1733248A84AD883C116)     | 2022-12-11   | Yes         |                    32 |
| [Minotaur4](https://metrics.torproject.org/rs.html#details/FFA371808475B05A9544E4A4BA413B486B049E74)    | 2023-02-11   | Yes         |                    34 |
| [Echidna4](https://metrics.torproject.org/rs.html#details/A9A567CC15293CD3CD6B2BC12A435F37731843A2)     | 2023-06-07   | Yes         |                    32 |
| [Lamia4](https://metrics.torproject.org/rs.html#details/961522CCF02F22018A72004B0FE9EF27D4BCD74E)       | 2023-06-07   | Yes         |                    34 |
| [Minotaur6](https://metrics.torproject.org/rs.html#details/66F4ABBF7DEC11993A45782BB552E6DF1416115A)    | 2023-06-10   | Yes         |                    34 |
| [Echidna3](https://metrics.torproject.org/rs.html#details/CB1816F95D43D6805230ED63326E88B0D4A7ABD7)     | 2023-04-28   | Yes         |                    32 |
| [Polyphemus2](https://metrics.torproject.org/rs.html#details/044428D910C037932A0763BB089769943F6BA648)  | 2022-10-19   | No          |                    34 |
| [Polyphemus](https://metrics.torproject.org/rs.html#details/0CABED9159F1E4BE82879F5A34ED8D7349E931BD)   | 2022-09-14   | No          |                    34 |
| [Polyphemus5](https://metrics.torproject.org/rs.html#details/0F3874C18BE50B83939D09AF2F6C362D1FC6C8CD)  | 2023-02-11   | No          |                    34 |
| [Chimera](https://metrics.torproject.org/rs.html#details/2946159CF9D8EAEB8C4A27F6A54B01A459DEE164)      | 2022-08-21   | No          |                    34 |
| [Polyphemus4](https://metrics.torproject.org/rs.html#details/41C106EAEB0B968C5E68927596500DC99B840367)  | 2023-02-11   | No          |                    34 |
| [Polyphemus8](https://metrics.torproject.org/rs.html#details/4D4B2695D6D02DFDCDE390ED5DF4A6798924CBBB)  | 2023-05-26   | No          |                    34 |
| [Chimera2](https://metrics.torproject.org/rs.html#details/4E60DE549B3B4C063E6035BCDAA69DD4F3AE3C4D)     | 2022-12-11   | No          |                    34 |
| [Polyphemus12](https://metrics.torproject.org/rs.html#details/55FFC2C4D01ACEAFE24C4089A615F91B616B865E) | 2023-07-09   | No          |                    34 |
| [Polyphemus9](https://metrics.torproject.org/rs.html#details/5B66B1C3023DFC4D579F7196D6D1663CA93BEC99)  | 2023-05-26   | No          |                    34 |
| [Polyphemus7](https://metrics.torproject.org/rs.html#details/6D7E1E64851F6FC3EB0143204C1EDEF992FAD947)  | 2023-05-26   | No          |                    34 |
| [Polyphemus3](https://metrics.torproject.org/rs.html#details/826C85481CCB8496EC3E67A4A477C24808D74011)  | 2022-11-05   | No          |                    34 |
| [Minotaur](https://metrics.torproject.org/rs.html#details/8BDBE498180C41249D3230FC5092CB3EB5A62482)     | 2021-04-06   | No          |                    34 |
| [Charybdis](https://metrics.torproject.org/rs.html#details/CBF59EC5B9FD108092AE9149EFDAE41F882DA669)    | 2022-08-19   | No          |                    34 |
| [Polyphemus6](https://metrics.torproject.org/rs.html#details/EDB75B4ED148C676B65A2631AC35682687F90BE7)  | 2023-02-11   | No          |                    34 |
| [Polyphemus11](https://metrics.torproject.org/rs.html#details/F3C86D3E09196BF2A80602A6B2398620610A54D1) | 2023-07-10   | No          |                    30 |
| [Polyphemus10](https://metrics.torproject.org/rs.html#details/F62DF7675006359605F699E23D18E52747012F1D) | 2023-07-10   | No          |                    30 |


## Fingerprint List of Guard-only Relays in E2E Groups

09F4736B37FA72AC7399F71F917F895D3CF22685,147CA31A3CD14F2EF7269BFDAE9A879E75295E2C,1DEECD906AFECF496B7DC1E40829F4563517B4CC,4B6A58C6E678F2B0F422D229F20284AB35194223,65369D044C659CD299E35763914FFD0FC9AD4509,66F4ABBF7DEC11993A45782BB552E6DF1416115A,6E586C8F62D0E153792095AFDA55D4E2E3F3421F,786835D15C33DCD2B7FD9E70CACBCDA3D6187300,8BF4E024210FF5DB1D7A4AFEBE11B48C73BFE779,961522CCF02F22018A72004B0FE9EF27D4BCD74E,A4789FA2F79E8EE39CFE3D272D6DBA599068EB28,A9A567CC15293CD3CD6B2BC12A435F37731843A2,B207494B6E471AB65C84891639D15F93750481E5,BA57222A0EC9ECDF003AED665DFB0B1287EA039D,C46548D44C0CA5855C175CE26F5817D38F833C9F,CB1816F95D43D6805230ED63326E88B0D4A7ABD7,EA05F22892CE6B556DD5F1733248A84AD883C116,FFA371808475B05A9544E4A4BA413B486B049E74