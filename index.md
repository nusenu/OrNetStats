---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-02-26 16:00 UTC**

## Tor Relay Operators in End-to-End Correlation Position

The following table lists relay operators that are in a position to see a tor client's entry and exit connections.
In the **worst-case a tor client would use these groups as entry (guard) and exit relay at the same time.**

Operators are only listed if they actually have a chance to do end-to-end correlation attacks, that is:
* their guard **and** exit probability is > 0%
* they did **not** properly configure [MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily)
* they run in **more** than a single /16 network block

This list might contain false-positives as [ContactInfo](https://www.torproject.org/docs/tor-manual.html.en#ContactInfo) is not authenticated.

The ContactInfo is truncated. Middle-only relays are not included in per-group relaycounts.

The table is sorted by guard probability.

| Contact                                                                                                                        | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                           | 0.15        | 0.21       | 3         | 2               | 2016-08-28     | 1                           |
| [https://www.torservers.net/donate.html &lt;support .A](endtoend-correlation-groups#httpswwwtorserversnetdonatehtml-support-a) | 0.07        | 4.56       | 12        | 3               | 2018-02-19     | 1                           |
| [tor-mngr AT scalaire DOT fr](endtoend-correlation-groups#tor-mngr-at-scalaire-dot-fr)                                         | 0.01        | 0.31       | 2         | 2               | 2017-11-27     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                 | 0.01        | 0.24       | 7         | 2               | 2018-02-11     | 5                           |
| **Total**                                                                                                                      | **0.24**    | **5.32**   | **24**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Exit(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |     15.07 |        32 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      5.2  |        13 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |      3.31 |        11 | 2017-12-05   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.56 |         1 | 2014-04-19   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      2.53 |         7 | 2014-04-09   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.4  |         7 | 2013-07-10   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      2.36 |         6 | 2017-11-29   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9)    |      1.99 |        50 | 2016-08-22   |
| [John Doe johndoe@novogara.com](https://metrics.torproject.org/rs.html#details/0593F5255316748247EBA76353A3A61F62224903)                                  |      1.91 |         1 | 2017-09-05   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://metrics.torproject.org/rs.html#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      1.7  |         3 | 2014-11-04   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                  |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://metrics.torproject.org/rs.html#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9) |       1.84 |         4 | 2017-02-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799) |       1.79 |         7 | 2014-04-22   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                           |       1.56 |         5 | 2017-10-24   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)      |       1.18 |        17 | 2015-10-10   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                |       1.16 |         3 | 2015-04-22   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:71539D1911ECB826069A4D156771AC4F9F4632A7)        |       1.16 |         9 | 2018-01-07   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)   |       1.01 |         6 | 2016-08-10   |
| [11882BD0](https://metrics.torproject.org/rs.html#search/family:11882BD0A5A587FEE13465244EA8BCD4C7E03510)                                           |       0.9  |         3 | 2016-07-26   |
| [tor-relays@lists.torproject.org](https://metrics.torproject.org/rs.html#search/family:151BDD000832E22385680E456E4B94220317B122)                    |       0.86 |        10 | 2017-07-02   |
| [TotorBE AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:F3CEC87ED91E0B0B1D86BE4D7DE90F00B607ECAF)                           |       0.81 |         2 | 2016-10-22   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            4.227 |     15.07 |       0    |        32 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |            1.459 |      5.2  |       0    |        13 | 2016-12-23   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://metrics.torproject.org/rs.html#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)    |            1.321 |      1.11 |       1.84 |         8 | 2015-06-01   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.956 |      0    |       1.79 |         7 | 2014-04-22   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |            0.93  |      3.31 |       0    |        11 | 2017-12-05   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |            0.833 |      0    |       1.56 |         5 | 2017-10-24   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.763 |      2.36 |       0.18 |         8 | 2016-01-26   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.718 |      2.56 |       0    |         1 | 2014-04-19   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            0.711 |      2.53 |       0    |         7 | 2014-04-09   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)           |            0.679 |      2.4  |       0    |         8 | 2013-07-10   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            15.76 |      22.92 |      7.34 |       499 |
| Online S.a.s.               |             9.6  |      10.1  |     10.59 |       372 |
| Hetzner Online GmbH         |             6.37 |       8.89 |      1.93 |       273 |
| DigitalOcean, LLC           |             4.47 |       5.79 |      2.3  |       280 |
| Host Europe GmbH            |             2    |       3.51 |      0    |        32 |
| SOFTplus Entwicklungen GmbH |             1.7  |       0.39 |      5.32 |        19 |
| THC Projects SRL            |             1.39 |       2.37 |      0    |        17 |
| SURFnet bv                  |             1.19 |       1.75 |      0.9  |        10 |
| NForce Entertainment B.V.   |             1.16 |       0.08 |      3.85 |        19 |
| Hurricane Electric, Inc.    |             0.93 |       0.53 |      2.2  |        18 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             45.6 |     42.79 |      46.35 |      2256 |
| 0.3.1         |             16.8 |     13.35 |      18.72 |      1109 |
| 0.3.3         |             15.2 |     28.39 |      11.56 |       311 |
| 0.2.9         |             12.6 |      7.89 |      13.22 |      1148 |
| 0.2.5         |              4   |      2.81 |       4.91 |       473 |
| 0.3.0         |              2   |      0.98 |       2.48 |       226 |
| 0.2.4         |              1.2 |      0.84 |       1.28 |       256 |
| 0.2.7         |              1   |      0.17 |       1.07 |       204 |
| 0.3.4         |              0.9 |      2.69 |       0    |        15 |
| 0.2.8         |              0.2 |      0    |       0.3  |        34 |
| 0.2.6         |              0   |      0.02 |       0.07 |        34 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             4.45 |        4.9 |      2.03 |       720 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             89.6 |      90.7 |       87.1 |      5587 |
| BSD     |             10.1 |       9.2 |       12.6 |       316 |
| Windows |              0.1 |       0   |        0   |       115 |
| Darwin  |              0   |       0   |        0   |         9 |
| SunOS   |              0   |       0   |        0   |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            20.13 |      21.39 |       15.47 |      24.5 |       645 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     29.39 |            158 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1034 |
| None                                       |       576 |
| obfs3, obfs4, scramblesuit                 |       247 |
| obfs3, obfs4                               |        51 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        17 |
| obfs2, obfs3                               |        11 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| fte, obfs3, obfs4                          |         3 |
| meek                                       |         3 |
| scramblesuit                               |         3 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| fte, scramblesuit                          |         1 |
| meek, meek                                 |         1 |
| meek, obfs4                                |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

