---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-11-02 14:00 UTC**

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
| [emerson tor@emersonveenstra.net bitcoin:126gyYcBji](endtoend-correlation-groups#emerson-toremersonveenstranet-bitcoin126gyycbji)    | 0.07        | 0.3        | 4         | 4               | 2017-10-04     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv) | 0.05        | 0.18       | 3         | 3               | 2017-08-23     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                             | 0.04        | 0.04       | 4         | 4               | 2017-10-01     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                       | 0.02        | 0.56       | 5         | 2               | 2017-06-23     | 1                           |
| **Total**                                                                                                                            | **0.18**    | **1.08**   | **16**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |      6.87 |        21 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |      5.45 |         6 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      3.76 |         4 | 2014-11-21   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |      2.78 |         6 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.67 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:E34E25D958D46DDE5092385B14117C9B301DC0E9)  |      2.02 |        10 | 2014-05-19   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C) |      1.97 |         6 | 2014-04-08   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)           |      1.91 |         8 | 2013-07-10   |
| [abuse@blockone.cz - 1DGEy5TrULnUns8T2CN97WnD8pTHLD](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)          |      1.74 |         1 | 2017-07-20   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                              |      1.63 |         6 | 2015-08-27   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                                 |       1.82 |         8 | 2016-07-26   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       1.8  |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                    |       1.27 |        27 | 2014-12-23   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       1.06 |        21 | 2015-05-16   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       1.03 |         7 | 2016-01-03   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)            |       0.83 |         6 | 2016-08-10   |
| [info AT omuravpn.com](https://atlas.torproject.org/#search/family:10AE18EA3E1841D8EF2459823E730B1A904E8A00)                                     |       0.72 |        13 | 2017-01-05   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://atlas.torproject.org/#search/family:F596E1B1EF98E1DDBBDC934DB722AF54069868F6) |       0.63 |        11 | 2014-04-09   |
| [11882BD0](https://atlas.torproject.org/#search/family:11882BD0A5A587FEE13465244EA8BCD4C7E03510)                                                 |       0.6  |         4 | 2016-07-26   |
| [tor terjan net](https://atlas.torproject.org/#search/family:B411027C926A9BFFCF7DA91E3CAF1856A321EFFD)                                           |       0.55 |        10 | 2015-03-05   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.584 |      6.87 |       0.43 |        29 | 2016-01-25   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            1.145 |      0    |       1.82 |         8 | 2016-07-26   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            1.133 |      0    |       1.8  |         7 | 2014-04-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            1.039 |      5.45 |       0    |         6 | 2014-04-09   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.942 |      0    |       1.27 |        30 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.815 |      0    |       0.4  |         3 | 2015-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.752 |      0.33 |       0.83 |         8 | 2016-08-10   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.718 |      3.76 |       0    |         4 | 2014-11-21   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.668 |      0    |       1.06 |        22 | 2015-05-16   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |            0.65  |      0    |       1.03 |         7 | 2016-01-03   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            24.29 |      26.9  |     20.8  |       919 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            21.41 |      25.41 |      7.59 |      1327 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            10.23 |       8.98 |     12.57 |       505 |
| [United States](https://atlas.torproject.org/#search/country:us)  |            10.03 |       8.86 |     11.7  |      1091 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             4.34 |       4.16 |      4.95 |       261 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.14 |       2.5  |      5.32 |       190 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             3.14 |       2.59 |      4.66 |       156 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             2.99 |       2.58 |      3.77 |       253 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.63 |       1.48 |      5.38 |        96 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             2    |       1.84 |      1.02 |       299 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            17.75 |      20.33 |     12.45 |       574 |
| Online S.a.s.       |            12.34 |      13.87 |     11.85 |       426 |
| Hetzner Online GmbH |             7.44 |       9.17 |      1.52 |       321 |
| Digital Ocean, Inc. |             5.33 |       6.03 |      1.57 |       377 |
| Host Europe GmbH    |             3.02 |       4.37 |      0    |        52 |
| myLoc managed IT AG |             1.78 |       2.35 |      0.27 |        45 |
| SURFnet bv          |             1.45 |       1    |      1.36 |        11 |
| Contabo GmbH        |             1.12 |       1.5  |      0.29 |        47 |
| ITL Company         |             0.89 |       1.14 |      0.09 |        52 |
| ISPpro Internet KG  |             0.86 |       1.28 |      0    |        34 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             40.8 |     44.21 |      40.13 |      2262 |
| 0.3.0         |             23.3 |     21.1  |      25.37 |      1089 |
| 0.2.9         |             15.6 |     11.04 |      16.4  |      1345 |
| 0.2.5         |              7.1 |      7.4  |       6.6  |       755 |
| 0.3.2         |              5.5 |     11.63 |       3.93 |       182 |
| 0.2.7         |              3.1 |      0.94 |       3.08 |       411 |
| 0.2.4         |              1.7 |      0.69 |       1.8  |       377 |
| 0.2.8         |              1.6 |      0.97 |       1.87 |       127 |
| 0.2.6         |              0.5 |      0.64 |       0.58 |        69 |
| 0.3.3         |              0.3 |      1.5  |       0.08 |        11 |
| c165e         |              0   |      0    |       0    |         1 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.46 |       5.47 |      2.28 |       858 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.5 |      89.1 |       92.9 |      6109 |
| BSD     |              7   |      10.9 |        6.7 |       328 |
| Darwin  |              0.1 |       0   |        0   |         9 |
| Windows |              0.1 |       0   |        0   |       164 |
| SunOS   |              0   |       0   |        0.1 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.42 |      16.83 |       15.75 |     27.47 |       599 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     31.18 |            138 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1272 |
| None                                       |       680 |
| obfs3, obfs4                               |        63 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs3                                      |        18 |
| obfs3, scramblesuit                        |         9 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, obfs4, scramblesuit                 |         7 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| obfs2, obfs3                               |         6 |
| meek                                       |         5 |
| obfs2, obfs3, obfs4, scramblesuit          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, obfs4                          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

