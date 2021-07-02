---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-07-02 15:00 UTC**

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
| [cynthia](https://metrics.torproject.org/rs.html#details/519137667154E62261381ED5B912898E7DBDC60C)  | 2021-06-10   | Yes         |                     7 |
| [thetrip](https://metrics.torproject.org/rs.html#details/424F9C80A25843A2E60EDACCD3092D31D300FD74)  | 2021-06-10   | Yes         |                     7 |
| [centauri](https://metrics.torproject.org/rs.html#details/BA45EB745D44E7FEA375AFF45A4C82C51E4C2B71) | 2021-06-10   | Yes         |                     6 |
| [cashew](https://metrics.torproject.org/rs.html#details/8063D1DCE54116090DD1B03E0D602E4AABE281F1)   | 2021-06-20   | No          |                     1 |
| [puddle](https://metrics.torproject.org/rs.html#details/9AF0C9EB3BDE62145DCE690CC82B9B8D79987E10)   | 2021-06-11   | No          |                     6 |
| [cuddle](https://metrics.torproject.org/rs.html#details/C1734E8C2D2DC1A579794DFA209C7CBCFA2B26F7)   | 2021-06-11   | No          |                     7 |
| [peanuts](https://metrics.torproject.org/rs.html#details/F62B74728AC72A495C986255199D9AF19CCA5B51)  | 2021-06-10   | No          |                     7 |

## ContactInfo: 4punk7 AT mailbox dot org (4) {#4punk7-at-mailbox-dot-org}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [4punk7r2](https://metrics.torproject.org/rs.html#details/CB2DBDB2D9422D57AD85148EF9511AF4CE4D6052) | 2020-04-04   | Yes         |                     1 |
| [4punk7e1](https://metrics.torproject.org/rs.html#details/2E0C69E59B5B6AA15BB1C269690722607663416C) | 2020-11-27   | No          |                     1 |
| [4punk7e2](https://metrics.torproject.org/rs.html#details/68057FD302B0F83C0ED00B6D70FDAD6BEEF2005B) | 2020-10-21   | No          |                     1 |
| [4punk7e3](https://metrics.torproject.org/rs.html#details/F42FF0E095F23AD253622272F984649DDEEB402C) | 2020-10-26   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

424F9C80A25843A2E60EDACCD3092D31D300FD74,519137667154E62261381ED5B912898E7DBDC60C,BA45EB745D44E7FEA375AFF45A4C82C51E4C2B71,CB2DBDB2D9422D57AD85148EF9511AF4CE4D6052