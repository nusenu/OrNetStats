---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-11-15 08:00 UTC**

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
| [tormazter@sentries.org z is s](endtoend-correlation-groups#tormaztersentriesorg-z-is-s)                                             | 0.07        | 0.1        | 3         | 3               | 2017-11-06     | 2                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                             | 0.05        | 0.04       | 4         | 4               | 2017-10-01     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv) | 0.04        | 0.21       | 3         | 3               | 2017-08-28     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                       | 0.02        | 0.45       | 5         | 2               | 2017-06-23     | 1                           |
| **Total**                                                                                                                            | **0.18**    | **0.80**   | **15**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                            |   Exit(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |      6.91 |        21 | 2016-01-25   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      4.16 |         4 | 2014-11-21   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |      3.88 |         6 | 2016-12-23   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |      3.51 |         6 | 2014-04-09   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.58 |         1 | 2014-04-19   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)           |      2.52 |         8 | 2013-07-10   |
| [abuse@blockone.cz - 1DGEy5TrULnUns8T2CN97WnD8pTHLD](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)          |      2.51 |         1 | 2017-07-20   |
| [Admin &lt;admin AT xshells DOT net&gt;](https://atlas.torproject.org/#details/E8E71987BCB8C24DBDF1C3BB0BF3B6C76550A108)                      |      2.31 |         1 | 2016-09-14   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C) |      2.26 |         6 | 2014-04-08   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                              |      1.92 |         6 | 2015-08-27   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.96 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |       1.68 |        29 | 2014-12-23   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       1.13 |         7 | 2016-01-03   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       0.9  |        20 | 2015-05-16   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       0.89 |         7 | 2016-08-10   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |       0.74 |         4 | 2016-07-26   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                  |       0.73 |         8 | 2014-04-10   |
| [info omuravpn.com](https://atlas.torproject.org/#search/family:10AE18EA3E1841D8EF2459823E730B1A904E8A00)                                     |       0.63 |        14 | 2017-01-05   |
| [tor terjan net](https://atlas.torproject.org/#search/family:B411027C926A9BFFCF7DA91E3CAF1856A321EFFD)                                        |       0.58 |        10 | 2015-03-05   |
| [poiuty@protonmail.com - 1YWqF3SGnQMkwgfGasrNmYv1XG](https://atlas.torproject.org/#search/family:CFEC9600E877776982C3161B6A98812871F2A07F)    |       0.54 |         2 | 2016-01-26   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.586 |      6.91 |       0.47 |        29 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            1.201 |      0    |       1.96 |         7 | 2014-04-22   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            1.09  |      0    |       0.74 |         8 | 2016-07-26   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            1.058 |      0    |       1.68 |        30 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.78  |      0    |       0.49 |         3 | 2015-04-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.78  |      4.16 |       0    |         4 | 2014-11-21   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |            0.728 |      3.88 |       0    |         6 | 2016-12-23   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |            0.694 |      0    |       1.13 |         7 | 2016-01-03   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            0.659 |      3.51 |       0    |         6 | 2014-04-09   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                  |            0.63  |      0    |       0.73 |        10 | 2014-04-10   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            24.49 |      26.29 |     23.16 |       935 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            22.72 |      25.84 |      6.1  |      1312 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            10.78 |       9.94 |     13.53 |       481 |
| [United States](https://atlas.torproject.org/#search/country:us)  |             9.2  |       7.84 |     13.44 |      1088 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             3.86 |       3.71 |      5    |       257 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.77 |       2.62 |      6.93 |       194 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.94 |       3.18 |      3.03 |       141 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             2.73 |       2.81 |      2.96 |       239 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.45 |       1.63 |      4.48 |        98 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             1.92 |       1.99 |      1.01 |       286 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                |            16.41 |      18.13 |     12.7  |       588 |
| Online S.a.s.          |            13.08 |      14.46 |     13.32 |       429 |
| Hetzner Online GmbH    |             9.52 |      10.84 |      1.16 |       338 |
| Digital Ocean, Inc.    |             5.08 |       6.13 |      1.58 |       364 |
| Host Europe GmbH       |             3.1  |       3.79 |      0    |        51 |
| myLoc managed IT AG    |             1.68 |       2.31 |      0.41 |        41 |
| SURFnet bv             |             1.39 |       1    |      1.05 |        11 |
| Contabo GmbH           |             1.06 |       1.44 |      0.48 |        47 |
| ITL Company            |             1.01 |       1.44 |      0.04 |        51 |
| Init7 Switzerland Ltd. |             0.89 |       1.43 |      0    |        20 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             46.2 |     45.69 |      45.91 |      2445 |
| 0.3.0         |             18.3 |     21.05 |      18.96 |       905 |
| 0.2.9         |             15   |      9.64 |      15.46 |      1286 |
| 0.2.5         |              6.8 |      5.86 |       7.2  |       730 |
| 0.3.2         |              6.5 |     12.36 |       5.72 |       206 |
| 0.2.7         |              3.1 |      2.77 |       2.93 |       381 |
| 0.2.4         |              1.5 |      0.07 |       1.79 |       344 |
| 0.2.8         |              1.5 |      0.93 |       1.34 |       114 |
| 0.2.6         |              0.4 |      0.11 |       0.49 |        59 |
| 0.3.3         |              0.3 |      1.45 |       0.14 |        14 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.15 |       5.22 |      2.97 |       784 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.4 |      89.8 |       92.2 |      6000 |
| BSD     |              7.1 |      10.1 |        7.3 |       328 |
| Windows |              0.1 |       0   |        0   |       136 |
| Darwin  |              0.1 |       0   |        0   |        10 |
| SunOS   |              0.1 |       0   |        0.1 |         3 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            19.66 |      18.72 |       16.95 |     27.58 |       585 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     29.76 |            124 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1227 |
| None                                       |       656 |
| obfs3, obfs4                               |        62 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        18 |
| obfs2, obfs3, obfs4                        |        10 |
| obfs3, obfs4, scramblesuit                 |         9 |
| obfs3, scramblesuit                        |         8 |
| obfs2, obfs3                               |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         5 |
| fte, obfs3, obfs4                          |         4 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

