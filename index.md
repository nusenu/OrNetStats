---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-12-20 22:00 UTC**

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
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)                                | 0.16        | 0.14       | 8         | 8               | 2018-11-24     | 1                           |
| [&lt;nobody AT example dot com&gt;](endtoend-correlation-groups#nobody-at-example-dot-com)                                               | 0.02        | 0.06       | 2         | 2               | 2018-11-22     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                     | 0.01        | 0.15       | 3         | 2               | 2016-08-28     | 1                           |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](endtoend-correlation-groups#zwiebeln-at-online-de-please-donate-btc-1k38x9xq) | 0.01        | 1.03       | 31        | 9               | 2018-12-05     | 6                           |
| [Cheena &lt;cheena @ cheena . net&gt;](endtoend-correlation-groups#cheena-cheena--cheena--net)                                           | 0.01        | 0.06       | 3         | 2               | 2018-12-03     | 1                           |
| [emerson tor@nodevine.net bitcoin:126gyYcBjirRmDh2G](endtoend-correlation-groups#emerson-tornodevinenet-bitcoin126gyycbjirrmdh2g)        | 0.01        | 0.14       | 2         | 2               | 2018-12-04     | 1                           |
| **Total**                                                                                                                                | **0.22**    | **1.58**   | **49**    |                 |                |                             |

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
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |      9.77 |        50 | 2016-08-22   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |      8.67 |        26 | 2016-02-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      3.15 |        13 | 2015-05-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |      2.74 |         7 | 2016-12-23   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:47C42E2094EE482E7C9B586B10BABFB67557030B)                         |      2.47 |         6 | 2016-01-25   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      2.35 |         4 | 2014-11-21   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88) |      2.34 |         7 | 2017-10-03   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.27 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      2.02 |        11 | 2017-12-05   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06) |      1.96 |         7 | 2014-04-08   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                  |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)  |       1.67 |        20 | 2017-06-13   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)      |       1.16 |        19 | 2015-05-16   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)   |       1.09 |        15 | 2016-12-11   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                |       1.05 |         3 | 2015-04-22   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                |       0.97 |        11 | 2018-01-31   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)               |       0.78 |         3 | 2018-04-22   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799) |       0.75 |         6 | 2014-04-22   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                           |       0.71 |         4 | 2018-08-17   |
| [TotorBE AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:25990FC54D7268C914170A118EE4EE75025451DA)                           |       0.71 |         3 | 2016-05-29   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                           |       0.66 |         5 | 2017-10-24   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |            2.359 |      9.77 |       0    |        50 | 2016-08-22   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.093 |      8.67 |       0    |        26 | 2016-02-05   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.041 |      0    |       1.67 |        20 | 2017-06-13   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |            0.813 |      0    |       1.09 |        16 | 2016-10-28   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.769 |      3.15 |       0.01 |        14 | 2013-08-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.724 |      0    |       1.16 |        19 | 2015-05-16   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            0.703 |      0    |       0.75 |         9 | 2014-04-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |            0.661 |      2.74 |       0    |         7 | 2016-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |            0.658 |      0    |       1.05 |         3 | 2015-04-22   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.609 |      0    |       0.97 |        11 | 2018-01-31   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            14.65 |      18.38 |      9.13 |       562 |
| Online S.a.s.               |            12.66 |      16.01 |      7.03 |       334 |
| Hetzner Online GmbH         |            11.05 |      13.11 |      0.48 |       384 |
| Joshua Peter McQuistan      |             2.99 |       0.32 |     11.57 |        35 |
| Quintex Alliance Consulting |             2.35 |       0    |      9.77 |        50 |
| netcup GmbH                 |             1.94 |       2.66 |      0.13 |        67 |
| myLoc managed IT AG         |             1.83 |       2.4  |      0.19 |        40 |
| SURFnet bv                  |             1.67 |       1.7  |      2.45 |        24 |
| DigitalOcean, LLC           |             1.59 |       1.71 |      0.84 |       244 |
| FranTech Solutions          |             1.59 |       1.02 |      3.53 |        39 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.4         |             53.6 |     57.69 |      54.02 |      2927 |
| 0.2.9         |             14.7 |      6.29 |      15.69 |      1289 |
| 0.3.3         |             13.6 |     20.64 |      10.81 |      1019 |
| 0.3.5         |              7.9 |     12.49 |       7.02 |       213 |
| 0.3.2         |              5.4 |      0.93 |       7.89 |       331 |
| 0.2.5         |              1.1 |      0.47 |       0.88 |       175 |
| 0.4.0         |              1   |      0.65 |       1.31 |        25 |
| 0.3.1         |              0.9 |      0.41 |       1.25 |       108 |
| 0.2.4         |              0.5 |      0.26 |       0.23 |       175 |
| 0.2.7         |              0.3 |      0.02 |       0.37 |       118 |
| 0.3.0         |              0.2 |      0.02 |       0.28 |        54 |
| 0.2.8         |              0.1 |      0    |       0.13 |        30 |
| 0.2.6         |              0   |      0.06 |       0.03 |        27 |
| 0.3.6         |              0   |      0    |       0.01 |         2 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|            10.02 |      12.43 |      2.87 |      1045 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.7 |      91.2 |       90.9 |      5971 |
| BSD     |              7.8 |       8.2 |        8.7 |       384 |
| Windows |              0.2 |       0.4 |        0.1 |        90 |
| Darwin  |              0   |       0   |        0   |        13 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            27.74 |      26.01 |       25.87 |     33.39 |       974 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     35.88 |            227 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       489 |
| None                                       |       360 |
| obfs3, obfs4                               |        50 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| fte, meek, obfs3, obfs4                    |         2 |
| obfs2, obfs3                               |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek                                       |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

