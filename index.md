---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-09-30 21:00 UTC**

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
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb) | 0.14        | 0.75       | 13        | 2               | 2016-04-01     | 4                           |
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.08        | 0.07       | 4         | 3               | 2017-09-24     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)     | 0.06        | 0.28       | 4         | 4               | 2017-08-28     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                           | 0.06        | 0.48       | 5         | 2               | 2017-06-23     | 1                           |
| [Syncaddict &lt;tor-node-operations@syncaddict.net&gt;](endtoend-correlation-groups#syncaddict-tor-node-operationssyncaddictnet)         | 0.05        | 0.01       | 2         | 2               | 2017-08-09     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           | 0.05        | 1.02       | 3         | 3               | 2016-08-08     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                     | 0.04        | 0.02       | 3         | 2               | 2016-08-28     | 1                           |
| [Brandon Kuschel &lt;kusch023 AT nospam UMN dot edu.](endtoend-correlation-groups#brandon-kuschel-kusch023-at-nospam-umn-dot-edu)        | 0.01        | 0.07       | 2         | 2               | 2016-10-26     | 1                           |
| **Total**                                                                                                                                | **0.49**    | **2.70**   | **36**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |      5.83 |        21 | 2016-01-25   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      3.79 |         4 | 2014-11-21   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |      3.51 |         4 | 2014-04-09   |
| [abuse@blockone.cz](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)                                           |      2.73 |         1 | 2017-07-20   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.41 |         1 | 2014-04-19   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://atlas.torproject.org/#search/family:7016E939A2DD6EF2FB66A33F1DD45357458B737F) |      2.23 |         8 | 2014-04-16   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                 |      2.11 |         6 | 2016-04-02   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:C656B41AEFB40A141967EBF49D6E69603C9B4A11) |      2.05 |         5 | 2014-04-08   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9) |      1.94 |        26 | 2016-08-22   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                              |      1.63 |         7 | 2015-08-27   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       1.28 |        20 | 2015-05-16   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |       1.22 |        24 | 2014-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.08 |         6 | 2014-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       1.02 |         7 | 2016-08-10   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |       0.91 |         8 | 2016-07-26   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |       0.9  |         5 | 2016-12-23   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       0.89 |         7 | 2016-01-03   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:8672E8A01B4D3FA4C0BBE21C740D4506302EA487)                      |       0.87 |         6 | 2016-03-10   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                  |       0.85 |        10 | 2014-04-10   |
| [noc@cymru.com](https://atlas.torproject.org/#search/family:896FCE19CB53A73A21DC874977C06B28FC9A8BBA)                                         |       0.69 |         6 | 2011-11-29   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.418 |      5.83 |       0.43 |        29 | 2016-01-25   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.903 |      0    |       1.22 |        28 | 2014-12-23   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.877 |      0    |       1.28 |        22 | 2015-05-16   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |            0.87  |      1.33 |       0.9  |         9 | 2014-02-13   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9) |            0.814 |      1.94 |       0    |        49 | 2016-08-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.793 |      0.52 |       1.02 |         8 | 2016-08-10   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.789 |      0    |       1.08 |         7 | 2014-04-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.733 |      3.79 |       0    |         4 | 2014-11-21   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            0.678 |      3.51 |       0    |         4 | 2014-04-09   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            0.616 |      0    |       0.91 |         8 | 2016-07-26   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            21.68 |      24.52 |     19.91 |       910 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            19.31 |      21.71 |      6.98 |      1309 |
| [United States](https://atlas.torproject.org/#search/country:us)  |            13.47 |      11.48 |     16.9  |      1145 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            10.95 |      10.34 |     13.51 |       493 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             5.35 |       5.3  |      7.5  |       279 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             3.89 |       3.48 |      3.9  |       251 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.51 |       3.87 |      3.05 |       192 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.52 |       1.56 |      6.67 |        86 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.22 |       2.26 |      1.85 |       150 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             1.97 |       1.93 |      0.86 |       311 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            16.42 |      18.65 |     14.49 |       597 |
| Online S.a.s.       |            11.81 |      13.24 |     12.66 |       428 |
| Digital Ocean, Inc. |             7.27 |       8.75 |      1.75 |       348 |
| Hetzner Online GmbH |             7.18 |       8.9  |      1.04 |       310 |
| Host Europe GmbH    |             1.76 |       2.51 |      0    |        46 |
| myLoc managed IT AG |             1.71 |       1.44 |      0.9  |        52 |
| SURFnet bv          |             1.13 |       1.23 |      1.54 |        10 |
| ITL Company         |             1.01 |       1.32 |      0.26 |        48 |
| ISPpro Internet KG  |             0.96 |       1.38 |      0    |        34 |
| Linode, LLC         |             0.85 |       0.44 |      0.55 |       197 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.0         |             37.8 |     39.21 |      38.69 |      1966 |
| 0.3.1         |             24.6 |     34.73 |      21.47 |      1243 |
| 0.2.9         |             17.8 |     12.13 |      19.64 |      1360 |
| 0.2.5         |              7.4 |      7.73 |       6.95 |       772 |
| 0.2.7         |              4.1 |      0.9  |       4.4  |       527 |
| 0.3.2         |              2.6 |      3.28 |       2.62 |        74 |
| 0.2.8         |              2.4 |      0.85 |       3.17 |       162 |
| 0.2.4         |              2   |      0.49 |       1.99 |       437 |
| 0.2.6         |              0.8 |      0.64 |       1.02 |        69 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             7.07 |       7.42 |      2.05 |      1033 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.6 |      90.2 |       92.6 |      6088 |
| BSD     |              6.9 |       9.4 |        7   |       319 |
| Windows |              0.2 |       0.3 |        0   |       174 |
| Darwin  |              0   |       0   |        0   |        10 |
| SunOS   |              0   |       0   |        0.1 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.03 |      18.13 |       15.37 |     23.35 |       563 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     27.94 |            121 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1446 |
| None                                       |       680 |
| obfs3, obfs4, scramblesuit                 |       248 |
| obfs3, obfs4                               |        69 |
| obfs3                                      |        23 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3, obfs4                        |        10 |
| obfs2, obfs3                               |         9 |
| obfs3, scramblesuit                        |         9 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| meek                                       |         5 |
| fte, obfs3, obfs4                          |         4 |
| obfs2, obfs3, obfs4, scramblesuit          |         3 |
| obfs4, scramblesuit                        |         2 |
| scramblesuit                               |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| snowflake                                  |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

