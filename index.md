---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-10-24 22:00 UTC**

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
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv) | 0.05        | 0.42       | 3         | 3               | 2017-08-23     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                             | 0.04        | 0.05       | 4         | 4               | 2017-10-01     | 1                           |
| [emerson tor@emersonveenstra.net bitcoin:126gyYcBji](endtoend-correlation-groups#emerson-toremersonveenstranet-bitcoin126gyycbji)    | 0.04        | 0.47       | 4         | 4               | 2017-10-04     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                       | 0.02        | 0.75       | 5         | 2               | 2017-06-23     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                       | 0.01        | 0.09       | 2         | 2               | 2016-03-07     | 1                           |
| **Total**                                                                                                                            | **0.16**    | **1.78**   | **18**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |      6.2  |        21 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |      5.35 |         5 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      3.54 |         4 | 2014-11-21   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:E34E25D958D46DDE5092385B14117C9B301DC0E9)  |      3.12 |        20 | 2014-05-19   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.75 |         1 | 2014-04-19   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |      2.62 |         6 | 2016-12-23   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:C656B41AEFB40A141967EBF49D6E69603C9B4A11) |      2.5  |         5 | 2014-04-08   |
| [Tor Manager &lt;tor@ibiblio.org&gt;](https://atlas.torproject.org/#search/family:C59E079437340E3AD14E6785C0A91A5B6F328566)                   |      2.16 |         2 | 2014-04-08   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                              |      1.99 |         6 | 2015-08-27   |
| [abuse@blockone.cz - 1DGEy5TrULnUns8T2CN97WnD8pTHLD](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)          |      1.98 |         1 | 2017-07-20   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |       1.57 |         8 | 2016-07-26   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.51 |         3 | 2015-04-22   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.43 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |       1.2  |        26 | 2014-12-23   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       1.07 |         7 | 2016-08-10   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       0.97 |         7 | 2016-01-03   |
| [info AT omuravpn.com](https://atlas.torproject.org/#search/family:10AE18EA3E1841D8EF2459823E730B1A904E8A00)                                  |       0.96 |        14 | 2017-01-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       0.88 |        20 | 2015-05-16   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                  |       0.85 |        10 | 2014-04-10   |
| [poiuty@protonmail.com - 1YWqF3SGnQMkwgfGasrNmYv1XG](https://atlas.torproject.org/#search/family:CFEC9600E877776982C3161B6A98812871F2A07F)    |       0.63 |         2 | 2016-01-26   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.446 |      6.2  |       0.45 |        29 | 2016-01-25   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            1.028 |      0    |       1.57 |         8 | 2016-07-26   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            0.991 |      5.35 |       0    |         5 | 2014-04-09   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.984 |      0    |       1.51 |         3 | 2015-04-22   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.935 |      0    |       1.43 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.87  |      0    |       1.2  |        29 | 2014-12-23   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.796 |      0.5  |       1.07 |         8 | 2016-08-10   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.655 |      3.54 |       0    |         4 | 2014-11-21   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |            0.636 |      0    |       0.97 |         7 | 2016-01-03   |
| [info AT omuravpn.com](https://atlas.torproject.org/#search/family:10AE18EA3E1841D8EF2459823E730B1A904E8A00)                                  |            0.626 |      0    |       0.96 |        14 | 2017-01-05   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            23.01 |      26.1  |     19.91 |       888 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            20.89 |      24.35 |      7.23 |      1289 |
| [United States](https://atlas.torproject.org/#search/country:us)  |            12.57 |      10.67 |     14.93 |      1112 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |             9.32 |       9.76 |     11.17 |       479 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             4.89 |       4.81 |      5.97 |       264 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.15 |       2.73 |      4.84 |       188 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             3.09 |       2.48 |      5.41 |       156 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             2.99 |       2.61 |      3.43 |       258 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.74 |       1.39 |      6.3  |        96 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             1.84 |       1.85 |      0.72 |       292 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            16.62 |      18.23 |     12.56 |       571 |
| Online S.a.s.       |            12.16 |      14.41 |     10.43 |       406 |
| Hetzner Online GmbH |             8.13 |      10.14 |      1.59 |       310 |
| Digital Ocean, Inc. |             5.55 |       6.42 |      1.71 |       355 |
| Host Europe GmbH    |             2.53 |       3.64 |      0    |        47 |
| SURFnet bv          |             1.61 |       2.26 |      0.74 |        11 |
| myLoc managed IT AG |             1.61 |       1.78 |      0.2  |        44 |
| Contabo GmbH        |             1.11 |       1.39 |      0.29 |        46 |
| ITL Company         |             0.97 |       1.16 |      0.07 |        51 |
| ISPpro Internet KG  |             0.92 |       1.39 |      0    |        32 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             36.4 |     42.36 |      36.06 |      2032 |
| 0.3.0         |             26.6 |     21.82 |      29.07 |      1235 |
| 0.2.9         |             16   |     10.05 |      16.34 |      1310 |
| 0.2.5         |              7.1 |      7.44 |       6.55 |       747 |
| 0.3.2         |              5.3 |     11.95 |       3.95 |       163 |
| 0.2.7         |              3.4 |      0.41 |       3.66 |       434 |
| 0.2.4         |              2.4 |      4.16 |       1.72 |       390 |
| 0.2.8         |              1.7 |      1.06 |       1.91 |       130 |
| 0.2.6         |              0.6 |      0.65 |       0.7  |        64 |
| 0.3.3         |              0   |      0.04 |       0    |         7 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             6.54 |       6.09 |      5.23 |       888 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.8 |      89.7 |       93.1 |      6012 |
| BSD     |              6.7 |      10.2 |        6.5 |       315 |
| SunOS   |              0.1 |       0   |        0.1 |         4 |
| Windows |              0.1 |       0   |        0   |       150 |
| Darwin  |              0   |       0   |        0.1 |        10 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.81 |      18.95 |        14.8 |     27.31 |       569 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     30.19 |            114 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1309 |
| None                                       |       642 |
| obfs3, obfs4, scramblesuit                 |       247 |
| obfs3, obfs4                               |        62 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs3                                      |        19 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs3, scramblesuit                        |         9 |
| obfs2, obfs3                               |         7 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
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

