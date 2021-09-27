---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-09-27 16:00 UTC**

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


## ContactInfo: Hurdy-Gurdy &lt;admin AT my-mail dot rocks&gt; (5) {#hurdy-gurdy-admin-at-my-mail-dot-rocks}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [0x90](https://metrics.torproject.org/rs.html#details/EF25C1F9BEF8C4A3F2859493C7C8C5148725B4E7)       | 2021-09-07   | Yes         |                     5 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/42A955B09A4E327FBFB46A08F6E21705271CCA12) | 2021-08-21   | Yes         |                     5 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/2189732AB3D2DFEB8B42AC1889C08626A6E56A1D) | 2021-08-21   | Yes         |                     1 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/9E195D72D11644A3C1D620463405335905584B40) | 2021-06-29   | No          |                     5 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/D1B853ED27E4DFDCA3A54D3F2E269C4D94677F66) | 2018-04-16   | No          |                     5 |

## ContactInfo: 4punk7 AT mailbox dot org (5) {#4punk7-at-mailbox-dot-org}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [4punk7r1](https://metrics.torproject.org/rs.html#details/ABA31795BAD2AB8097F3AD0FE1A920E518D3D3F3) | 2020-04-02   | Yes         |                     1 |
| [4punk7r2](https://metrics.torproject.org/rs.html#details/CB2DBDB2D9422D57AD85148EF9511AF4CE4D6052) | 2020-04-04   | Yes         |                     1 |
| [4punk7e1](https://metrics.torproject.org/rs.html#details/2E0C69E59B5B6AA15BB1C269690722607663416C) | 2020-11-27   | No          |                     1 |
| [4punk7e2](https://metrics.torproject.org/rs.html#details/68057FD302B0F83C0ED00B6D70FDAD6BEEF2005B) | 2020-10-21   | No          |                     1 |
| [4punk7e3](https://metrics.torproject.org/rs.html#details/F42FF0E095F23AD253622272F984649DDEEB402C) | 2020-10-26   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

2189732AB3D2DFEB8B42AC1889C08626A6E56A1D,42A955B09A4E327FBFB46A08F6E21705271CCA12,ABA31795BAD2AB8097F3AD0FE1A920E518D3D3F3,EF25C1F9BEF8C4A3F2859493C7C8C5148725B4E7,CB2DBDB2D9422D57AD85148EF9511AF4CE4D6052