---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-01-03 15:00 UTC**

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

| Contact                                                                                                                          | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:---------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)                        | 0.15        | 0.12       | 8         | 8               | 2018-12-23     | 1                           |
| [sysop at openinternet.io BTC: 1LZCkCZRqJ3fXnVqCBrq](endtoend-correlation-groups#sysopatopeninternetio-btc-1lzckczrqj3fxnvqcbrq) | 0.07        | 0.24       | 2         | 2               | 2018-12-16     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                             | 0.02        | 0.09       | 3         | 2               | 2016-08-28     | 1                           |
| [&lt;schneider&gt; schneiderweisse AT tutanota DOT de](endtoend-correlation-groups#schneider-schneiderweisse-at-tutanota-dot-de) | 0.02        | 0.08       | 3         | 3               | 2015-09-17     | 1                           |
| [&lt;nobody AT example dot com&gt;](endtoend-correlation-groups#nobody-at-example-dot-com)                                       | 0.01        | 0.07       | 2         | 2               | 2018-11-22     | 1                           |
| **Total**                                                                                                                        | **0.27**    | **0.60**   | **18**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |     11.91 |        35 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      8.51 |        50 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC)    |      3.29 |         7 | 2016-12-23   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      2.89 |        13 | 2015-05-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88)    |      2.36 |         7 | 2017-10-03   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.32 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      2.14 |        11 | 2017-12-05   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      1.97 |         6 | 2018-04-05   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      1.91 |         4 | 2014-11-21   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      1.78 |        12 | 2013-06-11   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                 |   Guard(%) |   #Relays | First Seen   |
|:---------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:0D12D8E72DED99EE31BB0C57789352BED0CEEEFF) |       1.18 |        14 | 2017-06-13   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)     |       1.06 |        19 | 2015-05-16   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)  |       1.03 |        15 | 2016-12-11   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)               |       1    |         3 | 2015-04-22   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                          |       0.87 |         4 | 2018-08-17   |
| [25C3DEAE](https://metrics.torproject.org/rs.html#search/family:25C3DEAE9AA786559DBB072D0470D1A6FC408846)                                          |       0.81 |        10 | 2018-12-14   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)              |       0.75 |         3 | 2018-04-22   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:01FD173C0AFD8137A21F0B28DC2DB1329DF0F529)       |       0.69 |        12 | 2018-01-07   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                          |       0.66 |         5 | 2017-10-24   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)              |       0.65 |         8 | 2015-01-29   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.986 |     11.91 |       0    |        35 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |            2.133 |      8.51 |       0    |        50 | 2016-08-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.231 |      1.97 |       1.18 |        20 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |            0.825 |      3.29 |       0    |         7 | 2016-12-23   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |            0.768 |      0    |       1.03 |        16 | 2016-10-28   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.726 |      2.89 |       0    |        13 | 2015-05-22   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.725 |      0    |       0.63 |        12 | 2018-01-31   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |            0.704 |      0    |       0.87 |         5 | 2016-09-06   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.658 |      0    |       1.06 |        19 | 2015-05-16   |
| [Ignitus Cryptonanus &lt;cryptonanus AT protonmail dot](https://metrics.torproject.org/rs.html#search/family:0F08870BB1EB436C852F3767F79B367E584B0E7E) |            0.634 |      0    |       0    |        22 | 2018-11-09   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            14.12 |      17.54 |      8.82 |       568 |
| Online S.a.s.               |            12.88 |      16.91 |      6.28 |       340 |
| Hetzner Online GmbH         |            12.11 |      13.87 |      0.52 |       400 |
| Joshua Peter McQuistan      |             3.09 |       0.34 |     11.45 |        36 |
| Quintex Alliance Consulting |             2.13 |       0    |      8.51 |        50 |
| netcup GmbH                 |             2.05 |       2.68 |      0.11 |        74 |
| myLoc managed IT AG         |             1.88 |       2.9  |      0.15 |        41 |
| SURFnet bv                  |             1.8  |       1.71 |      2.9  |        25 |
| DigitalOcean, LLC           |             1.72 |       1.69 |      0.91 |       256 |
| FranTech Solutions          |             1.52 |       1.02 |      3.5  |        43 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.4         |             55.5 |     57.16 |      56.4  |      3035 |
| 0.2.9         |             14   |      6.26 |      15.41 |      1309 |
| 0.3.3         |             12.3 |     19.1  |      10.5  |       640 |
| 0.3.5         |              8.5 |     14.22 |       6.98 |       224 |
| 0.3.2         |              4.9 |      1.62 |       6.86 |       322 |
| 0.2.5         |              1.1 |      0.57 |       0.84 |       182 |
| 0.4.0         |              1.1 |      0.64 |       0.91 |        28 |
| 0.3.1         |              0.9 |      0.22 |       1.1  |        97 |
| 0.2.4         |              0.6 |      0.17 |       0.26 |       176 |
| 0.2.7         |              0.3 |      0.01 |       0.3  |       112 |
| 0.3.0         |              0.2 |      0.02 |       0.28 |        55 |
| 0.2.6         |              0   |      0    |       0.04 |        22 |
| 0.2.8         |              0   |      0    |       0.09 |        26 |
| 0.3.6         |              0   |      0    |       0    |         1 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             8.28 |        9.8 |      2.64 |       993 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.7 |      89.8 |       91.9 |      5682 |
| BSD     |              7.8 |       9.8 |        7.7 |       390 |
| Windows |              0.2 |       0.2 |        0.1 |        90 |
| SunOS   |              0   |       0   |        0   |         5 |
| Darwin  |              0   |       0   |        0   |        11 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            27.33 |      25.87 |       25.51 |     32.24 |       992 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     35.21 |            232 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| None                                       |       366 |
| obfs4                                      |       350 |
| obfs3, obfs4                               |        51 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| obfs2, obfs3                               |         3 |
| fte, meek, obfs3, obfs4                    |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek                                       |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

