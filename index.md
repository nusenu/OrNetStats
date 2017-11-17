---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-11-17 09:00 UTC**

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
| [tormazter@sentries.org z is s](endtoend-correlation-groups#tormaztersentriesorg-z-is-s)                                             | 0.41        | 0.23       | 5         | 5               | 2017-11-07     | 2                           |
| [&lt;none&gt;](endtoend-correlation-groups#none)                                                                                     | 0.04        | 0.01       | 2         | 2               | 2017-11-02     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                             | 0.04        | 0.05       | 4         | 4               | 2017-10-01     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv) | 0.03        | 0.23       | 3         | 3               | 2017-08-28     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                       | 0.02        | 0.35       | 5         | 2               | 2017-06-23     | 1                           |
| **Total**                                                                                                                            | **0.54**    | **0.87**   | **19**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      7.71 |        21 | 2016-01-25   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)       |      4.26 |         6 | 2016-12-23   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      4.2  |         4 | 2014-11-21   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      3.66 |         6 | 2014-04-09   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      3.26 |         1 | 2014-04-19   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.63 |         3 | 2014-11-04   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.48 |         8 | 2013-07-10   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      2.25 |         6 | 2014-04-08   |
| [abuse@blockone.cz - 1DGEy5TrULnUns8T2CN97WnD8pTHLD](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)             |      2.21 |         1 | 2017-07-20   |
| [Admin &lt;admin AT xshells DOT net&gt;](https://atlas.torproject.org/#details/E8E71987BCB8C24DBDF1C3BB0BF3B6C76550A108)                         |      2.07 |         1 | 2016-09-14   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.65 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |       1.35 |        27 | 2014-12-31   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.05 |         3 | 2015-04-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       1.01 |         7 | 2016-01-03   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                  |       0.97 |        10 | 2014-04-10   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       0.87 |         7 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       0.81 |        20 | 2015-05-16   |
| [info omuravpn.com](https://atlas.torproject.org/#search/family:10AE18EA3E1841D8EF2459823E730B1A904E8A00)                                     |       0.76 |        14 | 2017-01-05   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |       0.66 |         4 | 2016-07-26   |
| [poiuty@protonmail.com - 1YWqF3SGnQMkwgfGasrNmYv1XG](https://atlas.torproject.org/#search/family:CFEC9600E877776982C3161B6A98812871F2A07F)    |       0.61 |         2 | 2016-01-26   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.754 |      7.71 |       0.48 |        29 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            1.028 |      0    |       1.65 |         7 | 2014-04-22   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            0.998 |      0    |       0.66 |         8 | 2016-07-26   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.87  |      0    |       1.35 |        28 | 2014-12-31   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |            0.803 |      4.26 |       0    |         6 | 2016-12-23   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.791 |      4.2  |       0    |         4 | 2014-11-21   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            0.689 |      3.66 |       0    |         6 | 2014-04-09   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.651 |      0    |       1.05 |         3 | 2015-04-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |            0.63  |      0    |       1.01 |         7 | 2016-01-03   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.615 |      3.26 |       0    |         1 | 2014-04-19   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            24.13 |      26.06 |     23.16 |       924 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            22.45 |      25.56 |      6.39 |      1325 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            10.49 |      10.19 |     13.05 |       475 |
| [United States](https://atlas.torproject.org/#search/country:us)  |             9.41 |       8.02 |     13.22 |      1116 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             4.18 |       4.02 |      5.3  |       260 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.97 |       2.81 |      7.4  |       205 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.93 |       3.09 |      3.08 |       141 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             2.69 |       2.45 |      3.34 |       242 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.55 |       1.87 |      4.74 |        93 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             2    |       2.08 |      0.94 |       279 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            17.27 |      19.43 |     12.71 |       583 |
| Online S.a.s.       |            12.59 |      13.6  |     13.26 |       421 |
| Hetzner Online GmbH |             9.46 |      11.06 |      1.04 |       336 |
| Digital Ocean, Inc. |             5.06 |       5.82 |      1.7  |       376 |
| Host Europe GmbH    |             2.98 |       3.55 |      0    |        52 |
| myLoc managed IT AG |             1.58 |       2.21 |      0.28 |        42 |
| SURFnet bv          |             1.41 |       1.63 |      1.42 |        11 |
| Contabo GmbH        |             1.06 |       1.42 |      0.55 |        46 |
| THC Projects SRL    |             1    |       0.82 |      0    |        18 |
| ITL Company         |             0.88 |       1.21 |      0.04 |        50 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             46.7 |     46.37 |      46.8  |      2492 |
| 0.3.0         |             17.7 |     21.52 |      18.77 |       872 |
| 0.2.9         |             15.4 |     10.32 |      15.67 |      1319 |
| 0.2.5         |              6.6 |      4.16 |       7.26 |       735 |
| 0.3.2         |              6   |     11.6  |       5.01 |       207 |
| 0.2.7         |              3.1 |      2.5  |       2.9  |       375 |
| 0.2.4         |              1.5 |      0.1  |       1.65 |       349 |
| 0.2.8         |              1.4 |      0.6  |       1.3  |       113 |
| 0.3.3         |              0.6 |      2.67 |       0.15 |        15 |
| 0.2.6         |              0.3 |      0.13 |       0.45 |        59 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.14 |       5.01 |      2.73 |       783 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.4 |      89.6 |       92.4 |      6045 |
| BSD     |              7   |      10.3 |        7   |       323 |
| Windows |              0.1 |       0   |        0   |       137 |
| Darwin  |              0.1 |       0   |        0.1 |        11 |
| SunOS   |              0.1 |       0   |        0.2 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            19.51 |      19.26 |       15.37 |     28.95 |       588 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     32.64 |            123 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1229 |
| None                                       |       655 |
| obfs3, obfs4                               |        61 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        19 |
| obfs2, obfs3, obfs4                        |        10 |
| obfs3, obfs4, scramblesuit                 |        10 |
| obfs3, scramblesuit                        |         9 |
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

