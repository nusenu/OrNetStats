---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-10-01 08:00 UTC**

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
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca) | 0.07        | 0.31       | 7         | 2               | 2018-02-11     | 5                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)           | 0.02        | 0.14       | 3         | 2               | 2016-08-28     | 1                           |
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)      | 0.01        | 0.14       | 2         | 2               | 2018-08-15     | 1                           |
| **Total**                                                                                                      | **0.10**    | **0.59**   | **12**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |      9.86 |        26 | 2016-01-25   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      3.24 |        13 | 2015-05-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)      |      3.02 |         7 | 2014-04-09   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.83 |         1 | 2014-04-19   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC)    |      2.22 |         7 | 2016-12-23   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      2.17 |         4 | 2014-11-21   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      2.13 |        11 | 2017-12-05   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06)    |      1.69 |         6 | 2014-04-08   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      1.61 |         7 | 2018-04-25   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://metrics.torproject.org/rs.html#search/family:185663B7C12777F052B2C2D23D7A239D8DA88A0F) |      1.51 |         5 | 2011-10-06   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |       2.04 |        19 | 2017-06-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |       1.71 |         7 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       1.12 |         3 | 2015-04-22   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |       0.85 |         9 | 2016-12-11   |
| [jwbecher@drazisil.com](https://metrics.torproject.org/rs.html#search/family:46FBC671FD6FCE6B298B2BAE3C7AC7D7DDF1365F)                                 |       0.83 |         6 | 2018-05-08   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       0.78 |        17 | 2015-05-16   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |       0.76 |         8 | 2015-01-29   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.7  |         6 | 2016-01-03   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.69 |         5 | 2017-10-24   |
| [TotorBE AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:25990FC54D7268C914170A118EE4EE75025451DA)                              |       0.65 |         2 | 2016-10-22   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.377 |      9.86 |       0    |        26 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.481 |      1.04 |       2.04 |        20 | 2017-06-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            1.034 |      0    |       1.71 |         7 | 2014-04-22   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.79  |      3.24 |       0.01 |        14 | 2013-08-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)   |            0.73  |      3.02 |       0    |         7 | 2014-04-09   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.684 |      2.83 |       0    |         1 | 2014-04-19   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |            0.679 |      0    |       1.12 |         3 | 2015-04-22   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |            0.632 |      0    |       0.85 |        10 | 2016-10-28   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |            0.536 |      2.22 |       0    |         7 | 2016-12-23   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.523 |      2.17 |       0    |         4 | 2014-11-21   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------|-----------------:|-----------:|----------:|----------:|
| Online S.a.s.          |            13.66 |      18.68 |      6.31 |       335 |
| OVH SAS                |            13.59 |      16.86 |     10.85 |       538 |
| Hetzner Online GmbH    |             8.56 |       7.57 |      0.72 |       351 |
| Joshua Peter McQuistan |             2.79 |       0.51 |     10.31 |        31 |
| myLoc managed IT AG    |             2.35 |       2.32 |      2.36 |        44 |
| SURFnet bv             |             2.11 |       2    |      3.74 |        23 |
| FranTech Solutions     |             1.73 |       1.27 |      3.73 |        45 |
| netcup GmbH            |             1.72 |       2.12 |      0.2  |        48 |
| Private Layer INC      |             1.6  |       0.64 |      4.26 |        46 |
| Host Europe GmbH       |             1.53 |       2.4  |      0    |        36 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.4         |             36.3 |     38.59 |      38.25 |      1822 |
| 0.3.3         |             29.3 |     41.34 |      25.61 |      1470 |
| 0.2.9         |             15.1 |      8.92 |      15.87 |      1354 |
| 0.3.2         |             10.7 |      4.78 |      12.91 |       855 |
| 0.3.5         |              2.6 |      2.28 |       2.85 |        63 |
| 0.3.1         |              2.3 |      2.84 |       2.24 |       178 |
| 0.2.5         |              1.3 |      0.95 |       0.91 |       224 |
| 0.2.4         |              1.2 |      0.18 |       0.41 |       189 |
| 0.2.7         |              0.4 |      0.03 |       0.46 |       141 |
| 0.3.0         |              0.2 |      0.02 |       0.24 |        63 |
| 0.2.8         |              0.1 |      0    |       0.13 |        30 |
| 0.2.6         |              0   |      0.01 |       0.04 |        25 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.38 |       2.23 |      1.21 |       672 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.3 |      88   |       90   |      5880 |
| BSD     |              9.2 |      11.4 |        9.5 |       393 |
| Windows |              0.2 |       0.3 |        0   |        93 |
| Darwin  |              0   |       0   |        0   |        13 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            25.48 |      23.73 |       23.73 |     31.01 |       869 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     32.98 |            191 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       387 |
| None                                       |       315 |
| obfs3, obfs4                               |        50 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3                                      |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         3 |
| fte, obfs3, obfs4                          |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| meek                                       |         1 |
| obfs2, obfs3                               |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

