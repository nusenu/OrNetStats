---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-09-29 15:00 UTC**

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
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.13        | 0.06       | 4         | 3               | 2017-09-24     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb) | 0.11        | 0.83       | 13        | 2               | 2016-04-01     | 4                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)     | 0.08        | 0.51       | 4         | 4               | 2017-08-28     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                           | 0.07        | 0.5        | 5         | 2               | 2017-06-23     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                     | 0.04        | 0.02       | 3         | 2               | 2016-08-28     | 1                           |
| [Syncaddict &lt;tor-node-operations@syncaddict.net&gt;](endtoend-correlation-groups#syncaddict-tor-node-operationssyncaddictnet)         | 0.04        | 0.01       | 2         | 2               | 2017-08-09     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           | 0.04        | 1.22       | 3         | 3               | 2016-08-08     | 1                           |
| [Brandon Kuschel &lt;kusch023 AT nospam UMN dot edu.](endtoend-correlation-groups#brandon-kuschel-kusch023-at-nospam-umn-dot-edu)        | 0.01        | 0.07       | 2         | 2               | 2016-10-26     | 1                           |
| **Total**                                                                                                                                | **0.52**    | **3.22**   | **36**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      7.1  |        21 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      3.29 |         4 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      3.26 |         4 | 2014-11-21   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:C656B41AEFB40A141967EBF49D6E69603C9B4A11)    |      2.51 |         5 | 2014-04-08   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.5  |         3 | 2014-11-04   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.43 |         1 | 2014-04-19   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://atlas.torproject.org/#search/family:7016E939A2DD6EF2FB66A33F1DD45357458B737F)    |      2.4  |         8 | 2014-04-16   |
| [abuse@blockone.cz](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)                                              |      2.34 |         1 | 2017-07-20   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                                 |      1.99 |         7 | 2015-08-27   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                    |      1.86 |         6 | 2016-04-02   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       1.37 |        20 | 2015-05-16   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                    |       1.22 |        24 | 2014-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       1.22 |         6 | 2014-04-22   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:8672E8A01B4D3FA4C0BBE21C740D4506302EA487)                         |       1.02 |         6 | 2016-03-10   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       1.02 |         7 | 2016-01-03   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)            |       0.96 |         7 | 2016-08-10   |
| [Schizopriest &lt;tor AT schizopriest DOT de&gt; - 1PNQeR](https://atlas.torproject.org/#search/family:49E7AD01BB96F6FE3AB8C3B15BD2470B150354DF) |       0.84 |         2 | 2015-10-31   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                                 |       0.8  |         8 | 2016-07-26   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                     |       0.8  |        10 | 2014-04-10   |
| [noc@cymru.com](https://atlas.torproject.org/#search/family:896FCE19CB53A73A21DC874977C06B28FC9A8BBA)                                            |       0.65 |         6 | 2011-11-29   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                               |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |            1.583 |      7.1  |       0.39 |        29 | 2016-01-25   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |            0.955 |      0    |       1.37 |        22 | 2015-05-16   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                    |            0.921 |      0    |       1.22 |        28 | 2014-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |            0.902 |      0    |       1.22 |         7 | 2014-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)            |            0.756 |      0.53 |       0.96 |         8 | 2016-08-10   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |            0.701 |      0    |       1.02 |         7 | 2016-01-03   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:8672E8A01B4D3FA4C0BBE21C740D4506302EA487)                         |            0.701 |      0    |       1.02 |         8 | 2016-03-10   |
| [Schizopriest &lt;tor AT schizopriest DOT de&gt; - 1PNQeR](https://atlas.torproject.org/#search/family:49E7AD01BB96F6FE3AB8C3B15BD2470B150354DF) |            0.624 |      0    |       0.84 |         3 | 2015-10-31   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |            0.607 |      3.29 |       0    |         4 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |            0.602 |      3.26 |       0    |         4 | 2014-11-21   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            22.6  |      25.64 |     20.89 |       900 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            20.14 |      22.74 |      6.86 |      1325 |
| [United States](https://atlas.torproject.org/#search/country:us)  |            12.56 |      11.02 |     15.46 |      1112 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            11.65 |      10.51 |     14.81 |       501 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             5.04 |       4.68 |      7.77 |       281 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             3.76 |       3.46 |      3.79 |       254 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             2.88 |       2.92 |      2.73 |       187 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.28 |       2.26 |      2.19 |       149 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.23 |       1.57 |      5.35 |        86 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             1.93 |       1.79 |      1.05 |       320 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            16.68 |      18.89 |     15.59 |       599 |
| Online S.a.s.       |            11.83 |      13.42 |     12.49 |       427 |
| Hetzner Online GmbH |             7.54 |       9.28 |      1.02 |       316 |
| Digital Ocean, Inc. |             7.35 |       8.75 |      1.82 |       359 |
| Host Europe GmbH    |             1.93 |       2.73 |      0    |        46 |
| myLoc managed IT AG |             1.72 |       1.63 |      0.87 |        50 |
| SURFnet bv          |             1.38 |       1.06 |      1.56 |        11 |
| ITL Company         |             1    |       1.29 |      0.29 |        48 |
| ISPpro Internet KG  |             0.93 |       1.33 |      0    |        34 |
| Linode, LLC         |             0.83 |       0.53 |      0.49 |       200 |

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.0         |             39.5 |     44.33 |      39.39 |      2055 |
| 0.3.1         |             22   |     26.15 |      21.46 |      1118 |
| 0.2.9         |             18.7 |     12.87 |      20.38 |      1381 |
| 0.2.5         |              7.5 |      8.19 |       6.86 |       778 |
| 0.2.7         |              4.2 |      0.99 |       4.53 |       534 |
| 0.2.8         |              2.7 |      1.67 |       3.26 |       173 |
| 0.2.4         |              2.1 |      0.5  |       2.01 |       446 |
| 0.3.2         |              2.1 |      4.55 |       1.13 |        62 |
| 0.2.6         |              0.8 |      0.69 |       0.93 |        72 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             7.28 |       7.48 |      2.19 |      1052 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.4 |      90.1 |       92.4 |      6089 |
| BSD     |              7.1 |       9.8 |        7.3 |       321 |
| Windows |              0.2 |       0   |        0   |       179 |
| Darwin  |              0.1 |       0   |        0   |        11 |
| SunOS   |              0.1 |       0   |        0.1 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            17.05 |      16.48 |       15.41 |     21.93 |       556 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     27.41 |            122 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1455 |
| None                                       |       687 |
| obfs3, obfs4, scramblesuit                 |       248 |
| obfs3, obfs4                               |        70 |
| obfs3                                      |        22 |
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

