---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-01-26 09:00 UTC**

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
| [abuse AT torworld.org - BTC 17iwdtpmgHdPt15twdT2](endtoend-correlation-groups#abuse-at-torworldorg---btc-17iwdtpmghdpt15twdt2)          | 0.23        | 0.78       | 9         | 6               | 2018-01-14     | 7                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                     | 0.12        | 0.15       | 3         | 2               | 2016-08-28     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-btc---14w) | 0.11        | 1.0        | 12        | 2               | 2016-04-01     | 4                           |
| [-](endtoend-correlation-groups#-)                                                                                                       | 0.07        | 0.28       | 2         | 2               | 2018-01-02     | 1                           |
| [tor-mngr AT scalaire DOT fr](endtoend-correlation-groups#tor-mngr-at-scalaire-dot-fr)                                                   | 0.03        | 0.18       | 2         | 2               | 2017-11-27     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                                 | 0.02        | 0.03       | 3         | 3               | 2017-10-01     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.02        | 0.27       | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                                                | **0.60**    | **2.69**   | **33**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |     11.56 |        33 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      6.13 |        12 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      3.22 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |      3.14 |        11 | 2017-12-05   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      2.57 |        10 | 2017-11-29   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.49 |         3 | 2014-11-04   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      2.15 |         5 | 2014-04-09   |
| [John Doe johndoe@novogara.com](https://atlas.torproject.org/#details/0593F5255316748247EBA76353A3A61F62224903)                                  |      2.07 |         1 | 2017-09-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.02 |         7 | 2013-07-10   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      1.94 |         6 | 2014-04-08   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |       2.38 |         6 | 2016-08-10   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       2.06 |         6 | 2014-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       1.65 |        17 | 2015-10-10   |
| [god AT universe.org](https://atlas.torproject.org/#search/family:F3CEC87ED91E0B0B1D86BE4D7DE90F00B607ECAF)                                   |       1.35 |         2 | 2016-10-22   |
| [0x9501B909 Random Person &lt;deep.thought AT riseup d](https://atlas.torproject.org/#search/family:3F39BC367D7FCF3F631C49190F4D0C4312307A8F) |       1.04 |         8 | 2017-02-20   |
| [poiuty@protonmail.com - 1YWqF3SGnQMkwgfGasrNmYv1XG](https://atlas.torproject.org/#search/family:CFEC9600E877776982C3161B6A98812871F2A07F)    |       1.02 |         3 | 2016-01-26   |
| [info omuravpn.com](https://atlas.torproject.org/#search/family:94C0F99BA44AA4A6767C71333B8A66DBD1BC08C7)                                     |       0.99 |         5 | 2017-01-05   |
| [Dam &lt;tor AT d4m dot fr&gt;](https://atlas.torproject.org/#details/417FC40312E2C392EFC569145E3D052716E7C27E)                               |       0.82 |         1 | 2018-01-02   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://atlas.torproject.org/#search/family:B08E51FED96A7A7A6081ACC96299713F3F171B3A)            |       0.81 |        11 | 2016-04-10   |
| [Anders Burmeister &lt;anders.burmeister AT protonmail](https://atlas.torproject.org/#search/family:92412EA1B9AA887D462B51D816777002F4D58907) |       0.81 |         6 | 2017-02-11   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            2.905 |     11.56 |       0    |        33 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |            1.541 |      6.13 |       0    |        12 | 2016-12-23   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |            1.103 |      0.31 |       2.38 |         7 | 2016-08-10   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://atlas.torproject.org/#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)    |            1.014 |      1.31 |       0.19 |         7 | 2016-11-02   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.949 |      0    |       2.06 |         7 | 2014-04-22   |
| [0ED0EA32](https://atlas.torproject.org/#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |            0.832 |      0    |       0    |         5 | 2017-10-24   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.812 |      2.57 |       0.38 |        13 | 2016-01-26   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.811 |      3.22 |       0    |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |            0.789 |      3.14 |       0    |        11 | 2017-12-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.723 |      0    |       1.65 |        19 | 2015-05-16   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            16.07 |      20.79 |      6.98 |       501 |
| Online S.a.s.               |             9.73 |      10.36 |     12.6  |       377 |
| DigitalOcean, LLC           |             5.57 |       7.68 |      1.44 |       305 |
| Hetzner Online GmbH         |             5.37 |       6.59 |      0.91 |       281 |
| Host Europe GmbH            |             2.14 |       3.45 |      0    |        36 |
| SOFTplus Entwicklungen GmbH |             1.37 |       0.3  |      4.79 |        19 |
| NForce Entertainment B.V.   |             1.3  |       0.2  |      4.52 |        16 |
| Voxility S.R.L.             |             1.15 |       0.49 |      2.66 |        17 |
| SURFnet bv                  |             1.15 |       0.04 |      1.12 |        12 |
| myLoc managed IT AG         |             1.01 |       1.66 |      0.37 |        38 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             36.8 |     54    |      35.04 |      1733 |
| 0.3.1         |             34.3 |     24.5  |      32.93 |      1725 |
| 0.2.9         |             13.8 |      9.03 |      15.26 |      1159 |
| 0.3.0         |              5.2 |      3.74 |       5.33 |       333 |
| 0.2.5         |              5   |      3.76 |       6.64 |       519 |
| 0.2.4         |              1.5 |      1.06 |       2.25 |       278 |
| 0.2.7         |              1.5 |      0.46 |       1.57 |       259 |
| 0.3.3         |              1.1 |      3.1  |       0.74 |        21 |
| 0.2.8         |              0.2 |      0.26 |       0.06 |        41 |
| 0.2.6         |              0.1 |      0.03 |       0.13 |        34 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.29 |       3.96 |      1.57 |       571 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             89.4 |      90.2 |       91.4 |      5615 |
| BSD     |             10.1 |       9.7 |        8.1 |       298 |
| Windows |              0.2 |       0   |        0.1 |       116 |
| Darwin  |              0   |       0   |        0   |         9 |
| SunOS   |              0   |       0   |        0.1 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.78 |      21.28 |       13.52 |     22.87 |       595 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     28.31 |            139 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1107 |
| None                                       |       579 |
| obfs3, obfs4, scramblesuit                 |       247 |
| obfs3, obfs4                               |        59 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        17 |
| obfs2, obfs3                               |        11 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs3, scramblesuit                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         3 |
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

