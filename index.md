---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-11-22 09:00 UTC**

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

| Contact                                                                                                   | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:----------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain) | 0.18        | 0.13       | 8         | 8               | 2018-11-08     | 1                           |
| [tor@sechsnulldrei.org](endtoend-correlation-groups#torsechsnulldreiorg)                                  | 0.03        | 0.16       | 4         | 2               | 2018-10-19     | 2                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)      | 0.02        | 0.13       | 3         | 2               | 2016-08-28     | 1                           |
| **Total**                                                                                                 | **0.23**    | **0.42**   | **15**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |      9.15 |        27 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:4BFC9C631A93FF4BA3AA84BC6931B4310C38A263)        |      3.89 |         3 | 2018-04-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      3.56 |        13 | 2015-05-22   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:1E5136DDC52FAE1219208F0A6BADB0BA62587EE6)    |      3.47 |        10 | 2017-09-14   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.88 |         1 | 2014-04-19   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC)    |      2.85 |         7 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      2.3  |        11 | 2017-12-05   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:93FAB6F91C2EF33D0ACEEF7448177FCA2CEB99A0)      |      1.95 |         5 | 2016-01-22   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://metrics.torproject.org/rs.html#search/family:185663B7C12777F052B2C2D23D7A239D8DA88A0F) |      1.93 |         5 | 2011-10-06   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      1.91 |         4 | 2014-11-21   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                  |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)  |       1.57 |        17 | 2017-06-13   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                |       1.16 |         3 | 2015-04-22   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324) |       0.99 |         5 | 2014-04-22   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                |       0.92 |        11 | 2018-01-31   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)               |       0.76 |         8 | 2015-01-29   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                           |       0.75 |         5 | 2017-10-24   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                           |       0.73 |         4 | 2018-08-17   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)               |       0.72 |         3 | 2018-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)      |       0.72 |        19 | 2015-05-16   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)   |       0.66 |        12 | 2016-12-11   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.142 |      9.15 |       0    |        27 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.889 |      3.89 |       1.57 |        20 | 2017-06-13   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.845 |      3.56 |       0.01 |        14 | 2013-08-22   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:1E5136DDC52FAE1219208F0A6BADB0BA62587EE6) |            0.812 |      3.47 |       0    |        10 | 2017-09-14   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            0.739 |      0    |       0.99 |         7 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |            0.721 |      0    |       1.16 |         3 | 2015-04-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.676 |      2.88 |       0    |         1 | 2014-04-19   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |            0.668 |      2.85 |       0    |         7 | 2016-12-23   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.573 |      0    |       0.92 |        11 | 2018-01-31   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |            0.55  |      0    |       0.66 |        14 | 2016-10-28   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                                                          |            14.89 |      17.88 |     11.49 |       567 |
| Online S.a.s.                                                    |            14.1  |      17.43 |      6.79 |       359 |
| Hetzner Online GmbH                                              |            10.43 |      11.7  |      0.47 |       372 |
| Joshua Peter McQuistan                                           |             2.45 |       0.32 |      9.62 |        31 |
| myLoc managed IT AG                                              |             2.18 |       3.07 |      0.79 |        40 |
| SURFnet bv                                                       |             1.9  |       1.95 |      2.97 |        24 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             1.76 |       1.36 |      3.89 |        17 |
| DigitalOcean, LLC                                                |             1.54 |       1.29 |      0.79 |       253 |
| netcup GmbH                                                      |             1.47 |       1.92 |      0.16 |        60 |
| FranTech Solutions                                               |             1.37 |       0.88 |      3.28 |        44 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.4         |             50.8 |     58.88 |      49.88 |      2622 |
| 0.3.3         |             15.3 |     19.89 |      13.57 |      1053 |
| 0.2.9         |             14.7 |      6.4  |      16.26 |      1280 |
| 0.3.2         |              8   |      3.44 |       9.7  |       417 |
| 0.3.5         |              6.3 |      9.59 |       6.13 |       168 |
| 0.2.5         |              1   |      0.72 |       0.83 |       186 |
| 0.3.1         |              1   |      0.55 |       1.41 |       117 |
| 0.2.4         |              0.9 |      0.3  |       0.26 |       179 |
| 0.4.0         |              0.6 |      0.08 |       1.07 |        18 |
| 0.2.7         |              0.3 |      0.04 |       0.37 |       119 |
| 0.3.0         |              0.2 |      0.02 |       0.21 |        70 |
| 0.2.8         |              0.1 |      0    |       0.16 |        29 |
| 0.2.6         |              0   |      0.02 |       0.05 |        26 |
| 0.3.6         |              0   |      0    |       0.04 |         4 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|            12.71 |      14.14 |      5.22 |      1165 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90   |      84.3 |       91   |      5748 |
| BSD     |              9.3 |      14.8 |        8.6 |       396 |
| Windows |              0.3 |       0.7 |        0   |        95 |
| Darwin  |              0   |       0   |        0   |        11 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            26.76 |      25.84 |       24.36 |     32.21 |       936 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     36.25 |            194 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       426 |
| None                                       |       371 |
| obfs3, obfs4                               |        49 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| obfs3, scramblesuit                        |         3 |
| fte, meek, obfs3, obfs4                    |         2 |
| fte, obfs4                                 |         2 |
| obfs2, obfs3                               |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3                                 |         1 |
| meek                                       |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

