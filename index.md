---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-02-17 07:00 UTC**

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

| Contact                                                                                                                                | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:---------------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                   | 0.1         | 0.19       | 3         | 2               | 2016-08-28     | 1                           |
| [https://www.torservers.net/donate.html &lt;support .A](endtoend-correlation-groups#httpswwwtorserversnetdonatehtml-support-a)         | 0.08        | 5.27       | 11        | 3               | 2017-11-01     | 1                           |
| [ninja.turtle5@aol.com](endtoend-correlation-groups#ninjaturtle5aolcom)                                                                | 0.06        | 0.06       | 5         | 2               | 2018-01-30     | 1                           |
| [Abuse Department &lt;abuse AT hartvoorinternetvrijhei](endtoend-correlation-groups#abuse-department-abuse-at-hartvoorinternetvrijhei) | 0.02        | 1.25       | 3         | 2               | 2018-01-27     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                           | 0.02        | 0.27       | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                                              | **0.28**    | **7.04**   | **24**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |     11.55 |        26 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      5.97 |        12 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |      3.35 |        11 | 2017-12-05   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      2.8  |         8 | 2017-11-29   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.48 |         7 | 2013-07-10   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.47 |         1 | 2014-04-19   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      2.4  |         7 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |      2.28 |         7 | 2016-02-06   |
| [John Doe johndoe@novogara.com](https://atlas.torproject.org/#details/0593F5255316748247EBA76353A3A61F62224903)                                  |      2.13 |         1 | 2017-09-05   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://atlas.torproject.org/#search/family:A10C4F666D27364036B562823E5830BC448E046A) |      1.96 |         5 | 2011-10-06   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                         |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [0ED0EA32](https://atlas.torproject.org/#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                           |       2.1  |         5 | 2017-10-24   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)      |       1.22 |        17 | 2015-10-10   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)   |       1.16 |         6 | 2016-08-10   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                |       1.1  |         3 | 2015-04-22   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://atlas.torproject.org/#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9) |       0.98 |         3 | 2017-02-25   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://atlas.torproject.org/#search/family:71539D1911ECB826069A4D156771AC4F9F4632A7)        |       0.97 |         6 | 2018-01-07   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799) |       0.92 |         5 | 2014-04-22   |
| [TotorBE AT gmail DOT com](https://atlas.torproject.org/#search/family:F3CEC87ED91E0B0B1D86BE4D7DE90F00B607ECAF)                           |       0.74 |         2 | 2016-10-22   |
| [D80EA216](https://atlas.torproject.org/#details/D80EA21626BFAE8044E4037FE765252E157E3586)                                                 |       0.72 |         1 | 2017-10-27   |
| [tor-relays@lists.torproject.org](https://atlas.torproject.org/#search/family:151BDD000832E22385680E456E4B94220317B122)                    |       0.65 |        10 | 2017-07-02   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            2.901 |     11.55 |       0    |        26 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |            1.499 |      5.97 |       0    |        12 | 2016-12-23   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://atlas.torproject.org/#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)    |            1.137 |      1.19 |       0.98 |         8 | 2015-06-01   |
| [0ED0EA32](https://atlas.torproject.org/#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |            1.103 |      0    |       2.1  |         5 | 2017-10-24   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.947 |      0    |       0.92 |         7 | 2014-04-22   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |            0.843 |      3.35 |       0    |        11 | 2017-12-05   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.83  |      2.8  |       0.24 |        10 | 2016-01-26   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |            0.654 |      0.17 |       1.16 |         7 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.651 |      0    |       1.22 |        19 | 2015-05-16   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)           |            0.633 |      2.48 |       0.01 |         8 | 2013-07-10   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            15.99 |      22.76 |      7.35 |       503 |
| Online S.a.s.               |            10.37 |      10.9  |     11.04 |       380 |
| Hetzner Online GmbH         |             7.19 |       9.27 |      1.84 |       287 |
| DigitalOcean, LLC           |             4.81 |       5.7  |      1.74 |       304 |
| Host Europe GmbH            |             2.18 |       2.82 |      0    |        36 |
| SOFTplus Entwicklungen GmbH |             1.61 |       0.39 |      5.4  |        19 |
| SURFnet bv                  |             1.28 |       1.82 |      1.25 |        12 |
| NForce Entertainment B.V.   |             1.2  |       0.03 |      4.4  |        17 |
| THC Projects SRL            |             1    |       1.28 |      0    |        17 |
| Voxility S.R.L.             |             0.95 |       0.13 |      2.83 |        14 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             44.4 |     43.74 |      44.74 |      2210 |
| 0.3.1         |             20   |     15.36 |      23.01 |      1151 |
| 0.2.9         |             13.2 |      9.64 |      12.83 |      1141 |
| 0.3.3         |             12.7 |     24.89 |       9.23 |       229 |
| 0.2.5         |              4.2 |      2.66 |       4.71 |       498 |
| 0.3.0         |              2   |      1.07 |       2.36 |       245 |
| 0.2.4         |              1.4 |      1.21 |       1.58 |       243 |
| 0.2.7         |              1.1 |      0.2  |       1.1  |       215 |
| 0.2.8         |              0.2 |      0.2  |       0.34 |        38 |
| 0.3.4         |              0.2 |      0.95 |       0    |         3 |
| 0.2.6         |              0   |      0.03 |       0.04 |        30 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             4.73 |        5.1 |      2.53 |       733 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90   |      91.3 |       87.7 |      5570 |
| BSD     |              9.7 |       8.4 |       12   |       290 |
| Windows |              0.1 |       0   |        0   |        99 |
| Darwin  |              0   |       0   |        0   |        10 |
| SunOS   |              0   |       0   |        0   |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            20.21 |      21.53 |       16.36 |     23.98 |       659 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     28.54 |            160 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1027 |
| None                                       |       588 |
| obfs3, obfs4, scramblesuit                 |       246 |
| obfs3, obfs4                               |        54 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        18 |
| obfs2, obfs3                               |        10 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| fte, obfs3, obfs4                          |         3 |
| meek                                       |         3 |
| scramblesuit                               |         3 |
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
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

