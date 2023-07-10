---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-07-10 16:00 UTC**

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


## ContactInfo: Brandon Kuschel &lt;kusch023 AT NOSPAM umn dot edu&gt; (32) {#brandon-kuschel-kusch023-at-nospam-umn-dot-edu}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Lamia2](https://metrics.torproject.org/rs.html#details/786835D15C33DCD2B7FD9E70CACBCDA3D6187300)       | 2022-12-11   | Yes         |                    34 |
| [Lamia](https://metrics.torproject.org/rs.html#details/C46548D44C0CA5855C175CE26F5817D38F833C9F)        | 2022-08-21   | Yes         |                    34 |
| [Charybdis2](https://metrics.torproject.org/rs.html#details/1DEECD906AFECF496B7DC1E40829F4563517B4CC)   | 2022-09-19   | Yes         |                    34 |
| [Charybdis3](https://metrics.torproject.org/rs.html#details/8BF4E024210FF5DB1D7A4AFEBE11B48C73BFE779)   | 2023-02-11   | Yes         |                    34 |
| [Lamia3](https://metrics.torproject.org/rs.html#details/09F4736B37FA72AC7399F71F917F895D3CF22685)       | 2023-04-28   | Yes         |                    34 |
| [Minotaur3](https://metrics.torproject.org/rs.html#details/147CA31A3CD14F2EF7269BFDAE9A879E75295E2C)    | 2022-10-17   | Yes         |                    34 |
| [Echidna](https://metrics.torproject.org/rs.html#details/BA57222A0EC9ECDF003AED665DFB0B1287EA039D)      | 2022-08-21   | Yes         |                    32 |
| [Minotaur2](https://metrics.torproject.org/rs.html#details/6E586C8F62D0E153792095AFDA55D4E2E3F3421F)    | 2022-09-19   | Yes         |                    34 |
| [Echidna2](https://metrics.torproject.org/rs.html#details/EA05F22892CE6B556DD5F1733248A84AD883C116)     | 2022-12-11   | Yes         |                    32 |
| [Minotaur4](https://metrics.torproject.org/rs.html#details/FFA371808475B05A9544E4A4BA413B486B049E74)    | 2023-02-11   | Yes         |                    34 |
| [Minotaur7](https://metrics.torproject.org/rs.html#details/B207494B6E471AB65C84891639D15F93750481E5)    | 2023-06-10   | Yes         |                    34 |
| [Echidna3](https://metrics.torproject.org/rs.html#details/CB1816F95D43D6805230ED63326E88B0D4A7ABD7)     | 2023-04-28   | Yes         |                    32 |
| [Minotaur5](https://metrics.torproject.org/rs.html#details/A4789FA2F79E8EE39CFE3D272D6DBA599068EB28)    | 2023-02-11   | Yes         |                    34 |
| [Lamia4](https://metrics.torproject.org/rs.html#details/961522CCF02F22018A72004B0FE9EF27D4BCD74E)       | 2023-06-07   | Yes         |                    34 |
| [Minotaur6](https://metrics.torproject.org/rs.html#details/66F4ABBF7DEC11993A45782BB552E6DF1416115A)    | 2023-06-10   | Yes         |                    34 |
| [Echidna4](https://metrics.torproject.org/rs.html#details/A9A567CC15293CD3CD6B2BC12A435F37731843A2)     | 2023-06-07   | Yes         |                    32 |
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

## ContactInfo: email:abuse artikel5ev.de url:https://artikel5ev. (30) {#emailabuseartikel5evde-urlhttpsartikel5ev}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [dc6jgk12c](https://metrics.torproject.org/rs.html#details/BFC6E7F298D581344DFCE95BB7EE9EDE1FC0745B)     | 2020-08-28   | Yes         |                    36 |
| [dc6jgk13b](https://metrics.torproject.org/rs.html#details/571BE7435DC9D660BB5EE0A37650E2421007BAEC)     | 2022-05-13   | Yes         |                    34 |
| [enceladus01](https://metrics.torproject.org/rs.html#details/4B170481AC4C3EC3603B9F4443C2E24B929D0429)   | 2020-12-02   | Yes         |                    29 |
| [dc6jgk11c](https://metrics.torproject.org/rs.html#details/7B700C0C207EBD0002E00F499BE265519AC3C25A)     | 2016-11-11   | Yes         |                    36 |
| [dc6jgk11d](https://metrics.torproject.org/rs.html#details/0040A5B04C7E309D37CBE7EDB2B72D3E15D057C1)     | 2022-05-13   | Yes         |                    35 |
| [dc6jgk12d](https://metrics.torproject.org/rs.html#details/4C25542B7649FC0472EDBF77521EA578F9AF5155)     | 2022-05-13   | Yes         |                    35 |
| [dc6jgk13](https://metrics.torproject.org/rs.html#details/E6D4332BF40FDEE7814F2DBC926650EF8032B643)      | 2020-08-28   | Yes         |                    35 |
| [dc6jgk7c](https://metrics.torproject.org/rs.html#details/F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A)      | 2016-11-04   | Yes         |                    35 |
| [artikel5ev7](https://metrics.torproject.org/rs.html#details/22404A3E87F2D7FE2FC6359FDE71B6DC2D6E730F)   | 2017-08-30   | Yes         |                    35 |
| [artikel5ev1](https://metrics.torproject.org/rs.html#details/0BC8BA32CC3CB0F598E0C92778F7C0946DFBCE91)   | 2016-10-19   | No          |                    35 |
| [artikel5ev1b](https://metrics.torproject.org/rs.html#details/166264168E8CCCBB2444ADE0F0A22E4E6DDEF6FD)  | 2022-05-13   | No          |                    34 |
| [artikel5ev3b](https://metrics.torproject.org/rs.html#details/195712E96FD1C1B18D14D09E9E4E7A6416E23B2C)  | 2017-12-05   | No          |                    35 |
| [artikel5ev2b](https://metrics.torproject.org/rs.html#details/1AA683E036EA10AA6E078D40498CC7234F6424B9)  | 2022-05-13   | No          |                    34 |
| [artikel5ev4](https://metrics.torproject.org/rs.html#details/26C28F29B611DF4DE23ACF5D9DC1EB4895EF5E8B)   | 2019-01-25   | No          |                    35 |
| [artikel5ev10b](https://metrics.torproject.org/rs.html#details/282CAAF0E11DAD47DD73D553DC20B51099A257BB) | 2022-05-13   | No          |                    34 |
| [artikel5ev8](https://metrics.torproject.org/rs.html#details/4D0DF468DC816F8096702C2DA2C6FD67561F81C8)   | 2019-12-29   | No          |                    35 |
| [artikel5ev13c](https://metrics.torproject.org/rs.html#details/51562252B9CF3120FAC9CF124391697296050E74) | 2023-07-08   | No          |                     1 |
| [artikel5ev12](https://metrics.torproject.org/rs.html#details/780D50DCCD7F3C831E5E750F41866497C1263F76)  | 2020-09-08   | No          |                    35 |
| [artikel5ev12d](https://metrics.torproject.org/rs.html#details/88C8F99559FEEB7C29E2EB196AACD734390D6289) | 2023-07-08   | No          |                     1 |
| [artikel5ev13](https://metrics.torproject.org/rs.html#details/89C7E852CC2FA537ED78775ADC3BEA24672B4154)  | 2020-09-07   | No          |                    36 |
| [artikel5ev12c](https://metrics.torproject.org/rs.html#details/9DEB16841863A939257160445052C606ECA46D25) | 2023-07-08   | No          |                     1 |
| [artikel5ev10](https://metrics.torproject.org/rs.html#details/AF7094B62864DE941DCD88A2F0DBAFECF3997E47)  | 2020-04-12   | No          |                    35 |
| [artikel5ev13b](https://metrics.torproject.org/rs.html#details/B1F926DA3895A89AF288623F5A4F913979299C53) | 2022-05-13   | No          |                    35 |
| [artikel5ev3c](https://metrics.torproject.org/rs.html#details/C36C76992198329C0D8F34E01D092BF2ACE0B6B0)  | 2022-05-13   | No          |                    34 |
| [artikel5ev12b](https://metrics.torproject.org/rs.html#details/CE5EF4FB644544DB2F430A60CC6EB86FD7E29BA6) | 2022-05-13   | No          |                    34 |
| [artikel5ev8b](https://metrics.torproject.org/rs.html#details/D4CA7FD04DABF6E2CB679426F5AA3205B640D147)  | 2022-05-13   | No          |                    34 |
| [artikel5ev2](https://metrics.torproject.org/rs.html#details/DC2191663DD4BAECB34F949CCAC3FDA004CE5BCE)   | 2016-10-29   | No          |                    35 |
| [artikel5ev9b](https://metrics.torproject.org/rs.html#details/E22694E83DA7BCF30DDAF5780EEF394CD0370CC4)  | 2022-05-13   | No          |                    34 |
| [artikel5ev4b](https://metrics.torproject.org/rs.html#details/F3B2CC8C2AB331150E096DD1DB8810E4A43F399D)  | 2022-05-13   | No          |                    34 |
| [artikel5ev9](https://metrics.torproject.org/rs.html#details/FC077C25B8DBB3132D397D7DF03C92BFC14C9D76)   | 2020-01-11   | No          |                    35 |


## Fingerprint List of Guard-only Relays in E2E Groups

09F4736B37FA72AC7399F71F917F895D3CF22685,147CA31A3CD14F2EF7269BFDAE9A879E75295E2C,1DEECD906AFECF496B7DC1E40829F4563517B4CC,66F4ABBF7DEC11993A45782BB552E6DF1416115A,6E586C8F62D0E153792095AFDA55D4E2E3F3421F,786835D15C33DCD2B7FD9E70CACBCDA3D6187300,8BF4E024210FF5DB1D7A4AFEBE11B48C73BFE779,961522CCF02F22018A72004B0FE9EF27D4BCD74E,A4789FA2F79E8EE39CFE3D272D6DBA599068EB28,A9A567CC15293CD3CD6B2BC12A435F37731843A2,B207494B6E471AB65C84891639D15F93750481E5,BA57222A0EC9ECDF003AED665DFB0B1287EA039D,C46548D44C0CA5855C175CE26F5817D38F833C9F,CB1816F95D43D6805230ED63326E88B0D4A7ABD7,0040A5B04C7E309D37CBE7EDB2B72D3E15D057C1,22404A3E87F2D7FE2FC6359FDE71B6DC2D6E730F,4B170481AC4C3EC3603B9F4443C2E24B929D0429,4C25542B7649FC0472EDBF77521EA578F9AF5155,571BE7435DC9D660BB5EE0A37650E2421007BAEC,7B700C0C207EBD0002E00F499BE265519AC3C25A,BFC6E7F298D581344DFCE95BB7EE9EDE1FC0745B,EA05F22892CE6B556DD5F1733248A84AD883C116,FFA371808475B05A9544E4A4BA413B486B049E74,E6D4332BF40FDEE7814F2DBC926650EF8032B643,F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A