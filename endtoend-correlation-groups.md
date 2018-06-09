---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-06-09 06:00 UTC**

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


## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://metrics.torproject.org/rs.html#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: zcashtorservers.org supported by a z.cash.foundati (7) {#zcashtorserversorg-supported-by-a-zcashfoundati}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [ZcashTor0se](https://metrics.torproject.org/rs.html#details/381DB186136F95370B0A7C7575E40B5DE8C18BDB) | 2017-03-14   | Yes         |                    10 |
| [ZcashTor0lv](https://metrics.torproject.org/rs.html#details/53825DFB32426F4D02E2FAA43AF713DC185299F4) | 2017-03-14   | Yes         |                    10 |
| [ZcashTor0nl](https://metrics.torproject.org/rs.html#details/6B23021CB4B4FE6525D23BE8E6BA4F91EAAB0741) | 2018-01-31   | No          |                    10 |
| [ZcashTor1nl](https://metrics.torproject.org/rs.html#details/6E89911A8045A577C53BC06D539F6AD5340391D4) | 2018-01-31   | No          |                    10 |
| [ZcashTor0ca](https://metrics.torproject.org/rs.html#details/800C0EBDF0C7B4A7950D445435706CD9B901C47B) | 2018-05-10   | No          |                     1 |
| [ZcashTor3nl](https://metrics.torproject.org/rs.html#details/B5A68709FF46B730CCA37D98CA477C4B9FF9296D) | 2018-01-31   | No          |                    10 |
| [ZcashTor2nl](https://metrics.torproject.org/rs.html#details/DB3B3FBD826C80E24C45043044AD33489012920F) | 2018-01-31   | No          |                    10 |

## ContactInfo: Person admin@example.com (2) {#person-adminexamplecom}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [whitegods](https://metrics.torproject.org/rs.html#details/28165E00A07D6C3A8F5245A0C1109205B625CFC8)     | 2018-04-24   | Yes         |                     1 |
| [nodeexitwhite](https://metrics.torproject.org/rs.html#details/E17023BCBD6E8656EC8CAAF56EBB4F638F1E49B2) | 2018-05-20   | No          |                     1 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://metrics.torproject.org/rs.html#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://metrics.torproject.org/rs.html#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |

## ContactInfo: DuckSounds31@aol.com (3) {#ducksounds31aolcom}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [DuckYou](https://metrics.torproject.org/rs.html#details/AF4997738E0CFC014CD04FB09A670D2C5F1E79A4)    | 2018-03-02   | Yes         |                     1 |
| [QuackQuack](https://metrics.torproject.org/rs.html#details/1EE15139F389FDA24400239607CB4C0BE5DD8C76) | 2018-01-31   | No          |                     2 |
| [FlappyBird](https://metrics.torproject.org/rs.html#details/B00478C4CD2F3ACC7D6F02AF8033D2906673651F) | 2018-02-01   | No          |                     2 |


## Fingerprint List of Guard-only Relays in E2E Groups

28165E00A07D6C3A8F5245A0C1109205B625CFC8,381DB186136F95370B0A7C7575E40B5DE8C18BDB,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,AF4997738E0CFC014CD04FB09A670D2C5F1E79A4,C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7