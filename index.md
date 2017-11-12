---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-11-12 09:00 UTC**

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
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                             | 0.06        | 0.04       | 4         | 4               | 2017-10-01     | 1                           |
| [&lt;none&gt;](endtoend-correlation-groups#none)                                                                                     | 0.04        | 0.01       | 2         | 2               | 2017-11-02     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                         | 0.04        | 0.32       | 2         | 2               | 2017-02-16     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                       | 0.04        | 0.45       | 5         | 2               | 2017-06-23     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv) | 0.03        | 0.18       | 3         | 3               | 2017-08-23     | 1                           |
| **Total**                                                                                                                            | **0.21**    | **1.00**   | **16**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      6.84 |        21 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      4.29 |         6 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      4.13 |         4 | 2014-11-21   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)       |      3.33 |         6 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.65 |         1 | 2014-04-19   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.36 |         8 | 2013-07-10   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.16 |         3 | 2014-11-04   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      2.08 |         6 | 2014-04-08   |
| [abuse@blockone.cz - 1DGEy5TrULnUns8T2CN97WnD8pTHLD](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)             |      2.05 |         1 | 2017-07-20   |
| [Admin &lt;admin AT xshells DOT net&gt;](https://atlas.torproject.org/#details/E8E71987BCB8C24DBDF1C3BB0BF3B6C76550A108)                         |      2.03 |         1 | 2016-09-14   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       1.76 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                    |       1.65 |        29 | 2014-12-23   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       1.1  |         7 | 2016-01-03   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                     |       1.04 |        10 | 2014-04-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       1.02 |        20 | 2015-05-16   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                                 |       0.91 |         4 | 2016-07-26   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)            |       0.9  |         7 | 2016-08-10   |
| [info omuravpn.com](https://atlas.torproject.org/#search/family:10AE18EA3E1841D8EF2459823E730B1A904E8A00)                                        |       0.76 |        13 | 2017-01-05   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://atlas.torproject.org/#search/family:F596E1B1EF98E1DDBBDC934DB722AF54069868F6) |       0.54 |        10 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:5DEF791E0025EA398CB26F4A10DC11394EB6FAAB)                            |       0.5  |         7 | 2016-08-24   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.661 |      6.84 |       0.5  |        29 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            1.093 |      0    |       1.76 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            1.057 |      0    |       1.65 |        30 | 2014-12-23   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            0.811 |      4.29 |       0    |         6 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.781 |      4.13 |       0    |         4 | 2014-11-21   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |            0.686 |      0    |       1.1  |         7 | 2016-01-03   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                  |            0.646 |      0    |       1.04 |        10 | 2014-04-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.644 |      0    |       1.02 |        22 | 2015-05-16   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |            0.63  |      3.33 |       0    |         6 | 2016-12-23   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.612 |      0.26 |       0.9  |         8 | 2016-08-10   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            24.23 |      26.05 |     23.1  |       918 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            22.35 |      26.75 |      6.49 |      1315 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            10.32 |       9.89 |     12.63 |       488 |
| [United States](https://atlas.torproject.org/#search/country:us)  |             9.25 |       7.61 |     12.78 |      1105 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             3.95 |       3.17 |      4.77 |       240 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.72 |       3.15 |      5.71 |       190 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             2.91 |       2.78 |      3.24 |       242 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.85 |       3.05 |      2.9  |       145 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.52 |       1.69 |      4.61 |       101 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             1.92 |       1.88 |      1    |       292 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            17.05 |      18.09 |     13.17 |       584 |
| Online S.a.s.       |            12.5  |      14    |     12.99 |       415 |
| Hetzner Online GmbH |             9.61 |      11.76 |      1.14 |       336 |
| Digital Ocean, Inc. |             5.42 |       6.24 |      1.95 |       383 |
| Host Europe GmbH    |             2.6  |       3.93 |      0    |        49 |
| myLoc managed IT AG |             1.63 |       2.17 |      0.29 |        43 |
| Contabo GmbH        |             1.09 |       1.36 |      0.57 |        48 |
| SURFnet bv          |             1.08 |       0.9  |      0.87 |        10 |
| ITL Company         |             1.02 |       1.44 |      0.04 |        50 |
| ISPpro Internet KG  |             0.92 |       1.45 |      0    |        34 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             45.6 |     44.72 |      45.3  |      2412 |
| 0.3.0         |             18.4 |     20.02 |      19.78 |       913 |
| 0.2.9         |             15.3 |     10.27 |      15.74 |      1318 |
| 0.2.5         |              6.9 |      6.75 |       6.95 |       744 |
| 0.3.2         |              6.3 |     11.34 |       5.73 |       199 |
| 0.2.7         |              3   |      2.68 |       2.9  |       392 |
| 0.2.4         |              1.7 |      0.93 |       1.71 |       366 |
| 0.2.8         |              1.4 |      0.95 |       1.28 |       123 |
| 0.3.3         |              0.5 |      2.19 |       0.06 |        11 |
| 0.2.6         |              0.4 |      0.1  |       0.51 |        63 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|              5.2 |       5.13 |      3.73 |       821 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.5 |      90.8 |       92.4 |      6050 |
| BSD     |              7   |       9.1 |        7.1 |       321 |
| SunOS   |              0.1 |       0   |        0.2 |         4 |
| Windows |              0.1 |       0   |        0   |       149 |
| Darwin  |              0   |       0   |        0   |        10 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            19.66 |      18.58 |        17.2 |     27.24 |       588 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     30.05 |            123 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1234 |
| None                                       |       654 |
| obfs3, obfs4                               |        61 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        19 |
| obfs2, obfs3, obfs4                        |        10 |
| obfs3, scramblesuit                        |         9 |
| obfs2, obfs3                               |         7 |
| obfs3, obfs4, scramblesuit                 |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         5 |
| fte, obfs3, obfs4                          |         3 |
| obfs2, obfs3, obfs4, scramblesuit          |         3 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

