---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-10-06 20:00 UTC**

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
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain) | 0.08        | 0.16       | 5         | 5               | 2018-09-25     | 1                           |
| [wgetdataatprotonmailch tor-relay.co](endtoend-correlation-groups#wgetdataatprotonmailch-tor-relayco)     | 0.04        | 0.08       | 3         | 2               | 2018-10-02     | 1                           |
| [0xFFFFFFFF anon &lt;tyb AT riseup.net&gt;](endtoend-correlation-groups#0xffffffff-anon-tyb-at-riseupnet) | 0.02        | 0.01       | 2         | 2               | 2018-09-29     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)      | 0.02        | 0.15       | 3         | 2               | 2016-08-28     | 1                           |
| [atlayo@atlayo.com](endtoend-correlation-groups#atlayoatlayocom)                                          | 0.01        | 0.15       | 3         | 3               | 2018-09-12     | 1                           |
| **Total**                                                                                                 | **0.17**    | **0.55**   | **16**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |      9.25 |        26 | 2016-01-25   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      3.61 |        13 | 2015-05-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)   |      3.05 |         7 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      2.72 |         4 | 2014-11-21   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.45 |         1 | 2014-04-19   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |      2.12 |         7 | 2016-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |      2    |        36 | 2016-08-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:B27CF1DCEECD50F7992B07D720D7F6BF0EDF9D40)     |      1.85 |         2 | 2018-04-05   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      1.84 |        11 | 2017-12-05   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06) |      1.64 |         6 | 2014-04-08   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |       1.95 |        18 | 2017-06-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |       1.66 |         7 | 2014-04-22   |
| [jwbecher@drazisil.com](https://metrics.torproject.org/rs.html#search/family:46FBC671FD6FCE6B298B2BAE3C7AC7D7DDF1365F)                                 |       0.86 |         6 | 2018-05-08   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                  |       0.83 |         3 | 2018-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.82 |         3 | 2015-04-22   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |       0.8  |         8 | 2015-01-29   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.77 |         5 | 2017-10-24   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       0.74 |        17 | 2015-05-16   |
| [Somebody &lt;mail@typhoon31.de&gt;](https://metrics.torproject.org/rs.html#search/family:74C80B0D670BEC33092413C398ADBB73D00476A9)                    |       0.67 |         3 | 2018-02-05   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.67 |         6 | 2016-01-03   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.251 |      9.25 |       0    |        26 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.646 |      1.85 |       1.95 |        20 | 2017-06-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            1.015 |      0    |       1.66 |         7 | 2014-04-22   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.89  |      3.61 |       0.01 |        14 | 2013-08-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)   |            0.743 |      3.05 |       0    |         7 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.663 |      2.72 |       0    |         4 | 2014-11-21   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.597 |      2.45 |       0    |         1 | 2014-04-19   |
| [jwbecher@drazisil.com](https://metrics.torproject.org/rs.html#search/family:46FBC671FD6FCE6B298B2BAE3C7AC7D7DDF1365F)                                 |            0.529 |      0    |       0.86 |         6 | 2018-05-08   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |            0.516 |      2.12 |       0    |         7 | 2016-12-23   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                  |            0.508 |      0    |       0.83 |         3 | 2018-04-22   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| Online S.a.s.                                                    |            14.07 |      18.82 |      7.2  |       343 |
| OVH SAS                                                          |            13.76 |      16.15 |     12.13 |       552 |
| Hetzner Online GmbH                                              |             8.92 |       8.17 |      0.38 |       361 |
| Joshua Peter McQuistan                                           |             2.7  |       0.57 |      9.6  |        31 |
| myLoc managed IT AG                                              |             2.46 |       2.54 |      2.57 |        44 |
| SURFnet bv                                                       |             1.71 |       1.54 |      3.11 |        24 |
| netcup GmbH                                                      |             1.56 |       2.17 |      0.23 |        49 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             1.48 |       1.7  |      1.85 |        18 |
| Host Europe GmbH                                                 |             1.46 |       2.29 |      0    |        36 |
| FranTech Solutions                                               |             1.38 |       0.81 |      3.4  |        43 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.4         |             39   |     41.65 |      40.49 |      1991 |
| 0.3.3         |             27.2 |     39.63 |      23.38 |      1673 |
| 0.2.9         |             15.7 |      7.75 |      16.99 |      1347 |
| 0.3.2         |             10   |      4.62 |      12.53 |       568 |
| 0.3.1         |              2.4 |      3.48 |       1.88 |       162 |
| 0.3.5         |              2.4 |      1.82 |       2.62 |        81 |
| 0.2.5         |              1.1 |      0.74 |       0.81 |       216 |
| 0.2.4         |              0.9 |      0.23 |       0.47 |       180 |
| 0.2.7         |              0.5 |      0.03 |       0.44 |       143 |
| 0.3.0         |              0.1 |      0.02 |       0.22 |        71 |
| 0.2.6         |              0   |      0.01 |       0.05 |        29 |
| 0.2.8         |              0   |      0    |       0.09 |        31 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.06 |       2.11 |      1.06 |       670 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.3 |      85.9 |       90.9 |      5901 |
| BSD     |              9.3 |      13.5 |        8.8 |       413 |
| Windows |              0.2 |       0.4 |        0   |        98 |
| SunOS   |              0   |       0   |        0.1 |         5 |
| Darwin  |              0   |       0   |        0   |         9 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|             25.7 |      23.28 |       23.99 |     32.15 |       893 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     34.09 |            209 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       416 |
| None                                       |       319 |
| obfs3, obfs4                               |        50 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3                                      |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         3 |
| fte, obfs3, obfs4                          |         2 |
| obfs2, obfs3                               |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| meek                                       |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

