---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-11-01 08:00 UTC**

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
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb) | 0.08        | 0.58       | 13        | 2               | 2016-04-01     | 4                           |
| [emerson tor@emersonveenstra.net bitcoin:126gyYcBji](endtoend-correlation-groups#emerson-toremersonveenstranet-bitcoin126gyycbji)        | 0.06        | 0.37       | 4         | 4               | 2017-10-04     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)     | 0.06        | 0.2        | 3         | 3               | 2017-08-23     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                                 | 0.05        | 0.04       | 4         | 4               | 2017-10-01     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.03        | 0.42       | 2         | 2               | 2017-02-16     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                           | 0.03        | 0.63       | 5         | 2               | 2017-06-23     | 1                           |
| **Total**                                                                                                                                | **0.31**    | **2.24**   | **31**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      7.47 |        21 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      5.32 |         6 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      3.54 |         4 | 2014-11-21   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      3.36 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:E34E25D958D46DDE5092385B14117C9B301DC0E9)     |      2.1  |        10 | 2014-05-19   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.05 |         3 | 2014-11-04   |
| [tor-relay-admin robgjansen com https://onionpop.](https://atlas.torproject.org/#search/family:4B1E3276137AD12DCCEBE354EA11C1E47F804F67)         |      1.97 |         3 | 2015-12-11   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                    |      1.91 |         6 | 2016-04-02   |
| [abuse@blockone.cz - 1DGEy5TrULnUns8T2CN97WnD8pTHLD](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)             |      1.89 |         1 | 2017-07-20   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)       |      1.81 |         6 | 2016-12-23   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.82 |         7 | 2014-04-22   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |       1.75 |         8 | 2016-07-26   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |       1.27 |        26 | 2014-12-23   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       1.05 |         7 | 2016-01-03   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                  |       1.04 |        10 | 2014-04-10   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       1.02 |         7 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       0.93 |        20 | 2015-05-16   |
| [info AT omuravpn.com](https://atlas.torproject.org/#search/family:10AE18EA3E1841D8EF2459823E730B1A904E8A00)                                  |       0.77 |        13 | 2017-01-05   |
| [A1F4E8E2](https://atlas.torproject.org/#search/family:A1F4E8E278B647E3B0BA91801DDA4F8C4CB009CF)                                              |       0.56 |         2 | 2016-04-25   |
| [11882BD0](https://atlas.torproject.org/#search/family:11882BD0A5A587FEE13465244EA8BCD4C7E03510)                                              |       0.54 |         4 | 2016-07-26   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.751 |      7.47 |       0.49 |        29 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            1.128 |      0    |       1.82 |         7 | 2014-04-22   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            1.085 |      0    |       1.75 |         8 | 2016-07-26   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            1.031 |      5.32 |       0    |         6 | 2014-04-09   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.907 |      0    |       1.27 |        30 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.844 |      0    |       0.44 |         3 | 2015-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.698 |      0.34 |       1.02 |         8 | 2016-08-10   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.686 |      3.54 |       0    |         4 | 2014-11-21   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.651 |      3.36 |       0    |         1 | 2014-04-19   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |            0.65  |      0    |       1.05 |         7 | 2016-01-03   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            23.11 |      26.31 |     19.65 |       893 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            20.67 |      24.44 |      7.14 |      1321 |
| [United States](https://atlas.torproject.org/#search/country:us)  |            11.54 |       9.68 |     13.8  |      1086 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            10.3  |       9.17 |     13.4  |       499 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             5.13 |       4.94 |      5.69 |       262 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.33 |       2.89 |      4.42 |       187 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             3.05 |       2.54 |      4.44 |       155 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             2.89 |       2.59 |      2.79 |       251 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.62 |       1.47 |      5.46 |        95 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             1.92 |       1.8  |      1.13 |       295 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            17.61 |      19.76 |     12.82 |       583 |
| Online S.a.s.       |            12.11 |      14.15 |     11.75 |       417 |
| Hetzner Online GmbH |             7.12 |       8.89 |      1.49 |       322 |
| Digital Ocean, Inc. |             5.53 |       5.88 |      1.61 |       366 |
| Host Europe GmbH    |             3.03 |       4.52 |      0    |        52 |
| myLoc managed IT AG |             1.92 |       2.28 |      0.33 |        45 |
| SURFnet bv          |             1.49 |       1.1  |      1.25 |        11 |
| Contabo GmbH        |             1.14 |       1.54 |      0.33 |        46 |
| Linode, LLC         |             0.98 |       0.28 |      1.13 |       203 |
| ITL Company         |             0.86 |       1.19 |      0.05 |        48 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             40   |     44.1  |      39.68 |      2178 |
| 0.3.0         |             23.8 |     21.35 |      25.8  |      1095 |
| 0.2.9         |             15.3 |      9.4  |      15.99 |      1317 |
| 0.2.5         |              7.3 |      9.04 |       6.53 |       769 |
| 0.3.2         |              5.5 |     11.67 |       4.1  |       177 |
| 0.2.7         |              3.3 |      0.48 |       3.5  |       418 |
| 0.2.8         |              1.7 |      1.04 |       1.95 |       123 |
| 0.2.4         |              1.6 |      0.1  |       1.73 |       361 |
| 0.2.6         |              0.6 |      0.69 |       0.69 |        67 |
| 0.3.3         |              0.4 |      2.08 |       0    |        11 |
| 00da5         |              0   |      0    |       0    |         1 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.61 |       5.92 |      1.28 |       847 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.6 |      88   |       93.3 |      6043 |
| BSD     |              6.9 |      11.8 |        6.4 |       314 |
| Windows |              0.1 |       0   |        0   |       141 |
| Darwin  |              0.1 |       0   |        0   |         9 |
| SunOS   |              0.1 |       0   |        0.2 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.13 |      17.12 |       14.96 |     26.86 |       599 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     31.17 |            136 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1270 |
| None                                       |       655 |
| obfs3, obfs4                               |        64 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs3                                      |        18 |
| obfs3, scramblesuit                        |         9 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, obfs4, scramblesuit                 |         8 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| obfs2, obfs3                               |         6 |
| meek                                       |         5 |
| fte, obfs3, obfs4                          |         3 |
| obfs2, obfs3, obfs4, scramblesuit          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

