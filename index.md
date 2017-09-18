---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-09-18 20:00 UTC**

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
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                 | 0.06        | 0.02       | 3         | 2               | 2016-08-28     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv) | 0.06        | 0.43       | 4         | 4               | 2017-08-28     | 1                           |
| [George Shuklin &lt;george.shuklin@gmail.com&gt;](endtoend-correlation-groups#george-shuklin-georgeshuklingmailcom)                  | 0.05        | 0.01       | 2         | 2               | 2016-07-21     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                       | 0.04        | 0.44       | 5         | 2               | 2017-06-23     | 1                           |
| [Syncaddict &lt;tor-node-operations@syncaddict.net&gt;](endtoend-correlation-groups#syncaddict-tor-node-operationssyncaddictnet)     | 0.02        | 0.01       | 2         | 2               | 2017-08-09     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                       | 0.02        | 0.97       | 3         | 3               | 2016-08-08     | 1                           |
| [Random Person &lt;determine AT riseup dot net&gt;](endtoend-correlation-groups#random-person-determine-at-riseup-dot-net)           | 0.01        | 0.03       | 2         | 2               | 2017-09-03     | 1                           |
| **Total**                                                                                                                            | **0.26**    | **1.91**   | **21**    |                 |                |                             |

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
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      6.3  |         7 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      4.25 |        20 | 2016-01-25   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      3.26 |         4 | 2014-11-21   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9)    |      2.79 |        50 | 2016-08-22   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:E34E25D958D46DDE5092385B14117C9B301DC0E9)     |      2.62 |        17 | 2014-05-19   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.25 |         3 | 2014-11-04   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://atlas.torproject.org/#search/family:7016E939A2DD6EF2FB66A33F1DD45357458B737F)    |      2.03 |         8 | 2014-04-16   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      1.91 |         6 | 2014-04-08   |
| [abuse@blockone.cz](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)                                              |      1.88 |         1 | 2017-07-20   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                    |      1.84 |         6 | 2016-04-02   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.55 |         3 | 2015-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |       1.35 |        24 | 2014-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.3  |         6 | 2014-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       1.17 |         7 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       1.17 |        20 | 2015-05-16   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |       1.05 |         5 | 2016-12-23   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |       0.92 |         8 | 2016-07-26   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:8672E8A01B4D3FA4C0BBE21C740D4506302EA487)                      |       0.78 |         6 | 2016-03-10   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       0.71 |         7 | 2016-01-03   |
| [tor terjan net](https://atlas.torproject.org/#search/family:A0E3D30A660DB70CA0B6D081BA54D094DED6F28D)                                        |       0.58 |         9 | 2015-03-05   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            1.243 |      6.3  |       0    |         7 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.154 |      4.25 |       0.42 |        28 | 2016-01-25   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            1.046 |      0    |       1.55 |         3 | 2015-04-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |            1.019 |      1.54 |       1.05 |         8 | 2014-02-13   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.978 |      0    |       1.35 |        26 | 2014-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.944 |      0    |       1.3  |         7 | 2014-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.836 |      0.23 |       1.17 |         8 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.803 |      0    |       1.17 |        22 | 2015-05-16   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.643 |      3.26 |       0    |         4 | 2014-11-21   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            0.622 |      0    |       0.92 |         8 | 2016-07-26   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.0         |             54.6 |     56.83 |      54.72 |      3000 |
| 0.2.9         |             18.4 |     10.85 |      20.83 |      1367 |
| 0.2.5         |              8.2 |      8.51 |       7.51 |       827 |
| 0.3.1         |              6.7 |     12.54 |       5.76 |       260 |
| 0.2.7         |              4.6 |      1.27 |       4.79 |       618 |
| 0.2.8         |              2.8 |      1.81 |       3.33 |       199 |
| 0.2.4         |              2.6 |      3.11 |       1.99 |       499 |
| 0.3.2         |              0.9 |      4.54 |       0.08 |        20 |
| 0.2.6         |              0.7 |      0.49 |       0.94 |        76 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             8.09 |       7.74 |      4.88 |      1193 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.8 |      89.4 |       93.5 |      6318 |
| BSD     |              6.5 |       9.7 |        6.2 |       332 |
| Windows |              0.3 |       0.7 |        0.1 |       184 |
| SunOS   |              0   |       0   |        0   |         4 |
| Darwin  |              0   |       0   |        0   |        11 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.87 |      18.82 |       15.82 |      25.2 |       575 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     29.23 |            133 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      2334 |
| None                                       |       699 |
| obfs3, obfs4, scramblesuit                 |       250 |
| obfs3, obfs4                               |        69 |
| obfs3                                      |        22 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3, obfs4                        |        10 |
| obfs2, obfs3                               |         9 |
| obfs3, scramblesuit                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| meek                                       |         5 |
| obfs2, obfs3, obfs4, scramblesuit          |         3 |
| fte, obfs3, obfs4                          |         2 |
| obfs4, scramblesuit                        |         2 |
| scramblesuit                               |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| obfs3 websocket, websocket                 |         1 |
| snowflake                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

