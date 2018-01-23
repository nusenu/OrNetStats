---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-01-23 07:00 UTC**

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

| Contact                                                                                                                                  | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-----------------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [abuse AT torworld.org - BTC 17iwdtpmgHdPt15twdT2](endtoend-correlation-groups#abuse-at-torworldorg---btc-17iwdtpmghdpt15twdt2)          | 0.16        | 0.85       | 8         | 6               | 2018-01-14     | 7                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                     | 0.12        | 0.19       | 3         | 2               | 2016-08-28     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-btc---14w) | 0.09        | 0.82       | 11        | 2               | 2016-04-01     | 4                           |
| [-](endtoend-correlation-groups#-)                                                                                                       | 0.07        | 0.25       | 2         | 2               | 2018-01-02     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                                 | 0.02        | 0.03       | 3         | 3               | 2017-10-01     | 1                           |
| [tor-mngr AT scalaire DOT fr](endtoend-correlation-groups#tor-mngr-at-scalaire-dot-fr)                                                   | 0.02        | 0.2        | 2         | 2               | 2017-11-27     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.01        | 0.26       | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                                                | **0.49**    | **2.60**   | **31**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |     11.7  |        33 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      6.02 |        12 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      3.32 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |      3.32 |        11 | 2017-12-05   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      2.87 |        11 | 2016-08-26   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      2.56 |         5 | 2014-04-09   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.22 |         7 | 2013-07-10   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.03 |         3 | 2014-11-04   |
| [John Doe johndoe@novogara.com](https://atlas.torproject.org/#details/0593F5255316748247EBA76353A3A61F62224903)                                  |      1.9  |         1 | 2017-09-05   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://atlas.torproject.org/#search/family:A10C4F666D27364036B562823E5830BC448E046A) |      1.9  |         5 | 2011-10-06   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       2.21 |         6 | 2014-04-22   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |       1.84 |         5 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       1.69 |        16 | 2015-10-10   |
| [poiuty@protonmail.com - 1YWqF3SGnQMkwgfGasrNmYv1XG](https://atlas.torproject.org/#search/family:CFEC9600E877776982C3161B6A98812871F2A07F)    |       1.07 |         3 | 2016-01-26   |
| [info omuravpn.com](https://atlas.torproject.org/#search/family:94C0F99BA44AA4A6767C71333B8A66DBD1BC08C7)                                     |       1.02 |         5 | 2017-01-05   |
| [poiuty@protonmail.com - 1YWqF3SGnQMkwgfGasrNmYv1XG](https://atlas.torproject.org/#details/B42AAFC99176BFDA23033191A9F6A7CCFE9F30EA)          |       0.99 |         1 | 2017-12-22   |
| [0x9501B909 Random Person &lt;deep.thought AT riseup d](https://atlas.torproject.org/#search/family:3F39BC367D7FCF3F631C49190F4D0C4312307A8F) |       0.93 |         7 | 2017-02-20   |
| [god AT universe.org](https://atlas.torproject.org/#search/family:F3CEC87ED91E0B0B1D86BE4D7DE90F00B607ECAF)                                   |       0.92 |         2 | 2016-10-22   |
| [&lt;roottor00@splitdna.com&gt; - 1LLnvMu2s4BaF2LmsqV8Ru](https://atlas.torproject.org/#details/1C90D3AEADFF3BCD079810632C8B85637924A58E)     |       0.89 |         1 | 2014-04-08   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://atlas.torproject.org/#search/family:B08E51FED96A7A7A6081ACC96299713F3F171B3A)            |       0.89 |        11 | 2016-04-10   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            2.813 |     11.7  |       0    |        33 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |            1.449 |      6.02 |       0    |        12 | 2016-12-23   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://atlas.torproject.org/#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)    |            1.129 |      1.32 |       0.26 |         8 | 2015-06-01   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            1.019 |      0    |       2.21 |         7 | 2014-04-22   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |            1.017 |      0.38 |       1.84 |         7 | 2016-08-10   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.845 |      2.87 |       0.35 |        14 | 2016-01-26   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.799 |      3.32 |       0    |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |            0.798 |      3.32 |       0    |        11 | 2017-12-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.759 |      0    |       1.69 |        19 | 2015-05-16   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            0.616 |      2.56 |       0    |         5 | 2014-04-09   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            16.51 |      21.06 |      7    |       506 |
| Online S.a.s.               |             9.71 |      11.2  |     12.69 |       376 |
| DigitalOcean, LLC           |             6.18 |       7.34 |      1.71 |       305 |
| Hetzner Online GmbH         |             5.69 |       7.06 |      0.74 |       273 |
| Host Europe GmbH            |             2.3  |       3.75 |      0    |        36 |
| SOFTplus Entwicklungen GmbH |             1.38 |       0.3  |      5.08 |        19 |
| SURFnet bv                  |             1.34 |       0.19 |      1.05 |        12 |
| NForce Entertainment B.V.   |             1.28 |       0.34 |      4.52 |        16 |
| Voxility S.R.L.             |             1.07 |       0.48 |      2.7  |        17 |
| ISPpro Internet KG          |             1.03 |       2.28 |      0    |        29 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             37.7 |     30.98 |      36.53 |      1842 |
| 0.3.2         |             32.8 |     47.22 |      31.36 |      1521 |
| 0.2.9         |             13.3 |      9.29 |      15.52 |      1139 |
| 0.3.0         |              5.6 |      3.84 |       5.62 |       345 |
| 0.2.5         |              5.4 |      4.42 |       6.36 |       520 |
| 0.2.7         |              1.6 |      0.49 |       1.48 |       261 |
| 0.2.4         |              1.5 |      0.88 |       2.09 |       264 |
| 0.3.3         |              1.2 |      2.59 |       0.83 |        21 |
| 0.2.8         |              0.3 |      0.2  |       0.05 |        43 |
| 0.2.6         |              0.1 |      0.04 |       0.11 |        38 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.37 |       3.68 |      1.41 |       563 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             89.7 |      90.6 |       91.4 |      5558 |
| BSD     |              9.9 |       9.3 |        8.1 |       296 |
| Windows |              0.2 |       0   |        0.1 |       105 |
| SunOS   |              0   |       0   |        0.1 |         4 |
| Darwin  |              0   |       0   |        0   |        12 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            19.14 |      22.19 |       14.08 |      22.3 |       586 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     28.01 |            134 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1113 |
| None                                       |       586 |
| obfs3, obfs4, scramblesuit                 |       247 |
| obfs3, obfs4                               |        59 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        18 |
| obfs2, obfs3                               |        10 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         5 |
| scramblesuit                               |         3 |
| fte, obfs3, obfs4                          |         2 |
| obfs2, obfs3, obfs4, scramblesuit          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| meek, obfs4                                |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

