---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-07-21 06:00 UTC**

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


## ContactInfo: Cheena &lt;cheena @ cheena . net&gt; (4) {#cheena-cheena--cheena--net}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CheenaTorRelay](https://metrics.torproject.org/rs.html#details/734644A4BC767464320B215A4DC68AB522ED912D)  | 2017-12-31   | Yes         |                     3 |
| [CheenaTorRelay3](https://metrics.torproject.org/rs.html#details/C3BC6B7E4E54AAEDDC79DB74E7D208E1D3C49CC3) | 2017-04-18   | Yes         |                     1 |
| [CheenaTorRelay2](https://metrics.torproject.org/rs.html#details/98D3C5BC8D2032588B6FB3297539814B59DBE94A) | 2018-06-14   | Yes         |                     3 |
| [CheenaTorExit](https://metrics.torproject.org/rs.html#details/50BD3C2C70050A999BD423EB23CDAE21F2214E02)   | 2017-02-20   | No          |                     3 |

## ContactInfo: tor at releasing dot fun (3) {#toratreleasingdotfun}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [releasingFun04](https://metrics.torproject.org/rs.html#details/E91FC7ABF7708A584FCFE88DB5CEA083D00E6511) | 2018-07-04   | Yes         |                     1 |
| [releasingFun02](https://metrics.torproject.org/rs.html#details/B26F12939CE5FE0D21E70429DDB51DDA3DB4CACF) | 2018-07-03   | No          |                     3 |
| [releasingFun01](https://metrics.torproject.org/rs.html#details/D826AF785186EF68DA329D2B005167967EB7F758) | 2018-07-02   | No          |                     3 |

## ContactInfo: DuckSounds31@aol.com (3) {#ducksounds31aolcom}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [DuckYou](https://metrics.torproject.org/rs.html#details/AF4997738E0CFC014CD04FB09A670D2C5F1E79A4)    | 2018-03-02   | Yes         |                     1 |
| [QuackQuack](https://metrics.torproject.org/rs.html#details/1EE15139F389FDA24400239607CB4C0BE5DD8C76) | 2018-01-31   | No          |                     2 |
| [FlappyBird](https://metrics.torproject.org/rs.html#details/B00478C4CD2F3ACC7D6F02AF8033D2906673651F) | 2018-02-01   | No          |                     2 |


## Fingerprint List of Guard-only Relays in E2E Groups

734644A4BC767464320B215A4DC68AB522ED912D,98D3C5BC8D2032588B6FB3297539814B59DBE94A,AF4997738E0CFC014CD04FB09A670D2C5F1E79A4,C3BC6B7E4E54AAEDDC79DB74E7D208E1D3C49CC3,E91FC7ABF7708A584FCFE88DB5CEA083D00E6511