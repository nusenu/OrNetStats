---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-02-25 20:00 UTC**

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
If someone else is using your contactInfo please send an email to bad-relays AT lists DOT torproject DOT org.


## ContactInfo: Kevin Hicks &lt;admin@fissionrelays.net&gt; (8) {#kevin-hicks-adminfissionrelaysnet}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [FissionEx3](https://metrics.torproject.org/rs.html#details/4FDDFAD51B24DDABB62FB59071F4DC421E76C685)    | 2018-10-15   | Yes         |                    17 |
| [FissionEx4](https://metrics.torproject.org/rs.html#details/3B4C5729F829CA2E895B81AF834A63DB336D0FFE)    | 2019-02-03   | Yes         |                    17 |
| [FissionEx1](https://metrics.torproject.org/rs.html#details/ECB24A326D382F84B7BD630CFDBE1A0CDCE0245A)    | 2019-07-30   | Yes         |                    17 |
| [FissionEx2](https://metrics.torproject.org/rs.html#details/460E5B882770C19761BC5747541913DB2AD01E35)    | 2018-07-08   | No          |                    17 |
| [FissionMasq01](https://metrics.torproject.org/rs.html#details/4A411DD8EBBD539AA0090A305856B9C838F7F2D6) | 2020-01-12   | No          |                    17 |
| [FissionMasq02](https://metrics.torproject.org/rs.html#details/5FA7596FB2BA2C889337F8B82DD7127BBB240D4D) | 2020-02-25   | No          |                     1 |
| [FissionMasq04](https://metrics.torproject.org/rs.html#details/7533ABDA9027F40CF87FB6189AEBB1F43A132A0B) | 2020-02-25   | No          |                     1 |
| [FissionMasq03](https://metrics.torproject.org/rs.html#details/8628D2ACCA1C9BE596DED1DF9D0099BBDB1352B3) | 2020-02-25   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (2) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4) | 2019-10-25   | Yes         |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/71840F45C2478347B872321066F9805D1A1B79FD)  | 2019-10-25   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

3B4C5729F829CA2E895B81AF834A63DB336D0FFE,4FDDFAD51B24DDABB62FB59071F4DC421E76C685,DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4,ECB24A326D382F84B7BD630CFDBE1A0CDCE0245A