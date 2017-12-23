---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-12-23 19:00 UTC**

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
| [https://www.torservers.net/donate.html &lt;support .A](endtoend-correlation-groups#httpswwwtorserversnetdonatehtml-support-a) | 0.07        | 4.72       | 11        | 3               | 2017-11-01     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                       | 0.05        | 0.03       | 3         | 3               | 2017-10-01     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                   | 0.04        | 0.29       | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                                      | **0.16**    | **5.04**   | **16**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                               |   Exit(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      8.85 |        21 | 2016-02-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      5.94 |        12 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      3.32 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |      3.1  |        11 | 2017-12-05   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9)    |      3.07 |        50 | 2016-08-22   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      2.39 |         6 | 2014-04-08   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      2.27 |         5 | 2014-04-09   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.24 |         3 | 2014-11-04   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.13 |         7 | 2013-07-10   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      2    |         6 | 2016-08-26   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                                 |       2.1  |         8 | 2016-07-26   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       1.61 |        16 | 2015-10-10   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       1.29 |         7 | 2016-08-10   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:951950A7993CF8A8E05174CF293BE4EA4DEFFF28)                                    |       1.09 |        17 | 2014-12-31   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       0.95 |         6 | 2014-04-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       0.88 |         7 | 2016-01-03   |
| [info omuravpn.com](https://atlas.torproject.org/#search/family:94C0F99BA44AA4A6767C71333B8A66DBD1BC08C7)                                        |       0.81 |         5 | 2017-01-05   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://atlas.torproject.org/#search/family:F596E1B1EF98E1DDBBDC934DB722AF54069868F6) |       0.69 |         6 | 2014-04-09   |
| [0x7A8647DB Daniel Winzen &lt;d@winzen4.de&gt; - 1CHvjeMJ](https://atlas.torproject.org/#search/family:72B19BAABE6846DF96EA2A50C28F4DC15A920041) |       0.6  |         5 | 2017-04-09   |
| [Random Person &lt;nobody AT example dot com&gt;](https://atlas.torproject.org/#details/85F277DFE886353598A51D3CAB04DD3F6EBB427D)                |       0.54 |         1 | 2017-12-09   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            2.171 |      8.85 |       0.18 |        25 | 2016-02-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |            1.399 |      5.94 |       0    |        12 | 2016-12-23   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            1.015 |      0    |       2.1  |         8 | 2016-07-26   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.82  |      0    |       1.61 |        19 | 2015-05-16   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.782 |      3.32 |       0    |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |            0.729 |      3.1  |       0    |        11 | 2017-12-05   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9) |            0.723 |      3.07 |       0    |        50 | 2016-08-22   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.698 |      0    |       0.95 |         7 | 2014-04-22   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |            0.672 |      0.21 |       1.29 |         8 | 2016-08-10   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.664 |      2    |       0.22 |         9 | 2016-01-26   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            15.1  |      15.26 |      6.57 |       506 |
| Online S.a.s.               |            11.01 |      13.15 |     11.99 |       405 |
| Hetzner Online GmbH         |             7.81 |       9.13 |      2.07 |       295 |
| DigitalOcean, LLC           |             4.44 |       5.69 |      1.5  |       298 |
| Host Europe GmbH            |             2.98 |       3.96 |      0    |        48 |
| myLoc managed IT AG         |             1.46 |       2.35 |      0.46 |        42 |
| THC Projects SRL            |             1.41 |       2.92 |      0    |        20 |
| SURFnet bv                  |             1.26 |       0.28 |      1.05 |        12 |
| SOFTplus Entwicklungen GmbH |             1.21 |       0.05 |      4.83 |        18 |
| ISPpro Internet KG          |             0.97 |       1.7  |      0    |        30 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             54.5 |     51.71 |      55.56 |      2839 |
| 0.2.9         |             15.3 |     10.8  |      15.74 |      1294 |
| 0.3.2         |             10.4 |     24.54 |       7.81 |       323 |
| 0.3.0         |              9.1 |      5.76 |       9.21 |       493 |
| 0.2.5         |              5.2 |      3.93 |       6.45 |       598 |
| 0.2.7         |              1.9 |      0.41 |       2.3  |       293 |
| 0.2.4         |              1.3 |      0.23 |       1.59 |       322 |
| 0.3.3         |              0.9 |      2.28 |       0.22 |        15 |
| 0.2.8         |              0.6 |      0.26 |       0.66 |        81 |
| 0.2.6         |              0.2 |      0.03 |       0.42 |        53 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.56 |       4.32 |      0.68 |       668 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.6 |      90   |       93   |      5836 |
| BSD     |              7.9 |       9.9 |        6.5 |       291 |
| SunOS   |              0.1 |       0   |        0.3 |         4 |
| Windows |              0.1 |       0   |        0   |       143 |
| Darwin  |              0   |       0   |        0   |        12 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.67 |      19.27 |       13.06 |     26.83 |       588 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     32.25 |            135 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1184 |
| None                                       |       600 |
| obfs3, obfs4, scramblesuit                 |       191 |
| obfs3, obfs4                               |        63 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        19 |
| obfs2, obfs3                               |         9 |
| obfs3, scramblesuit                        |         9 |
| obfs2, obfs3, obfs4                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| fte, obfs3, obfs4                          |         4 |
| obfs2, obfs3, obfs4, scramblesuit          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| meek                                       |         1 |
| meek, obfs4                                |         1 |
| scramblesuit                               |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

