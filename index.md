---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-03-18 21:00 UTC**

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

| Contact                                                                                                                       | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                          | 0.07        | 0.27       | 3         | 2               | 2016-08-28     | 1                           |
| [http://tor.jonny.mobi &lt;torsupport .AT. jonny .DOT.](endtoend-correlation-groups#httptorjonnymobi-torsupport-at-jonny-dot) | 0.03        | 0.18       | 6         | 2               | 2018-03-02     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                | 0.03        | 0.53       | 7         | 2               | 2018-02-11     | 4                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                  | 0.02        | 0.34       | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                                     | **0.15**    | **1.32**   | **18**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |     11.09 |        25 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88) |      6.14 |        13 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      2.93 |        11 | 2017-12-05   |
| [Datashield, Inc. abuse@xor.sc](https://metrics.torproject.org/rs.html#details/D8FF84E5E29A92F09F8263D4662627ECC479B108)                               |      2.71 |         1 | 2018-02-24   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.62 |         1 | 2014-04-19   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      2.23 |         7 | 2013-07-10   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |      2.15 |         6 | 2017-11-29   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06) |      2.12 |         6 | 2014-04-08   |
| [abuse aT nectodoT--onion](https://metrics.torproject.org/rs.html#search/family:162F7E752504C49A656FF1E9669E0B9572CE4870)                              |      2.04 |         6 | 2015-08-27   |
| [tor-abuse&lt;at&gt;mailbox&lt;dot&gt;org](https://metrics.torproject.org/rs.html#search/family:0EBD534AB62250AE6B074F2A031350332F44D8FF)              |      1.64 |         2 | 2018-01-23   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.72 |         6 | 2014-04-22   |
| [33b pm.me](https://metrics.torproject.org/rs.html#search/family:175921396C7C426309AB03775A9930B6F611F794)                                             |       1.63 |         8 | 2015-10-19   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       1.07 |         7 | 2016-01-03   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.98 |         5 | 2017-10-24   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:068308AD070849A71B8C1DB06C2509E82C40B908)      |       0.98 |         6 | 2016-08-10   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.93 |         3 | 2015-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       0.87 |        16 | 2015-10-10   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:27C0081F17CA00AAB981122F6A0E49C6CD0A5A6C)           |       0.79 |        10 | 2018-01-07   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://metrics.torproject.org/rs.html#search/family:166F00EA1BF27F20E8B2D7EF7FFF200E52B47D00)            |       0.62 |         9 | 2017-02-08   |
| [enigma AT= s0ny doT--- net](https://metrics.torproject.org/rs.html#details/42B4F52C5B11E4D39855F654955425B0D5A0598B)                                  |       0.58 |         1 | 2017-02-13   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.614 |     11.09 |       0    |        25 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88) |            1.446 |      6.14 |       0    |        13 | 2016-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            1.025 |      0    |       1.72 |         6 | 2014-04-22   |
| [33b pm.me](https://metrics.torproject.org/rs.html#search/family:175921396C7C426309AB03775A9930B6F611F794)                                             |            0.969 |      0    |       1.63 |         8 | 2015-10-19   |
| [tor-abuse&lt;at&gt;mailbox&lt;dot&gt;org](https://metrics.torproject.org/rs.html#search/family:0EBD534AB62250AE6B074F2A031350332F44D8FF)              |            0.716 |      1.64 |       0.55 |         4 | 2017-12-20   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |            0.692 |      2.93 |       0    |        11 | 2017-12-05   |
| [Datashield, Inc. abuse@xor.sc](https://metrics.torproject.org/rs.html#details/D8FF84E5E29A92F09F8263D4662627ECC479B108)                               |            0.639 |      2.71 |       0    |         1 | 2018-02-24   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |            0.638 |      0    |       1.07 |         7 | 2016-01-03   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.619 |      2.15 |       0.18 |         8 | 2016-01-26   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.618 |      2.62 |       0    |         1 | 2014-04-19   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                   |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                   |            14.54 |      18.04 |      7.66 |       519 |
| Online S.a.s.             |            11    |      13.5  |     10.08 |       376 |
| Hetzner Online GmbH       |             7.71 |       8.34 |      2.9  |       310 |
| DigitalOcean, LLC         |             5.2  |       7.21 |      0.8  |       276 |
| Joshua Peter McQuistan    |             2.98 |       0.61 |     11.09 |        30 |
| Digital Ocean, Inc.       |             1.95 |       1.92 |      1.55 |        56 |
| Host Europe GmbH          |             1.84 |       2.94 |      0.06 |        36 |
| NForce Entertainment B.V. |             1.66 |       0.06 |      6.74 |        21 |
| SURFnet bv                |             1.3  |       1.65 |      1.3  |        11 |
| myLoc managed IT AG       |             1.22 |       1.45 |      0.3  |        33 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             56.4 |     60.75 |      56.7  |      2600 |
| 0.2.9         |             13.6 |      9.64 |      13.51 |      1187 |
| 0.3.1         |             11.8 |     10.17 |      11.31 |       958 |
| 0.3.3         |             10   |     12.29 |      10.98 |       311 |
| 0.2.5         |              3.5 |      3.16 |       3.34 |       468 |
| 0.3.0         |              1.3 |      0.25 |       1.46 |       202 |
| 0.2.4         |              1.1 |      1.24 |       0.97 |       253 |
| 0.3.4         |              1   |      2.41 |       0.76 |        22 |
| 0.2.7         |              0.7 |      0.04 |       0.62 |       185 |
| 0.2.8         |              0.1 |      0.08 |       0.14 |        39 |
| 0.2.6         |              0   |      0    |       0.06 |        36 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.48 |       3.27 |      1.63 |       715 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.8 |      90.7 |       89.6 |      5779 |
| BSD     |              8.8 |       9.1 |       10   |       320 |
| Windows |              0.1 |       0   |        0   |       115 |
| SunOS   |              0.1 |       0   |        0.1 |         4 |
| Darwin  |              0   |       0   |        0   |        12 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            21.92 |      21.43 |       19.81 |     26.12 |       695 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     30.83 |            150 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1018 |
| None                                       |       583 |
| obfs3, obfs4, scramblesuit                 |       243 |
| obfs3, obfs4                               |        58 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        18 |
| obfs2, obfs3                               |         9 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         4 |
| scramblesuit                               |         3 |
| fte, obfs3, obfs4                          |         2 |
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

