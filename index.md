---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-03-28 17:00 UTC**

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
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)           | 0.04        | 0.16       | 3         | 2               | 2016-08-28     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)   | 0.04        | 0.31       | 2         | 2               | 2017-02-16     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca) | 0.01        | 0.46       | 7         | 2               | 2018-02-11     | 4                           |
| **Total**                                                                                                      | **0.09**    | **0.93**   | **12**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |     11.91 |        26 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88)    |      5.86 |        13 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      2.7  |        11 | 2017-12-05   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      2.58 |         6 | 2017-11-29   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.43 |         1 | 2014-04-19   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      1.99 |         4 | 2014-11-21   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)      |      1.92 |         7 | 2014-04-09   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06)    |      1.9  |         6 | 2014-04-08   |
| [Datashield, Inc. abuse@xor.sc](https://metrics.torproject.org/rs.html#details/D8FF84E5E29A92F09F8263D4662627ECC479B108)                                  |      1.81 |         1 | 2018-02-24   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://metrics.torproject.org/rs.html#search/family:38A42B8D7C0E6346F4A4821617740AEE86EA885B) |      1.8  |         3 | 2014-11-04   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [33b pm.me](https://metrics.torproject.org/rs.html#search/family:175921396C7C426309AB03775A9930B6F611F794)                                             |       1.78 |         8 | 2015-10-19   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.68 |         6 | 2014-04-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       1.19 |         7 | 2016-01-03   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:068308AD070849A71B8C1DB06C2509E82C40B908)      |       1.12 |         6 | 2016-08-10   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.88 |         5 | 2017-10-24   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       0.87 |        17 | 2015-10-10   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.84 |         3 | 2015-04-22   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:27C0081F17CA00AAB981122F6A0E49C6CD0A5A6C)           |       0.65 |        10 | 2018-01-07   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://metrics.torproject.org/rs.html#search/family:166F00EA1BF27F20E8B2D7EF7FFF200E52B47D00)            |       0.58 |         9 | 2017-02-08   |
| [tor-abuse&lt;at&gt;mailbox&lt;dot&gt;org](https://metrics.torproject.org/rs.html#search/family:21D53193494ADB42057242CE276953A90543BE31)              |       0.56 |         2 | 2017-12-20   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            3.092 |     11.91 |       0    |        26 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88) |            1.522 |      5.86 |       0    |        13 | 2016-12-23   |
| [33b pm.me](https://metrics.torproject.org/rs.html#search/family:175921396C7C426309AB03775A9930B6F611F794)                                             |            1.053 |      0    |       1.78 |         8 | 2015-10-19   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            1.006 |      0    |       1.68 |         8 | 2014-04-22   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.791 |      2.58 |       0.2  |         8 | 2016-01-26   |
| [tor-abuse&lt;at&gt;mailbox&lt;dot&gt;org](https://metrics.torproject.org/rs.html#search/family:0EBD534AB62250AE6B074F2A031350332F44D8FF)              |            0.782 |      1.72 |       0.56 |         4 | 2017-12-20   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:068308AD070849A71B8C1DB06C2509E82C40B908)      |            0.714 |      0.18 |       1.12 |         7 | 2016-08-10   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |            0.705 |      0    |       1.19 |         7 | 2016-01-03   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |            0.702 |      2.7  |       0    |        11 | 2017-12-05   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.631 |      2.43 |       0    |         1 | 2014-04-19   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                   |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                   |            13.8  |      16.26 |      9.48 |       524 |
| Online S.a.s.             |            11.87 |      13.98 |     11.5  |       375 |
| Hetzner Online GmbH       |             8.49 |      10.54 |      2.89 |       309 |
| DigitalOcean, LLC         |             5.59 |       7.62 |      0.77 |       302 |
| Joshua Peter McQuistan    |             3.09 |       0    |     11.91 |        26 |
| Digital Ocean, Inc.       |             2.11 |       2.57 |      1.25 |        52 |
| Host Europe GmbH          |             1.6  |       2.15 |      0.18 |        35 |
| NForce Entertainment B.V. |             1.57 |       0.14 |      5.73 |        21 |
| myLoc managed IT AG       |             1.32 |       1.61 |      0.29 |        32 |
| SURFnet bv                |             1.29 |       1.47 |      1.57 |        11 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             57.5 |     59.52 |      57.72 |      2753 |
| 0.2.9         |             14.1 |     10.35 |      14.65 |      1206 |
| 0.3.1         |             10.1 |     10.44 |       9.75 |       886 |
| 0.3.3         |             10   |     12.23 |      10.71 |       321 |
| 0.2.5         |              3.5 |      3.38 |       3.3  |       468 |
| 0.2.4         |              1.2 |      0.96 |       1.15 |       273 |
| 0.3.0         |              1.2 |      0.09 |       1.46 |       204 |
| 0.3.4         |              1   |      2.8  |       0.43 |        21 |
| 0.2.7         |              0.7 |      0.05 |       0.69 |       187 |
| 0.2.8         |              0.1 |      0.14 |       0.03 |        34 |
| 0.2.6         |              0   |      0    |       0.06 |        31 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.43 |       3.41 |      1.26 |       729 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.6 |      91.2 |       90.7 |      5861 |
| BSD     |              8.1 |       8.7 |        9.1 |       329 |
| Windows |              0.1 |       0   |        0   |       125 |
| Darwin  |              0   |       0   |        0   |        11 |
| SunOS   |              0   |       0   |        0   |         3 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            22.26 |      21.51 |       21.36 |     24.62 |       704 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     28.72 |            147 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1016 |
| None                                       |       589 |
| obfs3, obfs4, scramblesuit                 |       245 |
| obfs3, obfs4                               |        60 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        17 |
| obfs2, obfs3                               |         9 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         4 |
| fte, obfs3, obfs4                          |         3 |
| scramblesuit                               |         3 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
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

