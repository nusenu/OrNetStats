---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-12-25 08:00 UTC**

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
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)                                | 0.18        | 0.1        | 8         | 8               | 2018-11-24     | 1                           |
| [sysop at openinternet.io BTC: 1LZCkCZRqJ3fXnVqCBrq](endtoend-correlation-groups#sysopatopeninternetio-btc-1lzckczrqj3fxnvqcbrq)         | 0.04        | 0.35       | 2         | 2               | 2018-12-16     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                     | 0.02        | 0.12       | 3         | 2               | 2016-08-28     | 1                           |
| [&lt;nobody AT example dot com&gt;](endtoend-correlation-groups#nobody-at-example-dot-com)                                               | 0.02        | 0.06       | 2         | 2               | 2018-11-22     | 1                           |
| [&lt;schneider&gt; schneiderweisse AT tutanota DOT de](endtoend-correlation-groups#schneider-schneiderweisse-at-tutanota-dot-de)         | 0.02        | 0.01       | 3         | 3               | 2015-09-17     | 1                           |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](endtoend-correlation-groups#zwiebeln-at-online-de-please-donate-btc-1k38x9xq) | 0.02        | 0.99       | 31        | 9               | 2018-12-05     | 6                           |
| [Cheena &lt;cheena @ cheena . net&gt;](endtoend-correlation-groups#cheena-cheena--cheena--net)                                           | 0.01        | 0.05       | 3         | 2               | 2018-12-03     | 1                           |
| [emerson tor@nodevine.net bitcoin:126gyYcBjirRmDh2G](endtoend-correlation-groups#emerson-tornodevinenet-bitcoin126gyycbjirrmdh2g)        | 0.01        | 0.08       | 2         | 2               | 2018-12-04     | 1                           |
| **Total**                                                                                                                                | **0.32**    | **1.76**   | **54**    |                 |                |                             |

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
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |      8.39 |        33 | 2016-09-17   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:14877C6384A9E793F422C8D1DDA447CACA4F7C4B)                         |      6.76 |        15 | 2016-01-25   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |      6.5  |        17 | 2016-02-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |      3.28 |         7 | 2016-12-23   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      2.97 |        13 | 2015-05-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88) |      2.64 |         7 | 2017-10-03   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.31 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      2.17 |        11 | 2017-12-05   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      1.92 |         4 | 2014-11-21   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06) |      1.81 |         7 | 2014-04-08   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                  |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)  |       1.77 |        20 | 2017-06-13   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)      |       1.15 |        19 | 2015-05-16   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)   |       0.97 |        15 | 2016-12-11   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                |       0.92 |         3 | 2015-04-22   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                           |       0.91 |         4 | 2018-08-17   |
| [25C3DEAE](https://metrics.torproject.org/rs.html#search/family:25C3DEAE9AA786559DBB072D0470D1A6FC408846)                                           |       0.79 |        10 | 2018-12-14   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)               |       0.75 |         3 | 2018-04-22   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)               |       0.66 |         8 | 2015-01-29   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324) |       0.64 |         5 | 2014-04-22   |
| [TotorBE AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:25990FC54D7268C914170A118EE4EE75025451DA)                           |       0.63 |         3 | 2016-05-29   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |            2.074 |      8.39 |       0    |        33 | 2016-09-17   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:14877C6384A9E793F422C8D1DDA447CACA4F7C4B)                         |            1.671 |      6.76 |       0    |        15 | 2016-01-25   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            1.607 |      6.5  |       0    |        17 | 2016-02-05   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.085 |      0    |       1.77 |        20 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |            0.811 |      3.28 |       0    |         7 | 2016-12-23   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.733 |      2.97 |       0    |        13 | 2015-05-22   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |            0.718 |      0    |       0.97 |        16 | 2016-10-28   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.708 |      0    |       1.15 |        19 | 2015-05-16   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |            0.696 |      0    |       0.91 |         5 | 2016-09-06   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            0.686 |      0    |       0.64 |         9 | 2014-04-22   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            14.31 |      18.26 |      8.47 |       568 |
| Online S.a.s.               |            13.06 |      17.28 |      6.8  |       331 |
| Hetzner Online GmbH         |            11.43 |      12.89 |      0.37 |       392 |
| Joshua Peter McQuistan      |             3.57 |       0.35 |     13.61 |        35 |
| Quintex Alliance Consulting |             2.07 |       0    |      8.39 |        33 |
| SURFnet bv                  |             1.87 |       1.65 |      3.43 |        24 |
| myLoc managed IT AG         |             1.82 |       2.5  |      0.18 |        40 |
| netcup GmbH                 |             1.75 |       2.3  |      0.11 |        68 |
| DigitalOcean, LLC           |             1.63 |       1.3  |      0.97 |       261 |
| FranTech Solutions          |             1.43 |       0.96 |      2.92 |        41 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.4         |             53.2 |     55.39 |      54.12 |      2942 |
| 0.2.9         |             14.8 |      6.46 |      15.97 |      1292 |
| 0.3.3         |             13.9 |     22.31 |      11.05 |       857 |
| 0.3.5         |              8.5 |     12.95 |       7.56 |       210 |
| 0.3.2         |              5   |      1.12 |       7.24 |       321 |
| 0.2.5         |              1   |      0.37 |       0.89 |       176 |
| 0.4.0         |              1   |      0.48 |       0.86 |        26 |
| 0.3.1         |              0.8 |      0.38 |       1.17 |       103 |
| 0.2.4         |              0.5 |      0.27 |       0.22 |       174 |
| 0.2.7         |              0.3 |      0.01 |       0.41 |       112 |
| 0.3.0         |              0.2 |      0.01 |       0.29 |        53 |
| 0.2.6         |              0.1 |      0.19 |       0.04 |        27 |
| 0.2.8         |              0.1 |      0    |       0.13 |        29 |
| 0.3.6         |              0   |      0    |       0    |         1 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             9.44 |      11.28 |      2.87 |      1022 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.7 |      91.2 |       91.1 |      5804 |
| BSD     |              7.8 |       8.2 |        8.5 |       388 |
| Windows |              0.2 |       0.4 |        0.1 |        85 |
| Darwin  |              0   |       0   |        0   |         9 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            26.87 |       25.9 |       24.78 |     31.55 |       949 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     34.09 |            210 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       428 |
| None                                       |       367 |
| obfs3, obfs4                               |        53 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| fte, meek, obfs3, obfs4                    |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek                                       |         1 |
| obfs2, obfs3                               |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

