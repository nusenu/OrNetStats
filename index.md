---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-01-14 16:00 UTC**

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
| [abuse@to-surf-and-protect.net](endtoend-correlation-groups#abuseto-surf-and-protectnet)                                         | 0.19        | 9.02       | 39        | 3               | 2019-01-05     | 35                          |
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)                        | 0.16        | 0.13       | 7         | 7               | 2018-12-23     | 1                           |
| [con at fynn dot sh tor-relay.co](endtoend-correlation-groups#conatfynndotsh-tor-relayco)                                        | 0.06        | 0.13       | 3         | 3               | 2019-01-07     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                             | 0.04        | 0.14       | 3         | 2               | 2016-08-28     | 1                           |
| [&lt;schneider&gt; schneiderweisse AT tutanota DOT de](endtoend-correlation-groups#schneider-schneiderweisse-at-tutanota-dot-de) | 0.02        | 0.09       | 3         | 3               | 2015-09-17     | 1                           |
| [&lt;nobody AT example dot com&gt;](endtoend-correlation-groups#nobody-at-example-dot-com)                                       | 0.01        | 0.07       | 2         | 2               | 2018-11-22     | 1                           |
| **Total**                                                                                                                        | **0.48**    | **9.58**   | **57**    |                 |                |                             |

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
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |     10.22 |        50 | 2016-08-22   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |      8.62 |        32 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |      5.96 |        17 | 2016-12-23   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |      4.99 |         6 | 2018-04-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      2.88 |        13 | 2015-05-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.53 |         1 | 2014-04-19   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06) |      2    |         7 | 2014-04-08   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      1.97 |        11 | 2017-12-05   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A) |      1.72 |         7 | 2018-04-25   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      1.45 |         4 | 2014-11-21   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:0D12D8E72DED99EE31BB0C57789352BED0CEEEFF)     |       1.2  |        14 | 2017-06-13   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |       1.02 |        13 | 2016-12-11   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       0.98 |        19 | 2015-05-16   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.86 |         3 | 2015-04-22   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.78 |         5 | 2017-10-24   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:01FD173C0AFD8137A21F0B28DC2DB1329DF0F529)           |       0.72 |        12 | 2018-01-07   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |       0.72 |         8 | 2015-01-29   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                  |       0.69 |         3 | 2018-04-22   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |       0.65 |         4 | 2018-08-17   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.65 |         8 | 2016-01-03   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |            2.357 |     10.22 |       0    |        50 | 2016-08-22   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            1.99  |      8.62 |       0    |        32 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.929 |      4.99 |       1.2  |        20 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |            1.376 |      5.96 |       0    |        17 | 2016-12-23   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |            0.768 |      0    |       1.02 |        15 | 2016-10-28   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.736 |      0    |       0.6  |        12 | 2018-01-31   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.664 |      2.88 |       0    |        13 | 2015-05-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.631 |      0    |       0.98 |        19 | 2015-05-16   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.584 |      2.53 |       0    |         1 | 2014-04-19   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |            0.559 |      0    |       0.86 |         3 | 2015-04-22   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                                                          |            14.26 |      17.66 |      9.52 |       570 |
| Online S.a.s.                                                    |            12.76 |      16.6  |      6.35 |       367 |
| Hetzner Online GmbH                                              |            11.36 |      13.02 |      0.43 |       391 |
| Quintex Alliance Consulting                                      |             2.35 |       0    |     10.22 |        50 |
| netcup GmbH                                                      |             2.31 |       2.88 |      0.09 |        72 |
| Joshua Peter McQuistan                                           |             2.24 |       0.31 |      8.87 |        35 |
| DigitalOcean, LLC                                                |             1.92 |       1.75 |      0.53 |       246 |
| myLoc managed IT AG                                              |             1.84 |       2.71 |      0.18 |        42 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             1.83 |       1.06 |      4.99 |        17 |
| SURFnet bv                                                       |             1.79 |       1.54 |      3.4  |        25 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.4         |             42.6 |     42.83 |      43.62 |      2610 |
| 0.3.5         |             23.4 |     32.07 |      21.62 |      1147 |
| 0.2.9         |             14.1 |      8.45 |      14.36 |      1290 |
| 0.3.3         |             10.5 |     14.19 |       9.71 |       588 |
| 0.3.2         |              4.8 |      1.29 |       6.27 |       302 |
| 0.4.0         |              1.3 |      0    |       1.52 |        26 |
| 0.2.5         |              0.9 |      0.56 |       0.72 |       167 |
| 0.3.1         |              0.8 |      0.23 |       1.12 |        95 |
| 0.2.4         |              0.4 |      0.3  |       0.26 |       179 |
| 0.2.7         |              0.3 |      0.02 |       0.31 |       109 |
| 0.3.0         |              0.2 |      0.02 |       0.3  |        58 |
| 0.2.6         |              0   |      0    |       0.03 |        22 |
| 0.2.8         |              0   |      0    |       0.09 |        26 |
| 0.3.6         |              0   |      0    |       0    |         1 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             7.86 |       9.14 |      2.44 |       959 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91   |      87.3 |       91.6 |      6067 |
| BSD     |              8.5 |      12.2 |        8   |       383 |
| Windows |              0.2 |       0.3 |        0.1 |        96 |
| Darwin  |              0   |       0   |        0   |        14 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|             28.3 |       25.6 |       25.05 |     38.23 |      1006 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|      41.1 |            232 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       490 |
| None                                       |       376 |
| obfs3, obfs4                               |        51 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         3 |
| fte, meek, obfs3, obfs4                    |         2 |
| meek                                       |         2 |
| obfs2, obfs3                               |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

