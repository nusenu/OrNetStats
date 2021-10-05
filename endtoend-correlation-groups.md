---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-10-05 18:00 UTC**

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


## ContactInfo: xKek Operations &lt;system@lysergic.dev&gt; (7) {#xkek-operations-systemlysergicdev}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [thetrip](https://metrics.torproject.org/rs.html#details/424F9C80A25843A2E60EDACCD3092D31D300FD74)  | 2021-06-10   | Yes         |                     7 |
| [cynthia](https://metrics.torproject.org/rs.html#details/519137667154E62261381ED5B912898E7DBDC60C)  | 2021-06-10   | Yes         |                     7 |
| [centauri](https://metrics.torproject.org/rs.html#details/BA45EB745D44E7FEA375AFF45A4C82C51E4C2B71) | 2021-06-10   | Yes         |                     7 |
| [cashew](https://metrics.torproject.org/rs.html#details/8063D1DCE54116090DD1B03E0D602E4AABE281F1)   | 2021-06-20   | No          |                     6 |
| [puddle](https://metrics.torproject.org/rs.html#details/9AF0C9EB3BDE62145DCE690CC82B9B8D79987E10)   | 2021-06-11   | No          |                     7 |
| [cuddle](https://metrics.torproject.org/rs.html#details/C1734E8C2D2DC1A579794DFA209C7CBCFA2B26F7)   | 2021-06-11   | No          |                     7 |
| [peanuts](https://metrics.torproject.org/rs.html#details/F62B74728AC72A495C986255199D9AF19CCA5B51)  | 2021-06-10   | No          |                     6 |

## ContactInfo: arkx &lt;tor-relays@rkx.se&gt; (3) {#arkx-tor-relaysrkxse}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [RkxTorRelay1](https://metrics.torproject.org/rs.html#details/BEE3A96D4C92B2253BD411BC355518399518C3F2) | 2021-07-06   | Yes         |                     1 |
| [RkxTorExit1](https://metrics.torproject.org/rs.html#details/1E0F9B3F63C8F333A0B9173D897837DF0BAF84C8)  | 2021-10-01   | No          |                     2 |
| [RkxTorExit1](https://metrics.torproject.org/rs.html#details/2F8DFD2824E32DA0F04A5D5F003566F2B4BA6F69)  | 2021-10-01   | No          |                     2 |

## ContactInfo: plithismostor@protonmail.com (9) {#plithismostorprotonmailcom}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [plithismos](https://metrics.torproject.org/rs.html#details/45047C78E1F5E7B775B0A42F118D4ED64504D09E) | 2021-06-19   | Yes         |                     9 |
| [plithismos](https://metrics.torproject.org/rs.html#details/4FCB8DDD2F59816949812525EACCD6B47091062A) | 2021-06-28   | Yes         |                     9 |
| [plithismos](https://metrics.torproject.org/rs.html#details/153042336222143D67BF3D03C92557F91B1AD86A) | 2021-09-23   | Yes         |                     1 |
| [plithismos](https://metrics.torproject.org/rs.html#details/1917535158147B554B49FA4B2245751C1EF21D2E) | 2021-07-06   | No          |                     9 |
| [plithismos](https://metrics.torproject.org/rs.html#details/4B1D53F25E019C211FC26BE2BB61612625CE2D44) | 2021-07-21   | No          |                     9 |
| [plithismos](https://metrics.torproject.org/rs.html#details/7798C99855EF1A08C64DF0497C97608F7062F112) | 2021-07-10   | No          |                     9 |
| [plithismos](https://metrics.torproject.org/rs.html#details/9FD8AF6546A248A4C7F07A79325496015D799195) | 2021-07-21   | No          |                     9 |
| [plithismos](https://metrics.torproject.org/rs.html#details/B3195576E1E6A8F342C312A2F0D1AFCAAF5A5EDF) | 2021-07-09   | No          |                     9 |
| [plithismos](https://metrics.torproject.org/rs.html#details/D3BAB67D1079EA080B83F158D69CA270FA44486B) | 2021-07-09   | No          |                     9 |


## Fingerprint List of Guard-only Relays in E2E Groups

424F9C80A25843A2E60EDACCD3092D31D300FD74,519137667154E62261381ED5B912898E7DBDC60C,BA45EB745D44E7FEA375AFF45A4C82C51E4C2B71,BEE3A96D4C92B2253BD411BC355518399518C3F2,153042336222143D67BF3D03C92557F91B1AD86A,45047C78E1F5E7B775B0A42F118D4ED64504D09E,4FCB8DDD2F59816949812525EACCD6B47091062A