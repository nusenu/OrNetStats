---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-07-01 07:00 UTC**

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

| Contact                                                                                                      | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)    | 0.19        | 0.04       | 2         | 2               | 2018-06-20     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de) | 0.02        | 0.3        | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                    | **0.21**    | **0.34**   | **4**     |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |      9.1  |        27 | 2016-01-25   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      3.55 |        13 | 2015-05-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)      |      2.87 |         7 | 2014-04-09   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88)    |      2.84 |         6 | 2017-10-03   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.75 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      2.06 |        11 | 2017-12-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC)    |      2.03 |         6 | 2016-12-23   |
| [zcashtorservers.org - supported by a z.cash.founda](https://metrics.torproject.org/rs.html#search/family:6B23021CB4B4FE6525D23BE8E6BA4F91EAAB0741)       |      1.75 |         4 | 2018-01-31   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06)    |      1.7  |         6 | 2014-04-08   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://metrics.torproject.org/rs.html#search/family:185663B7C12777F052B2C2D23D7A239D8DA88A0F) |      1.55 |         5 | 2011-10-06   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |       1.84 |         7 | 2014-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       1.15 |        17 | 2015-05-16   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |       1    |         8 | 2015-01-29   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:068308AD070849A71B8C1DB06C2509E82C40B908)      |       0.95 |         6 | 2016-08-10   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.85 |         7 | 2016-01-03   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.79 |         2 | 2015-04-22   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.76 |         5 | 2017-10-24   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:27C0081F17CA00AAB981122F6A0E49C6CD0A5A6C)           |       0.71 |        10 | 2018-01-07   |
| [TotorBE AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:25990FC54D7268C914170A118EE4EE75025451DA)                              |       0.69 |         2 | 2016-10-22   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                  |       0.64 |         3 | 2018-04-22   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.329 |      9.1  |       0    |        27 | 2016-01-25   |
| [tor AT appliedprivacy.net](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)                             |            1.184 |      0    |       0.52 |        14 | 2017-06-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            1.078 |      0    |       1.84 |         7 | 2014-04-22   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.922 |      3.55 |       0.02 |        14 | 2013-08-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)   |            0.734 |      2.87 |       0    |         7 | 2014-04-09   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88) |            0.728 |      2.84 |       0    |         6 | 2017-10-03   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.703 |      2.75 |       0    |         1 | 2014-04-19   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.675 |      0    |       1.15 |        17 | 2015-05-16   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:068308AD070849A71B8C1DB06C2509E82C40B908)      |            0.593 |      0.15 |       0.95 |         7 | 2016-08-10   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |            0.584 |      0    |       1    |         8 | 2015-01-29   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                   |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                   |            13.1  |      17.09 |      7.24 |       535 |
| Online S.a.s.             |            12.08 |      14.53 |      9.63 |       350 |
| Hetzner Online GmbH       |             8.51 |       8.95 |      0.4  |       351 |
| NForce Entertainment B.V. |             2.63 |       0.29 |      9.41 |        32 |
| Joshua Peter McQuistan    |             2.35 |       0.04 |      9.1  |        28 |
| DigitalOcean, LLC         |             2.11 |       2.54 |      0.13 |       245 |
| SURFnet bv                |             2.04 |       1.96 |      3.49 |        28 |
| netcup GmbH               |             1.75 |       2.1  |      0.73 |        50 |
| Host Europe GmbH          |             1.73 |       2.84 |      0    |        36 |
| myLoc managed IT AG       |             1.64 |       2.14 |      0.99 |        36 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.3         |             47.9 |     55.84 |      46.69 |      2307 |
| 0.3.2         |             23.8 |     23.02 |      25.78 |      1413 |
| 0.2.9         |             13.9 |      7.4  |      14.65 |      1367 |
| 0.3.4         |              4.6 |      7.72 |       3.96 |       158 |
| 0.3.1         |              4.4 |      3.22 |       4.61 |       342 |
| 0.2.5         |              2.3 |      1.79 |       2.08 |       293 |
| 0.2.4         |              1.1 |      0.61 |       0.58 |       224 |
| 0.3.0         |              0.7 |      0.01 |       0.79 |        98 |
| 0.2.7         |              0.5 |      0.11 |       0.45 |       157 |
| 0.3.5         |              0.1 |      0.23 |       0.22 |         6 |
| 0.2.6         |              0   |      0    |       0.03 |        30 |
| 0.2.8         |              0   |      0.05 |       0.09 |        33 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             4.94 |       4.05 |      2.59 |       835 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.2 |      90.8 |       90.1 |      5906 |
| BSD     |              9.3 |       9.1 |        9.5 |       367 |
| Windows |              0.1 |       0   |        0.1 |        98 |
| SunOS   |              0   |       0   |        0   |         5 |
| Darwin  |              0   |       0   |        0   |        17 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            24.84 |      23.46 |       23.01 |     29.52 |       798 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     32.54 |            170 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       863 |
| None                                       |       588 |
| obfs3, obfs4                               |        63 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        14 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs2, obfs3                               |         8 |
| obfs3, scramblesuit                        |         7 |
| obfs3, obfs4, scramblesuit                 |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         4 |
| fte, meek, obfs3, obfs4                    |         3 |
| fte, obfs3, obfs4                          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| obfs2                                      |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

