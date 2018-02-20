---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-02-20 06:00 UTC**

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
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                           | 0.1         | 0.23       | 3         | 2               | 2016-08-28     | 1                           |
| [https://www.torservers.net/donate.html &lt;support .A](endtoend-correlation-groups#httpswwwtorserversnetdonatehtml-support-a) | 0.09        | 4.17       | 12        | 3               | 2018-02-19     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                   | 0.01        | 0.25       | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                                      | **0.20**    | **4.65**   | **17**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |     14.81 |        32 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      4.86 |        13 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |      3.26 |        11 | 2017-12-05   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      2.91 |         6 | 2017-11-29   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.62 |         1 | 2014-04-19   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.61 |         7 | 2013-07-10   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      2.26 |         7 | 2014-04-09   |
| [John Doe johndoe@novogara.com](https://metrics.torproject.org/rs.html#details/0593F5255316748247EBA76353A3A61F62224903)                                  |      2.18 |         1 | 2017-09-05   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://metrics.torproject.org/rs.html#search/family:A10C4F666D27364036B562823E5830BC448E046A) |      1.98 |         5 | 2011-10-06   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      1.85 |         6 | 2014-04-08   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                  |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799) |       1.75 |         7 | 2014-04-22   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                           |       1.72 |         5 | 2017-10-24   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)   |       1.28 |         6 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)      |       1.18 |        17 | 2015-10-10   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                |       1.01 |         3 | 2015-04-22   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://metrics.torproject.org/rs.html#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9) |       1.01 |         3 | 2017-02-25   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:71539D1911ECB826069A4D156771AC4F9F4632A7)        |       0.99 |         9 | 2018-01-07   |
| [6FF440DF](https://metrics.torproject.org/rs.html#details/6FF440DFB1D0697B942357D747900CC308DD57CC)                                                 |       0.79 |         1 | 2017-10-27   |
| [TotorBE AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:F3CEC87ED91E0B0B1D86BE4D7DE90F00B607ECAF)                           |       0.72 |         2 | 2016-10-22   |
| [tor-relays@lists.torproject.org](https://metrics.torproject.org/rs.html#search/family:151BDD000832E22385680E456E4B94220317B122)                    |       0.72 |        10 | 2017-07-02   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            3.935 |     14.81 |       0    |        32 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |            1.292 |      4.86 |       0    |        13 | 2016-12-23   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://metrics.torproject.org/rs.html#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)    |            1.123 |      1.09 |       1.01 |         8 | 2015-06-01   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.932 |      0    |       1.75 |         7 | 2014-04-22   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |            0.92  |      0    |       1.72 |         5 | 2017-10-24   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.91  |      2.91 |       0.25 |         8 | 2016-01-26   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |            0.868 |      3.26 |       0    |        11 | 2017-12-05   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |            0.724 |      0.15 |       1.28 |         7 | 2016-08-10   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)           |            0.706 |      2.61 |       0.02 |         8 | 2013-07-10   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.696 |      2.62 |       0    |         1 | 2014-04-19   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            15.39 |      21.37 |      7.71 |       512 |
| Online S.a.s.               |            10.22 |      10.36 |     11.04 |       373 |
| Hetzner Online GmbH         |             6.78 |       9.3  |      1.89 |       285 |
| DigitalOcean, LLC           |             4.84 |       5.85 |      1.98 |       298 |
| Host Europe GmbH            |             2.27 |       3.9  |      0    |        35 |
| SOFTplus Entwicklungen GmbH |             1.6  |       0.27 |      5.38 |        19 |
| THC Projects SRL            |             1.22 |       2    |      0    |        17 |
| SURFnet bv                  |             1.11 |       1.61 |      0.9  |        11 |
| Voxility S.R.L.             |             1.03 |       0.2  |      2.99 |        14 |
| NForce Entertainment B.V.   |             0.98 |       0.02 |      3.38 |        18 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             44.8 |     44.55 |      44.67 |      2245 |
| 0.3.1         |             19.3 |     13.79 |      21.99 |      1106 |
| 0.3.3         |             13.4 |     25.98 |      10.23 |       245 |
| 0.2.9         |             12.8 |      9.19 |      13.07 |      1149 |
| 0.2.5         |              4.2 |      2.94 |       4.74 |       489 |
| 0.3.0         |              1.9 |      1.12 |       1.98 |       245 |
| 0.2.4         |              1.4 |      1.03 |       1.52 |       233 |
| 0.2.7         |              1.1 |      0.18 |       1.12 |       209 |
| 0.3.4         |              0.4 |      0.91 |       0.31 |         7 |
| 0.2.8         |              0.2 |      0.2  |       0.26 |        39 |
| 0.2.6         |              0   |      0.03 |       0.07 |        32 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             4.59 |       4.71 |      2.37 |       719 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.2 |      90.1 |       88.5 |      5579 |
| BSD     |              9.5 |       9.6 |       11.3 |       296 |
| Windows |              0.1 |       0   |        0   |        93 |
| Darwin  |              0   |       0   |        0   |        14 |
| SunOS   |              0   |       0   |        0   |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            20.45 |      21.74 |       16.32 |     24.35 |       648 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     29.33 |            155 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1027 |
| None                                       |       586 |
| obfs3, obfs4, scramblesuit                 |       246 |
| obfs3, obfs4                               |        57 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        17 |
| obfs2, obfs3                               |        10 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         3 |
| scramblesuit                               |         3 |
| fte, obfs3, obfs4                          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| meek, meek                                 |         1 |
| meek, obfs4                                |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

