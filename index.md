---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-10-03 17:00 UTC**

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
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)              | 0.09        | 0.18       | 4         | 3               | 2017-09-24     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                 | 0.05        | 0.02       | 3         | 2               | 2016-08-28     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv) | 0.05        | 0.35       | 4         | 4               | 2017-08-28     | 1                           |
| [Syncaddict &lt;tor-node-operations@syncaddict.net&gt;](endtoend-correlation-groups#syncaddict-tor-node-operationssyncaddictnet)     | 0.05        | 0.01       | 2         | 2               | 2017-08-09     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                       | 0.04        | 0.38       | 5         | 2               | 2017-06-23     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                       | 0.03        | 0.86       | 3         | 3               | 2016-08-08     | 1                           |
| **Total**                                                                                                                            | **0.31**    | **1.80**   | **21**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      6.58 |        21 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      5.8  |         5 | 2014-04-09   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9)    |      3.59 |        50 | 2016-08-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      2.85 |         4 | 2014-11-21   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.29 |         3 | 2014-11-04   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.27 |         1 | 2014-04-19   |
| [abuse@blockone.cz](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)                                              |      2.07 |         1 | 2017-07-20   |
| [Tor Manager &lt;tor@ibiblio.org&gt;](https://atlas.torproject.org/#details/C59E079437340E3AD14E6785C0A91A5B6F328566)                            |      2.06 |         1 | 2017-07-27   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:C656B41AEFB40A141967EBF49D6E69603C9B4A11)    |      1.98 |         5 | 2014-04-08   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                    |      1.97 |         6 | 2016-04-02   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       1.23 |        19 | 2015-05-16   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                    |       1.22 |        24 | 2014-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       1.22 |         6 | 2014-04-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       1.16 |         7 | 2016-01-03   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)            |       1.12 |         7 | 2016-08-10   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                      |       0.92 |         3 | 2015-04-22   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                                 |       0.84 |         8 | 2016-07-26   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:8672E8A01B4D3FA4C0BBE21C740D4506302EA487)                         |       0.82 |         6 | 2016-03-10   |
| [info AT omuravpn.com](https://atlas.torproject.org/#search/family:94C0F99BA44AA4A6767C71333B8A66DBD1BC08C7)                                     |       0.69 |         5 | 2017-01-05   |
| [Schizopriest &lt;tor AT schizopriest DOT de&gt; - 1PNQeR](https://atlas.torproject.org/#search/family:49E7AD01BB96F6FE3AB8C3B15BD2470B150354DF) |       0.64 |         3 | 2015-10-31   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.621 |      6.58 |       0.33 |        29 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            1.24  |      5.8  |       0    |         5 | 2014-04-09   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |            0.907 |      1.64 |       0    |         9 | 2014-02-13   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.881 |      0    |       1.22 |        28 | 2014-12-23   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.844 |      0    |       1.23 |        22 | 2015-05-16   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.829 |      0    |       1.22 |         7 | 2014-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.784 |      0.32 |       1.12 |         8 | 2016-08-10   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9) |            0.768 |      3.59 |       0    |        50 | 2016-08-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |            0.744 |      0    |       1.16 |         7 | 2016-01-03   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.61  |      2.85 |       0    |         4 | 2014-11-21   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            21.19 |      24.99 |     17.82 |       921 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            19.33 |      22.15 |      5.88 |      1328 |
| [United States](https://atlas.torproject.org/#search/country:us)  |            13.79 |      11.5  |     18.72 |      1193 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            11.39 |      10.95 |     14.33 |       521 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             5.07 |       4.89 |      6.88 |       285 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             3.43 |       3.24 |      3.58 |       256 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.43 |       2.8  |      3.03 |       190 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.73 |       1.5  |      7.43 |        86 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.28 |       2.31 |      2.35 |       153 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             2.02 |       1.98 |      1.04 |       326 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            15.8  |      18.27 |     13.31 |       599 |
| Online S.a.s.       |            11.74 |      13.84 |     12.04 |       433 |
| Hetzner Online GmbH |             7.13 |       8.81 |      0.44 |       317 |
| Digital Ocean, Inc. |             6.77 |       8.44 |      1.46 |       372 |
| myLoc managed IT AG |             1.73 |       1.53 |      0.94 |        40 |
| Host Europe GmbH    |             1.71 |       2.54 |      0    |        46 |
| SURFnet bv          |             1.31 |       1.75 |      0.88 |        11 |
| Linode, LLC         |             1.29 |       0.51 |      1.35 |       222 |
| ITL Company         |             0.96 |       1.33 |      0.23 |        45 |
| ISPpro Internet KG  |             0.93 |       1.43 |      0    |        34 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.0         |             37.4 |     38.92 |      38.51 |      1942 |
| 0.3.1         |             26.6 |     35.32 |      24.36 |      1382 |
| 0.2.9         |             17.4 |     11.73 |      19.02 |      1409 |
| 0.2.5         |              6.9 |      7.07 |       6.58 |       776 |
| 0.2.7         |              3.6 |      0.29 |       4.08 |       516 |
| 0.3.2         |              2.7 |      4.7  |       1.37 |        85 |
| 0.2.8         |              2.4 |      0.78 |       3.3  |       163 |
| 0.2.4         |              1.9 |      0.7  |       1.85 |       430 |
| 0.2.6         |              0.7 |      0.46 |       0.89 |        74 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             6.32 |       6.82 |      1.46 |      1020 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.5 |      91.2 |       92   |      6237 |
| BSD     |              7.1 |       8.7 |        7.6 |       328 |
| Windows |              0.1 |       0   |        0   |       182 |
| SunOS   |              0.1 |       0   |        0.1 |         4 |
| Darwin  |              0   |       0   |        0   |        15 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.11 |      17.38 |       15.82 |     23.68 |       574 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     27.72 |            124 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1431 |
| None                                       |       699 |
| obfs3, obfs4, scramblesuit                 |       248 |
| obfs3, obfs4                               |        72 |
| obfs3                                      |        23 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3                               |        10 |
| obfs2, obfs3, obfs4                        |        10 |
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

