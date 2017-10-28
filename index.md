---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-10-28 06:00 UTC**

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

| Contact                                                                                                                              | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-------------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [emerson tor@emersonveenstra.net bitcoin:126gyYcBji](endtoend-correlation-groups#emerson-toremersonveenstranet-bitcoin126gyycbji)    | 0.06        | 0.44       | 5         | 5               | 2017-10-04     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv) | 0.04        | 0.29       | 3         | 3               | 2017-08-23     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                             | 0.03        | 0.05       | 4         | 4               | 2017-10-01     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                       | 0.03        | 0.09       | 2         | 2               | 2016-03-07     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                         | 0.02        | 0.49       | 2         | 2               | 2017-02-16     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                       | 0.02        | 0.51       | 5         | 2               | 2017-06-23     | 1                           |
| **Total**                                                                                                                            | **0.20**    | **1.87**   | **21**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                               |   Exit(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      6.6  |        21 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      5.24 |         6 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      3.84 |         4 | 2014-11-21   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9)    |      3.17 |        50 | 2016-08-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.58 |         1 | 2014-04-19   |
| [abuse@blockone.cz - 1DGEy5TrULnUns8T2CN97WnD8pTHLD](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)             |      2.49 |         1 | 2017-07-20   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)       |      2.2  |         6 | 2016-12-23   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.09 |         3 | 2014-11-04   |
| [Tor Manager &lt;tor@ibiblio.org&gt;](https://atlas.torproject.org/#search/family:C59E079437340E3AD14E6785C0A91A5B6F328566)                      |      2.03 |         2 | 2014-04-08   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                    |      1.98 |         6 | 2016-04-02   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |       1.65 |         8 | 2016-07-26   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.45 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |       1.25 |        26 | 2014-12-23   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                  |       1    |        10 | 2014-04-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       0.93 |        20 | 2015-05-16   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       0.91 |         7 | 2016-08-10   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       0.8  |         7 | 2016-01-03   |
| [info AT omuravpn.com](https://atlas.torproject.org/#search/family:10AE18EA3E1841D8EF2459823E730B1A904E8A00)                                  |       0.64 |        13 | 2017-01-05   |
| [Tor Relay Admin &lt;tor-admin AT meurisse DOT fr&gt;](https://atlas.torproject.org/#details/C818C0EA0BAD90F5432DBA4EE662BCBEC39D2668)        |       0.58 |         1 | 2016-10-12   |
| [poiuty@protonmail.com - 1YWqF3SGnQMkwgfGasrNmYv1XG](https://atlas.torproject.org/#search/family:CFEC9600E877776982C3161B6A98812871F2A07F)    |       0.57 |         2 | 2016-01-26   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.551 |      6.6  |       0.46 |        29 | 2016-01-25   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            1.063 |      0    |       1.65 |         8 | 2016-07-26   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            0.994 |      5.24 |       0    |         6 | 2014-04-09   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.937 |      0    |       1.25 |        30 | 2014-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.932 |      0    |       1.45 |         7 | 2014-04-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.729 |      3.84 |       0    |         4 | 2014-11-21   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                  |            0.649 |      0    |       1    |        10 | 2014-04-10   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.645 |      0.31 |       0.91 |         8 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.612 |      0    |       0.93 |        22 | 2015-05-16   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9) |            0.601 |      3.17 |       0    |        50 | 2016-08-22   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            23.25 |      26.37 |     19.2  |       860 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            20.96 |      24.81 |      7.49 |      1297 |
| [United States](https://atlas.torproject.org/#search/country:us)  |            12.92 |      11.03 |     16.71 |      1127 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |             9.38 |       8.06 |     13.13 |       499 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             4.77 |       4.6  |      5.33 |       266 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.05 |       2.68 |      3.9  |       184 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             2.79 |       2.4  |      3.61 |       251 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.56 |       2.31 |      4.03 |       150 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.49 |       1.47 |      5.05 |        98 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             1.84 |       1.76 |      0.73 |       276 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            16.92 |      19.21 |     11.58 |       572 |
| Online S.a.s.       |            12.11 |      14.22 |     11.3  |       404 |
| Hetzner Online GmbH |             8.03 |      10.22 |      1.84 |       316 |
| Digital Ocean, Inc. |             5.61 |       5.75 |      2.52 |       395 |
| Host Europe GmbH    |             2.67 |       3.9  |      0    |        52 |
| myLoc managed IT AG |             1.6  |       1.69 |      0.23 |        43 |
| Contabo GmbH        |             1.07 |       1.48 |      0.26 |        46 |
| SURFnet bv          |             0.95 |       0.42 |      0.59 |        11 |
| ITL Company         |             0.93 |       1.17 |      0.05 |        50 |
| Linode, LLC         |             0.91 |       0.43 |      0.24 |       190 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             37.5 |     43.22 |      36.3  |      2100 |
| 0.3.0         |             25.8 |     22.07 |      29.26 |      1156 |
| 0.2.9         |             15.8 |      8.92 |      16.27 |      1311 |
| 0.2.5         |              7.1 |      9.19 |       6.33 |       767 |
| 0.3.2         |              5.4 |     11.31 |       3.93 |       166 |
| 0.2.7         |              3.4 |      0.43 |       3.42 |       424 |
| 0.2.4         |              1.9 |      1.08 |       1.78 |       354 |
| 0.2.8         |              1.6 |      0.82 |       1.87 |       126 |
| 0.2.6         |              0.6 |      0.64 |       0.7  |        62 |
| 0.3.3         |              0.4 |      2.14 |       0    |        12 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             6.04 |       5.92 |      2.16 |       840 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93.1 |      89.7 |       93.5 |      6009 |
| BSD     |              6.5 |      10   |        6.1 |       319 |
| Windows |              0.1 |       0   |        0   |       136 |
| SunOS   |              0   |       0   |        0   |         4 |
| Darwin  |              0   |       0   |        0   |         8 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            17.85 |       17.6 |       14.59 |     25.35 |       572 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     28.26 |            119 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1288 |
| None                                       |       642 |
| obfs3, obfs4, scramblesuit                 |       247 |
| obfs3, obfs4                               |        62 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs3                                      |        19 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| obfs2, obfs3                               |         6 |
| meek                                       |         5 |
| fte, obfs3, obfs4                          |         3 |
| obfs2, obfs3, obfs4, scramblesuit          |         3 |
| obfs4, scramblesuit                        |         2 |
| scramblesuit                               |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

