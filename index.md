---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-05-15 16:00 UTC**

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

| Contact                                                                                                                           | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:----------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                              | 0.07        | 0.07       | 3         | 2               | 2016-08-28     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                    | 0.04        | 0.01       | 7         | 2               | 2018-02-11     | 4                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                      | 0.03        | 0.31       | 2         | 2               | 2017-02-16     | 1                           |
| [zcashtorservers.org supported by a z.cash.foundati](endtoend-correlation-groups#zcashtorserversorg-supported-by-a-zcashfoundati) | 0.02        | 1.64       | 7         | 4               | 2018-05-10     | 1                           |
| **Total**                                                                                                                         | **0.16**    | **2.03**   | **19**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Exit(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |      9.65 |        27 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88) |      5.58 |        13 | 2016-12-23   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      3.97 |        15 | 2015-05-22   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A) |      3.54 |         8 | 2014-04-09   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.94 |         1 | 2014-04-19   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |      2.7  |         6 | 2017-11-29   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)   |      2.13 |         7 | 2014-04-09   |
| [Datashield, Inc. abuse@xor.sc](https://metrics.torproject.org/rs.html#details/D4E49B296490283DBD55665F10431284E92E3306)                               |      1.92 |         1 | 2018-04-04   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      1.86 |         4 | 2014-11-21   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      1.84 |        11 | 2017-12-05   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |       1.34 |         7 | 2014-04-22   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:068308AD070849A71B8C1DB06C2509E82C40B908)      |       0.99 |         6 | 2016-08-10   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |       0.97 |         8 | 2015-01-29   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.94 |         7 | 2016-01-03   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.86 |         5 | 2017-10-24   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       0.84 |        14 | 2015-05-16   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.77 |         2 | 2015-04-22   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:27C0081F17CA00AAB981122F6A0E49C6CD0A5A6C)           |       0.75 |        10 | 2018-01-07   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://metrics.torproject.org/rs.html#search/family:166F00EA1BF27F20E8B2D7EF7FFF200E52B47D00)            |       0.66 |         9 | 2017-02-08   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |       0.59 |        10 | 2016-10-28   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.458 |      9.65 |       0    |        27 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88) |            1.422 |      5.58 |       0    |        13 | 2016-12-23   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            1.036 |      3.97 |       0.01 |        17 | 2013-08-22   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A) |            0.908 |      3.54 |       0    |         9 | 2014-04-09   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            0.827 |      0    |       1.34 |         7 | 2014-04-22   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.791 |      2.7  |       0.16 |         8 | 2016-01-26   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.749 |      2.94 |       0    |         1 | 2014-04-19   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.671 |      0    |       0.84 |        17 | 2015-05-16   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:068308AD070849A71B8C1DB06C2509E82C40B908)      |            0.657 |      0.17 |       0.99 |         7 | 2016-08-10   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |            0.603 |      0    |       0.97 |         8 | 2015-01-29   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                   |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                   |            13.85 |      18.05 |      8.39 |       532 |
| Online S.a.s.             |            12.71 |      13.2  |     13.57 |       383 |
| Hetzner Online GmbH       |             7.8  |       8.93 |      1.17 |       348 |
| DigitalOcean, LLC         |             3.79 |       5.07 |      0.18 |       270 |
| Joshua Peter McQuistan    |             2.48 |       0.03 |      9.65 |        29 |
| myLoc managed IT AG       |             1.91 |       2.75 |      0.47 |        35 |
| SURFnet bv                |             1.91 |       1.54 |      3.54 |        18 |
| NForce Entertainment B.V. |             1.68 |       0.13 |      6.23 |        21 |
| Digital Ocean, Inc.       |             1.55 |       1.58 |      0.78 |        49 |
| netcup GmbH               |             1.26 |       1.73 |      0.34 |        43 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             60.8 |     63.48 |      62.74 |      3052 |
| 0.2.9         |             13.7 |      8.97 |      13.42 |      1359 |
| 0.3.3         |             10.4 |     16.99 |       8.75 |       342 |
| 0.3.1         |              7.7 |      5.88 |       7.87 |       747 |
| 0.2.5         |              2.9 |      2.71 |       3.15 |       356 |
| 0.2.4         |              1.4 |      0.14 |       1.75 |       244 |
| 0.2.7         |              0.8 |      0.04 |       0.56 |       177 |
| 0.3.4         |              0.8 |      1.68 |       0.64 |        19 |
| 0.3.0         |              0.7 |      0.04 |       0.87 |       164 |
| 0.2.8         |              0.1 |      0    |       0.14 |        38 |
| 0.2.6         |              0   |      0.01 |       0.06 |        29 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             6.24 |       6.56 |      2.96 |      1008 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91   |      91.4 |       90   |      6024 |
| BSD     |              8.6 |       8.5 |        9.7 |       341 |
| Windows |              0.2 |       0   |        0.1 |       107 |
| Darwin  |              0   |       0   |        0   |        15 |
| SunOS   |              0   |       0   |        0.1 |         3 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            23.11 |      23.22 |       20.34 |     26.99 |       753 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     30.46 |            164 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       916 |
| None                                       |       586 |
| obfs3, obfs4                               |        61 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        16 |
| obfs2, obfs3                               |         9 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         7 |
| obfs3, obfs4, scramblesuit                 |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         4 |
| fte, obfs3, obfs4                          |         3 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| meek, obfs4                                |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

