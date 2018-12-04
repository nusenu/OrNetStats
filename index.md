---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-12-04 20:00 UTC**

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
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)                                | 0.19        | 0.19       | 9         | 9               | 2018-11-24     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                     | 0.02        | 0.17       | 3         | 2               | 2016-08-28     | 1                           |
| [&lt;nobody AT example dot com&gt;](endtoend-correlation-groups#nobody-at-example-dot-com)                                               | 0.02        | 0.08       | 2         | 2               | 2018-11-22     | 1                           |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](endtoend-correlation-groups#zwiebeln-at-online-de-please-donate-btc-1k38x9xq) | 0.02        | 0.87       | 27        | 7               | 2018-11-20     | 15                          |
| [wgetdataatprotonmailch tor-relay.co](endtoend-correlation-groups#wgetdataatprotonmailch-tor-relayco)                                    | 0.02        | 0.06       | 2         | 2               | 2018-09-17     | 1                           |
| [tech@emeraldonion.org](endtoend-correlation-groups#techemeraldonionorg)                                                                 | 0.01        | 0.23       | 4         | 2               | 2018-11-19     | 1                           |
| **Total**                                                                                                                                | **0.28**    | **1.60**   | **47**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |     12.63 |        27 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:1E5136DDC52FAE1219208F0A6BADB0BA62587EE6)    |      4.1  |        10 | 2017-09-14   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:4BFC9C631A93FF4BA3AA84BC6931B4310C38A263)        |      3.84 |         3 | 2018-04-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      3.41 |        13 | 2015-05-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC)    |      2.71 |         7 | 2016-12-23   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      2.62 |         4 | 2014-11-21   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.44 |         1 | 2014-04-19   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      1.79 |        12 | 2013-06-11   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:93FAB6F91C2EF33D0ACEEF7448177FCA2CEB99A0)      |      1.74 |         5 | 2016-01-22   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06)    |      1.71 |         7 | 2014-04-08   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |       1.32 |        17 | 2017-06-13   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |       1.24 |        11 | 2018-01-31   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)       |       0.89 |         7 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                      |       0.88 |         3 | 2015-04-22   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)         |       0.83 |        14 | 2016-12-11   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)            |       0.78 |        16 | 2015-05-16   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                                 |       0.76 |         4 | 2018-08-17   |
| [TheEpTic &lt;torrelay@eptic.me&gt; - BTC: 18HoXqpoVicNs5](https://metrics.torproject.org/rs.html#search/family:4204C1B166CCE784CF38B02E4A0C94640A2BECA2) |       0.69 |         6 | 2017-03-29   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                     |       0.68 |         8 | 2015-01-29   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://metrics.torproject.org/rs.html#search/family:13557448AD1632BF080757C2FF7769BB23DF1DF3) |       0.65 |         7 | 2014-04-09   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.598 |     12.63 |       0    |        27 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.637 |      3.84 |       1.32 |        20 | 2017-06-13   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:1E5136DDC52FAE1219208F0A6BADB0BA62587EE6) |            0.843 |      4.1  |       0    |        10 | 2017-09-14   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.794 |      0    |       1.24 |        11 | 2018-01-31   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.729 |      0    |       0.78 |        19 | 2015-05-16   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.712 |      3.41 |       0.01 |        14 | 2013-08-22   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |            0.696 |      0    |       0.83 |        16 | 2016-10-28   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            0.692 |      0    |       0.89 |         9 | 2014-04-22   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |            0.583 |      0    |       0.76 |         5 | 2016-09-06   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |            0.561 |      0    |       0.88 |         3 | 2015-04-22   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                                                          |            14.19 |      17.7  |      9.35 |       552 |
| Online S.a.s.                                                    |            14.17 |      17.49 |      8.2  |       354 |
| Hetzner Online GmbH                                              |            11.63 |      12.14 |      0.99 |       388 |
| Joshua Peter McQuistan                                           |             2.87 |       0.24 |     13.23 |        30 |
| netcup GmbH                                                      |             2.02 |       2.39 |      0.12 |        64 |
| myLoc managed IT AG                                              |             1.7  |       2.35 |      0.19 |        37 |
| DigitalOcean, LLC                                                |             1.6  |       1.23 |      1.14 |       257 |
| SURFnet bv                                                       |             1.55 |       1.62 |      2.55 |        24 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             1.51 |       1.13 |      3.84 |        17 |
| FranTech Solutions                                               |             1.39 |       1.06 |      3.16 |        43 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.4         |             55.4 |     71.11 |      53.32 |      2777 |
| 0.2.9         |             15.2 |      6.48 |      16.64 |      1304 |
| 0.3.3         |             12.1 |     11    |      12.06 |      1123 |
| 0.3.2         |              6.4 |      1.53 |       7.6  |       369 |
| 0.3.5         |              6.1 |      8.7  |       5.68 |       181 |
| 0.3.1         |              1.1 |      0.48 |       1.27 |       115 |
| 0.4.0         |              1   |      0.07 |       1.45 |        20 |
| 0.2.5         |              0.9 |      0.22 |       0.85 |       197 |
| 0.2.4         |              0.6 |      0.29 |       0.25 |       179 |
| 0.2.7         |              0.3 |      0.01 |       0.34 |       119 |
| 0.3.0         |              0.2 |      0.03 |       0.3  |        58 |
| 0.2.8         |              0.1 |      0    |       0.13 |        32 |
| 0.2.6         |              0   |      0.02 |       0.03 |        28 |
| 0.3.6         |              0   |      0    |       0.01 |         2 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|            11.02 |      12.28 |      2.68 |      1119 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.7 |      86   |       91.3 |      5957 |
| BSD     |              8.8 |      13.2 |        8.4 |       387 |
| Windows |              0.3 |       0.5 |        0   |       103 |
| SunOS   |              0.1 |       0   |        0.1 |         5 |
| Darwin  |              0   |       0   |        0   |        11 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            25.81 |      25.68 |       24.93 |     27.76 |       912 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     27.88 |            179 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       480 |
| None                                       |       376 |
| obfs3, obfs4                               |        52 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| obfs2, obfs3                               |         3 |
| fte, meek, obfs3, obfs4                    |         2 |
| fte, obfs4                                 |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| meek                                       |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

