---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-06-12 21:00 UTC**

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
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain) | 0.15        | 0.17       | 7         | 7               | 2019-05-29     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)      | 0.02        | 0.09       | 3         | 2               | 2016-08-28     | 1                           |
| **Total**                                                                                                 | **0.17**    | **0.26**   | **10**    |                 |                |                             |

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
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |     11.45 |        50 | 2016-08-22   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                         |     10.03 |        42 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |      6.2  |        17 | 2016-12-23   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |      5.33 |        10 | 2018-03-23   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                 |      3.34 |        54 | 2019-04-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      2.16 |        13 | 2015-05-22   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A) |      1.88 |        15 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      1.84 |         4 | 2014-11-21   |
| [abuse@f3netze.de](https://metrics.torproject.org/rs.html#search/family:6BCB964AB74E23F8986BDA905697D3A6BE08AF28)                                      |      1.76 |         4 | 2018-03-21   |
| [tor-operator@privateinternetaccess.com](https://metrics.torproject.org/rs.html#search/family:3F62F05E859D7F98B086F702A31F7714D566E49A)                |      1.67 |         5 | 2018-12-11   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                 |   Guard(%) |   #Relays | First Seen   |
|:---------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                     |       1.5  |        16 | 2019-01-05   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)               |       0.85 |         4 | 2018-09-25   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                          |       0.85 |         4 | 2018-08-17   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)               |       0.78 |         3 | 2015-04-22   |
| [email:tor appliedprivacy.net twitter:applied priv](https://metrics.torproject.org/rs.html#search/family:113143469021882C3A4B82F084F8125B08EE471E) |       0.75 |         9 | 2017-06-13   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:3B4C5729F829CA2E895B81AF834A63DB336D0FFE)       |       0.65 |        13 | 2018-01-07   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:39F91959416763AFD34DBEEC05474411B964B2DC)                              |       0.61 |        20 | 2018-08-28   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:0C475BA4D3AA3C289B716F95954CAD616E50C4E5)     |       0.58 |        14 | 2015-05-16   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)              |       0.58 |         3 | 2018-04-22   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)               |       0.54 |         4 | 2018-10-05   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                         |            3.39  |     10.03 |       1.5  |        58 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |            2.761 |     11.45 |       0    |        50 | 2016-08-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.775 |      5.33 |       0.75 |        19 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |            1.495 |      6.2  |       0    |        17 | 2016-12-23   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                 |            0.816 |      3.34 |       0    |        55 | 2019-04-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.689 |      0    |       0.54 |         8 | 2018-10-05   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |            0.585 |      0    |       0.85 |         5 | 2016-09-06   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                   |            0.551 |      0    |       0.85 |         4 | 2018-09-25   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.522 |      2.16 |       0    |        13 | 2015-05-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |            0.506 |      0    |       0.78 |         3 | 2015-04-22   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH                                              |            15.55 |      19.78 |      0.07 |       405 |
| OVH SAS                                                          |            15.15 |      18.1  |     12.17 |       588 |
| Online S.a.s.                                                    |             9.89 |      12.72 |      3.91 |       299 |
| iomart Cloud Services Limited.                                   |             2.94 |       3.56 |      0    |        20 |
| Quintex Alliance Consulting                                      |             2.76 |       0    |     11.45 |        50 |
| Joshua Peter McQuistan                                           |             2.49 |       0.1  |     10.03 |        46 |
| netcup GmbH                                                      |             2.43 |       3.27 |      0.11 |        78 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             1.69 |       0.63 |      5.33 |        18 |
| 1&amp;1 Internet SE                                              |             1.55 |       1.99 |      0.09 |        33 |
| NForce Entertainment B.V.                                        |             1.46 |       1.13 |      2.94 |        30 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.5         |             51.5 |     55.16 |      50.13 |      3116 |
| 0.4.0         |             16.5 |     23.66 |      15.53 |       752 |
| 0.3.4         |             13.7 |      4.87 |      17.27 |       817 |
| 0.2.9         |              8.8 |      3.46 |       9.97 |       993 |
| 0.3.2         |              4.3 |     10.6  |       2.47 |       227 |
| 0.4.1         |              2.2 |      0.94 |       1.98 |        79 |
| 0.3.3         |              1.5 |      0.71 |       1.65 |       174 |
| 0.2.5         |              0.3 |      0.28 |       0.17 |       108 |
| 0.3.1         |              0.3 |      0.13 |       0.38 |        55 |
| 0.2.4         |              0.2 |      0.05 |       0.08 |       116 |
| 0.4.2         |              0.1 |      0.09 |       0.15 |         5 |
| 0.2.6         |              0   |      0    |       0.02 |        25 |
| 0.2.7         |              0   |      0    |       0.03 |        63 |
| 0.2.8         |              0   |      0    |       0    |        15 |
| 0.3.0         |              0   |      0    |       0.09 |        57 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             6.97 |       4.92 |     11.78 |       840 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.2 |      87.4 |       93.4 |      6020 |
| BSD     |              7.4 |      12.4 |        6.1 |       454 |
| Windows |              0.1 |       0   |        0.1 |        85 |
| SunOS   |              0   |       0   |        0   |         4 |
| Darwin  |              0   |       0   |        0.1 |        10 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            28.23 |      23.58 |       24.93 |     40.75 |      1080 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     42.11 |            297 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       505 |
| None                                       |       417 |
| obfs3, obfs4                               |        69 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| obfs2, obfs3, obfs4                        |         6 |
| obfs3                                      |         6 |
| meek                                       |         5 |
| obfs3, obfs4, scramblesuit                 |         5 |
| fte, meek, obfs3, obfs4                    |         2 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek, meek                                 |         1 |
| obfs2, obfs3                               |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs3, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

