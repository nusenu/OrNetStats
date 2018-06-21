---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-06-21 11:00 UTC**

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

| Contact                                                                                                        | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:---------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca) | 0.04        | 0.09       | 7         | 2               | 2018-02-11     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)           | 0.03        | 0.16       | 3         | 2               | 2016-08-28     | 1                           |
| [Person admin@example.com](endtoend-correlation-groups#person-adminexamplecom)                                 | 0.03        | 0.11       | 2         | 2               | 2018-05-20     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)   | 0.02        | 0.31       | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                      | **0.12**    | **0.67**   | **14**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |      8.97 |        27 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88)    |      5.14 |        12 | 2016-12-23   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      4.28 |        15 | 2015-05-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)      |      2.94 |         7 | 2014-04-09   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.53 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      2.28 |        11 | 2017-12-05   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06)    |      1.7  |         6 | 2014-04-08   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      1.65 |         4 | 2017-11-29   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://metrics.torproject.org/rs.html#search/family:185663B7C12777F052B2C2D23D7A239D8DA88A0F) |      1.61 |         5 | 2011-10-06   |
| [zcashtorservers.org supported by a z.cash.foundati](https://metrics.torproject.org/rs.html#search/family:6B23021CB4B4FE6525D23BE8E6BA4F91EAAB0741)       |      1.45 |         4 | 2018-01-31   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |       1.94 |         7 | 2014-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       1.2  |        17 | 2015-05-16   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |       1.01 |         8 | 2015-01-29   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.97 |         7 | 2016-01-03   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:068308AD070849A71B8C1DB06C2509E82C40B908)      |       0.9  |         6 | 2016-08-10   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.79 |         5 | 2017-10-24   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:27C0081F17CA00AAB981122F6A0E49C6CD0A5A6C)           |       0.72 |        10 | 2018-01-07   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                  |       0.69 |         3 | 2018-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.67 |         2 | 2015-04-22   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://metrics.torproject.org/rs.html#search/family:166F00EA1BF27F20E8B2D7EF7FFF200E52B47D00)            |       0.58 |         9 | 2017-02-08   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.259 |      8.97 |       0    |        27 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88) |            1.294 |      5.14 |       0    |        12 | 2016-12-23   |
| [tor AT appliedprivacy.net](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)                             |            1.249 |      0    |       0.31 |        14 | 2017-06-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            1.139 |      0    |       1.94 |         7 | 2014-04-22   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            1.088 |      4.28 |       0.01 |        16 | 2013-08-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)   |            0.739 |      2.94 |       0    |         7 | 2014-04-09   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.703 |      0    |       1.2  |        17 | 2015-05-16   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.638 |      2.53 |       0    |         1 | 2014-04-19   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |            0.595 |      0    |       1.01 |         8 | 2015-01-29   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |            0.574 |      2.28 |       0    |        11 | 2017-12-05   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                   |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                   |            13.58 |      17.66 |      7.8  |       535 |
| Online S.a.s.             |            12.88 |      15.29 |      9.84 |       344 |
| Hetzner Online GmbH       |             7.58 |       7.91 |      1.42 |       346 |
| DigitalOcean, LLC         |             2.72 |       3.19 |      0.12 |       240 |
| Joshua Peter McQuistan    |             2.28 |       0.04 |      8.97 |        28 |
| NForce Entertainment B.V. |             2.01 |       0.08 |      7.74 |        28 |
| Host Europe GmbH          |             1.89 |       2.89 |      0.38 |        36 |
| SURFnet bv                |             1.85 |       1.76 |      3.26 |        28 |
| myLoc managed IT AG       |             1.7  |       2.17 |      1.23 |        36 |
| netcup GmbH               |             1.34 |       1.84 |      0.37 |        42 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.3         |             45.3 |     53.66 |      43.11 |      2136 |
| 0.3.2         |             26.8 |     24.73 |      29.65 |      1522 |
| 0.2.9         |             14   |      9.76 |      13.94 |      1354 |
| 0.3.1         |              4.5 |      3.51 |       4.93 |       346 |
| 0.3.4         |              4   |      6.26 |       3.89 |       127 |
| 0.2.5         |              2.3 |      1.69 |       2.08 |       298 |
| 0.2.4         |              1.2 |      0.2  |       0.81 |       214 |
| 0.2.7         |              0.6 |      0.03 |       0.44 |       156 |
| 0.3.0         |              0.6 |      0    |       0.78 |        95 |
| 0.2.8         |              0.1 |      0.06 |       0.12 |        31 |
| 0.2.6         |              0   |      0.01 |       0.04 |        28 |
| 0.3.5         |              0   |      0.01 |       0.15 |         4 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.07 |       4.29 |      2.03 |       822 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.2 |      92.1 |       89.8 |      5816 |
| BSD     |              9.3 |       7.7 |        9.8 |       350 |
| SunOS   |              0.1 |       0   |        0.1 |         5 |
| Windows |              0.1 |       0   |        0.1 |        96 |
| Darwin  |              0   |       0   |        0   |        19 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|             24.8 |      23.47 |       22.87 |     29.66 |       783 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     33.16 |            170 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       871 |
| None                                       |       590 |
| obfs3, obfs4                               |        62 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        15 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs2, obfs3                               |         7 |
| obfs3, obfs4, scramblesuit                 |         6 |
| obfs3, scramblesuit                        |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         4 |
| fte, meek, obfs3, obfs4                    |         3 |
| fte, obfs3, obfs4                          |         2 |
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

