---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-11-25 20:00 UTC**

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
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.15        | 0.02       | 6         | 5               | 2017-11-23     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb) | 0.09        | 0.72       | 13        | 2               | 2016-04-01     | 4                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)     | 0.07        | 0.37       | 3         | 3               | 2017-08-28     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                                 | 0.04        | 0.04       | 4         | 4               | 2017-10-01     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.02        | 0.54       | 2         | 2               | 2017-02-16     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                           | 0.01        | 0.46       | 5         | 2               | 2017-06-23     | 1                           |
| **Total**                                                                                                                                | **0.38**    | **2.15**   | **33**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |      7.02 |        20 | 2016-01-25   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      5.04 |         4 | 2014-11-21   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |      4.73 |         6 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      3.63 |         1 | 2014-04-19   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9) |      3.05 |        50 | 2016-08-22   |
| [Admin &lt;admin AT xshells DOT net&gt;](https://atlas.torproject.org/#details/E8E71987BCB8C24DBDF1C3BB0BF3B6C76550A108)                      |      2.37 |         1 | 2016-09-14   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                 |      2.26 |         6 | 2016-04-02   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C) |      2.17 |         6 | 2014-04-08   |
| [abuse@blockone.cz - 1DGEy5TrULnUns8T2CN97WnD8pTHLD](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)          |      2.14 |         1 | 2017-07-20   |
| [Tor Manager &lt;tor@ibiblio.org&gt;](https://atlas.torproject.org/#search/family:C59E079437340E3AD14E6785C0A91A5B6F328566)                   |      2.14 |         2 | 2014-04-08   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)            |       1.27 |         7 | 2016-08-10   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       1.25 |         7 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                      |       1.18 |         3 | 2015-04-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       1.11 |         7 | 2016-01-03   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       0.98 |        20 | 2015-05-16   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                    |       0.92 |        27 | 2014-12-31   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                                 |       0.84 |         4 | 2016-07-26   |
| [tormazter@sentries.org z is s](https://atlas.torproject.org/#search/family:49F5F13DAA45D6BF6A97DBD5E008DF99F50207DD)                            |       0.67 |         3 | 2017-11-06   |
| [info omuravpn.com](https://atlas.torproject.org/#search/family:94C0F99BA44AA4A6767C71333B8A66DBD1BC08C7)                                        |       0.6  |         6 | 2017-01-05   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://atlas.torproject.org/#search/family:F596E1B1EF98E1DDBBDC934DB722AF54069868F6) |       0.53 |         9 | 2014-04-09   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.507 |      7.02 |       0.35 |        28 | 2016-01-25   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            1.18  |      0    |       0.84 |         8 | 2016-07-26   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.913 |      5.04 |       0    |         4 | 2014-11-21   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.887 |      0.32 |       1.27 |         8 | 2016-08-10   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |            0.857 |      4.73 |       0    |         6 | 2016-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.819 |      0    |       1.25 |         7 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.772 |      0    |       1.18 |         3 | 2015-04-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |            0.727 |      0    |       1.11 |         7 | 2016-01-03   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.658 |      3.63 |       0    |         1 | 2014-04-19   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.649 |      0    |       0.92 |        28 | 2014-12-31   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            24.48 |      26.59 |     24.31 |       926 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            22.54 |      25.23 |      6.97 |      1301 |
| [United States](https://atlas.torproject.org/#search/country:us)  |             9.79 |       8.09 |     15.22 |      1122 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |             9.66 |       9.83 |      9.5  |       458 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             4.19 |       3.78 |      6.42 |       271 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.73 |       1.85 |      7.51 |       191 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             3.1  |       2.39 |      4.01 |       101 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.65 |       2.72 |      2.7  |       143 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             2.35 |       2.28 |      2.45 |       230 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             1.9  |       1.93 |      0.59 |       297 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            17.26 |      19.58 |     14.1  |       579 |
| Online S.a.s.       |            13.06 |      14.47 |     14.4  |       422 |
| Hetzner Online GmbH |             8.85 |      10.57 |      0.88 |       319 |
| Digital Ocean, Inc. |             5    |       6.21 |      1.85 |       329 |
| Host Europe GmbH    |             3.01 |       3.41 |      0    |        48 |
| myLoc managed IT AG |             1.78 |       2.39 |      0.43 |        42 |
| THC Projects SRL    |             1.71 |       1.95 |      0    |        25 |
| SURFnet bv          |             1.47 |       1.74 |      1.28 |        11 |
| Contabo GmbH        |             1.09 |       1.25 |      0.71 |        48 |
| ISPpro Internet KG  |             0.95 |       1.26 |      0    |        35 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             46.8 |     43.52 |      46.74 |      2544 |
| 0.3.0         |             18.2 |     20.11 |      19.03 |       841 |
| 0.2.9         |             14.9 |     10.87 |      15.77 |      1330 |
| 0.3.2         |              6.7 |     15.38 |       4.94 |       255 |
| 0.2.5         |              6.4 |      5.44 |       7.01 |       701 |
| 0.2.7         |              2.9 |      2.58 |       2.57 |       355 |
| 0.2.4         |              1.7 |      0.71 |       1.74 |       354 |
| 0.2.8         |              1.2 |      0.1  |       1.42 |       108 |
| 0.2.6         |              0.4 |      0.15 |       0.49 |        62 |
| 0.3.3         |              0.4 |      1.09 |       0.24 |        11 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.09 |        4.8 |      3.44 |       771 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.3 |      89.4 |       92   |      6070 |
| BSD     |              7.3 |      10.4 |        7.6 |       308 |
| SunOS   |              0.1 |       0   |        0.2 |         4 |
| Windows |              0.1 |       0   |        0   |       159 |
| Darwin  |              0   |       0   |        0   |        10 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            19.65 |      19.12 |       16.71 |     27.48 |       581 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     30.79 |            116 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1226 |
| None                                       |       630 |
| obfs3, obfs4, scramblesuit                 |       195 |
| obfs3, obfs4                               |        62 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        16 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs3, scramblesuit                        |         9 |
| obfs2, obfs3                               |         8 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         5 |
| fte, obfs3, obfs4                          |         3 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| scramblesuit                               |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

