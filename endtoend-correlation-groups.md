---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-01-19 14:00 UTC**

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


## ContactInfo: &lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq (21) {#zwiebeln-at-online-de-please-donate-btc-1k38x9xq}

| Nickname                                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [GaoZhisheng](https://metrics.torproject.org/rs.html#details/23B3EF4271E38A744E23ACC4345E56CBDB42A1A5)         | 2019-12-12   | Yes         |                     1 |
| [LuXun](https://metrics.torproject.org/rs.html#details/693A982584CF4DD7BF2158B640CCF9A75A87B1BD)               | 2019-12-12   | Yes         |                     1 |
| [LiuXiaobo](https://metrics.torproject.org/rs.html#details/1617A702B30320C37A5C9FA3CFB737A2AFA9198D)           | 2019-11-26   | No          |                    15 |
| [TahirElci](https://metrics.torproject.org/rs.html#details/3246ECCAEDC4FF2949B655E0245AFFF42F8C9DFC)           | 2016-11-12   | No          |                    15 |
| [Hecker](https://metrics.torproject.org/rs.html#details/348439F4A3D959E6D1481070DA81A135343419CB)              | 2019-12-01   | No          |                    15 |
| [LechWalesa](https://metrics.torproject.org/rs.html#details/364E18848469385C5948376FAF778AC61D4CFB67)          | 2019-11-29   | No          |                    15 |
| [weirenminfuwu](https://metrics.torproject.org/rs.html#details/53FF1EDC8528AF4238FB7501831E6BACFF4B42D2)       | 2019-11-26   | No          |                    15 |
| [SimonBolivar](https://metrics.torproject.org/rs.html#details/69ECFB731C2B0AA7B4D8746EF3504ADCB1F0A556)        | 2019-11-29   | No          |                    15 |
| [SebnemKorurFincanci](https://metrics.torproject.org/rs.html#details/74FB777F25E7F80BA6BF8B808DF873A1708821A7) | 2016-12-18   | No          |                    15 |
| [Politkowskaja](https://metrics.torproject.org/rs.html#details/777B2DECD67C607D8857AD60E976EE3E1E8A52BF)       | 2016-11-15   | No          |                    15 |
| [MartinLutherKing](https://metrics.torproject.org/rs.html#details/78DF2B937849E6B7636E901377DB08A15B51525C)    | 2020-01-10   | No          |                     1 |
| [Freiheit](https://metrics.torproject.org/rs.html#details/8B496F3EF3BF5CC32A4C20ECDBEC2A06E7EA4357)            | 2020-01-06   | No          |                     1 |
| [JanKuciak](https://metrics.torproject.org/rs.html#details/9C1559C46AD0279EEF6FD187E1B27D939C303086)           | 2020-01-06   | No          |                     1 |
| [ShirinEbadi](https://metrics.torproject.org/rs.html#details/A926970FE1AEF9C6D8D4BF57ED6B88F3F8C66415)         | 2019-11-28   | No          |                    15 |
| [DaphneCaruana](https://metrics.torproject.org/rs.html#details/B22169DDB936E4CF4B8C81E9514BD05658466974)       | 2019-11-28   | No          |                    15 |
| [BadshahKhan](https://metrics.torproject.org/rs.html#details/B56D5A0543C35B45D81D792A4735590E3612A815)         | 2016-12-18   | No          |                    15 |
| [Marx](https://metrics.torproject.org/rs.html#details/BCB6AC303A69A7E87BB2D6F3F13A0C0F0A6C938E)                | 2019-11-26   | No          |                    15 |
| [Brecht](https://metrics.torproject.org/rs.html#details/E00C087ECFB27D7BF969936F1FDD9354E03CAE2F)              | 2020-01-10   | No          |                     1 |
| [Sacharow](https://metrics.torproject.org/rs.html#details/E79A58AF0DB93B90F97B48963CC4729E4CFA43C5)            | 2019-11-26   | No          |                    15 |
| [Mandela](https://metrics.torproject.org/rs.html#details/F1F9D1DBD7E56F99C61C3712D5F4A02153FD9AD4)             | 2019-11-26   | No          |                    15 |
| [Gandhi](https://metrics.torproject.org/rs.html#details/F2AF93D23D91F9CFE03C5151DF01B0481BF99E12)              | 2019-11-28   | No          |                    15 |


## Fingerprint List of Guard-only Relays in E2E Groups

23B3EF4271E38A744E23ACC4345E56CBDB42A1A5,693A982584CF4DD7BF2158B640CCF9A75A87B1BD