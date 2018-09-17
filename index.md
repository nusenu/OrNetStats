---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-09-17 07:00 UTC**

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
| [abuse-node49 AT posteo DOT de](endtoend-correlation-groups#abuse-node49-at-posteo-dot-de)                     | 0.07        | 1.35       | 7         | 6               | 2018-09-05     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca) | 0.05        | 0.32       | 7         | 2               | 2018-02-11     | 5                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)           | 0.03        | 0.11       | 3         | 2               | 2016-08-28     | 1                           |
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)      | 0.02        | 0.13       | 3         | 3               | 2018-08-17     | 1                           |
| **Total**                                                                                                      | **0.17**    | **1.91**   | **20**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |      8.37 |        26 | 2016-01-25   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      3.22 |        13 | 2015-05-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |      2.98 |         7 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.88 |         1 | 2014-04-19   |
| [Relay Control &lt;office AT universalipsolution dot b](https://metrics.torproject.org/rs.html#search/family:0C2D910C87E9197878C005021E8BF4D2AF0FF17C) |      2.53 |        20 | 2018-07-10   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      2.35 |         4 | 2014-11-21   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      2.31 |        11 | 2017-12-05   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)   |      2.14 |         7 | 2014-04-09   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06) |      2.03 |         6 | 2014-04-08   |
| [admin&lt;AT&gt;tor4us.net](https://metrics.torproject.org/rs.html#search/family:1A0910312F40BDA7329B71A9E88F887545736458)                             |      1.68 |         3 | 2018-02-24   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |       1.72 |        19 | 2017-06-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |       1.66 |         7 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       1.26 |         3 | 2015-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       1.04 |        17 | 2015-05-16   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.85 |         7 | 2016-01-03   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                  |       0.84 |         3 | 2018-04-22   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |       0.83 |         8 | 2015-01-29   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |       0.77 |         9 | 2016-12-11   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.74 |         5 | 2017-10-24   |
| [max@zamax.fr](https://metrics.torproject.org/rs.html#details/E34F2CEE28981A64132D7EDBE8DD5EC546B64071)                                                |       0.7  |         1 | 2018-03-08   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            1.921 |      8.37 |       0    |        26 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.238 |      0.73 |       1.72 |        20 | 2017-06-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            1.03  |      0    |       1.66 |         7 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |            0.784 |      0    |       1.26 |         3 | 2015-04-22   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.748 |      3.22 |       0.01 |        14 | 2013-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |            0.684 |      2.98 |       0    |         7 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.662 |      2.88 |       0    |         1 | 2014-04-19   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.647 |      0    |       1.04 |        17 | 2015-05-16   |
| [Relay Control &lt;office AT universalipsolution dot b](https://metrics.torproject.org/rs.html#search/family:0C2D910C87E9197878C005021E8BF4D2AF0FF17C) |            0.582 |      2.53 |       0    |        20 | 2018-07-10   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |            0.581 |      0    |       0.77 |        10 | 2016-10-28   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                |            14.41 |      16.99 |     13.29 |       560 |
| Online S.a.s.          |            13.45 |      16.49 |      6.68 |       337 |
| Hetzner Online GmbH    |             8.59 |       7.97 |      0.67 |       353 |
| myLoc managed IT AG    |             2.68 |       3.01 |      1.9  |        42 |
| Joshua Peter McQuistan |             2.27 |       0.05 |      8.42 |        30 |
| SURFnet bv             |             2.17 |       2.32 |      3.19 |        24 |
| FranTech Solutions     |             1.9  |       1.27 |      4.81 |        43 |
| netcup GmbH            |             1.83 |       2.05 |      0.73 |        51 |
| Host Europe GmbH       |             1.63 |       2.49 |      0    |        37 |
| DigitalOcean, LLC      |             1.3  |       1.24 |      0.25 |       203 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.3         |             41.3 |     57.74 |      37.58 |      2103 |
| 0.3.4         |             23.9 |     21.51 |      27.4  |      1128 |
| 0.2.9         |             15.9 |      9.92 |      15.98 |      1378 |
| 0.3.2         |             12.1 |      5.88 |      13.66 |       899 |
| 0.3.1         |              2.4 |      3.3  |       2.35 |       202 |
| 0.2.5         |              1.5 |      0.84 |       1.18 |       226 |
| 0.2.4         |              1.4 |      0.52 |       0.52 |       182 |
| 0.2.7         |              0.4 |      0.04 |       0.34 |       140 |
| 0.3.0         |              0.2 |      0.05 |       0.39 |        69 |
| 0.2.8         |              0.1 |      0    |       0.26 |        28 |
| 0.3.5         |              0.1 |      0.12 |       0.23 |        12 |
| 0.2.6         |              0   |      0.01 |       0.06 |        23 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.97 |       2.77 |      1.49 |       668 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.2 |      87   |       89.9 |      5869 |
| BSD     |              9.4 |      12.6 |        9.7 |       387 |
| Windows |              0.1 |       0.2 |        0   |        76 |
| SunOS   |              0.1 |       0   |        0.1 |         5 |
| Darwin  |              0   |       0   |        0   |        16 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|             25.7 |      23.88 |       22.55 |     34.04 |       870 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     37.79 |            207 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       373 |
| None                                       |       313 |
| obfs3, obfs4                               |        47 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3, obfs4                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3                                      |         5 |
| meek                                       |         2 |
| obfs3, obfs4, scramblesuit                 |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, obfs4                          |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

