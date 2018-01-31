---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-01-31 07:00 UTC**

For each operator the list of running relays is shown (relays are linked to [Atlas](https://atlas.torproject.org)).
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


## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://atlas.torproject.org/#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://atlas.torproject.org/#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://atlas.torproject.org/#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: - (2) {#-}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [chrissrelay](https://atlas.torproject.org/#details/55C95AC7FB3005DDDC73FECD9AB9D2CDA2986D78) | 2018-01-02   | Yes         |                     1 |
| [RainbowDash](https://atlas.torproject.org/#details/7FD90DB48DB568884DEA6EE3F89CF27250CF83A6) | 2017-12-30   | No          |                     1 |

## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv (3) {#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay1](https://atlas.torproject.org/#details/D31BFE2048AD5B77CA072E977B5961861A2415E6)     | 2018-01-21   | Yes         |                     1 |
| [NeelTorExitUSWest](https://atlas.torproject.org/#details/331243DA4C5EC6F4886F4E56EEFB5800300FDC57) | 2018-01-13   | No          |                     2 |
| [NeelTorExitUSEast](https://atlas.torproject.org/#details/76BD45BAC8CC057D0A6DE927711F3F378555D731) | 2018-01-06   | No          |                     2 |

## ContactInfo: AnonyMaid Team &lt;info@anonymaid.net&gt; (3) {#anonymaid-team-infoanonymaidnet}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [DutchDroid](https://atlas.torproject.org/#details/BF5068641A54A9433CA612BDFF7F098B72EB9762)  | 2017-08-09   | Yes         |                     1 |
| [DutchMaid04](https://atlas.torproject.org/#details/44182447E5E9F2997754CE53FFB4881942B5B3C6) | 2017-10-01   | No          |                     1 |
| [DutchMaid03](https://atlas.torproject.org/#details/7FAB8FED1A821455902BEA3388A6DA5BF6F78198) | 2017-10-01   | No          |                     1 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://atlas.torproject.org/#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://atlas.torproject.org/#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,BF5068641A54A9433CA612BDFF7F098B72EB9762,55C95AC7FB3005DDDC73FECD9AB9D2CDA2986D78,D31BFE2048AD5B77CA072E977B5961861A2415E6