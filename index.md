---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-04-29 14:00 UTC**

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

| Contact                                                                                                   | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:----------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain) | 0.11        | 0.14       | 6         | 6               | 2018-12-23     | 1                           |
| [tomas.vanagas@knf.vu.lt tor-relay.co](endtoend-correlation-groups#tomasvanagasknfvult-tor-relayco)       | 0.02        | 0.39       | 4         | 3               | 2019-04-09     | 1                           |
| **Total**                                                                                                 | **0.13**    | **0.53**   | **10**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).


## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Exit(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                         |     11.56 |        45 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |      6.63 |        48 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |      6.31 |        17 | 2016-12-23   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |      6.24 |        10 | 2018-03-23   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:0C6842CCF836DE08EFEA0BD6C1471AE3463B9B71)                                 |      2.74 |        24 | 2019-04-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      2.52 |        13 | 2015-05-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      1.99 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      1.92 |        12 | 2017-12-05   |
| [18CFB7BA](https://metrics.torproject.org/rs.html#search/family:18CFB7BA07F13AEABF50A7148786DA68773B2498)                                              |      1.72 |         2 | 2018-12-15   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      1.56 |         4 | 2014-11-21   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                  |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                      |       1.53 |        16 | 2019-01-05   |
| [email:tor appliedprivacy.net twitter:applied priv](https://metrics.torproject.org/rs.html#search/family:113143469021882C3A4B82F084F8125B08EE471E)  |       0.98 |         9 | 2017-06-13   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                           |       0.88 |         4 | 2018-08-17   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                |       0.74 |         3 | 2015-04-22   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                           |       0.65 |         5 | 2017-10-24   |
| [jwbecher@drazisil.com](https://metrics.torproject.org/rs.html#search/family:46FBC671FD6FCE6B298B2BAE3C7AC7D7DDF1365F)                              |       0.63 |         6 | 2018-05-08   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)   |       0.62 |        15 | 2016-12-11   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:3B4C5729F829CA2E895B81AF834A63DB336D0FFE)        |       0.61 |        13 | 2018-01-07   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:39F91959416763AFD34DBEEC05474411B964B2DC)                               |       0.61 |        18 | 2018-08-28   |
| [emerson tor@nodevine.net bitcoin:126gyYcBjirRmDh2G](https://metrics.torproject.org/rs.html#search/family:19C38081249BC20F4F404018603DB11A0A0AD8A0) |       0.56 |        22 | 2018-12-27   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                         |            3.901 |     11.56 |       1.53 |        61 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            2.208 |      6.24 |       0.98 |        19 | 2017-06-13   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |            1.659 |      6.63 |       0    |        48 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |            1.581 |      6.31 |       0    |        17 | 2016-12-23   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:13E8EB1D9FD7470AA87A47DC93538E88340A0903)      |            0.732 |      0.99 |       0.62 |        20 | 2016-10-28   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.7   |      0    |       0.46 |         8 | 2018-10-05   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:0C6842CCF836DE08EFEA0BD6C1471AE3463B9B71)                                 |            0.697 |      2.74 |       0    |        25 | 2019-04-05   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |            0.635 |      0    |       0.88 |         5 | 2016-09-06   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.63  |      2.52 |       0    |        13 | 2015-05-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.498 |      1.99 |       0    |         1 | 2014-04-19   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                                                          |            14.52 |      17.68 |     10.1  |       581 |
| Hetzner Online GmbH                                              |            13.88 |      18.45 |      0.12 |       392 |
| Online S.a.s.                                                    |            10.91 |      13.18 |      4.84 |       313 |
| Joshua Peter McQuistan                                           |             2.95 |       0.08 |     11.56 |        46 |
| iomart Cloud Services Limited.                                   |             2.65 |       3.26 |      0    |        21 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             2.13 |       0.86 |      6.24 |        17 |
| netcup GmbH                                                      |             2.01 |       2.7  |      0.34 |        79 |
| myLoc managed IT AG                                              |             1.81 |       2.33 |      1.08 |        44 |
| NForce Entertainment B.V.                                        |             1.78 |       1.36 |      3.5  |        32 |
| Quintex Alliance Consulting                                      |             1.65 |       0    |      6.63 |        48 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.5         |             54.8 |     64.81 |      51.59 |      3363 |
| 0.3.4         |             19.5 |      5.64 |      25.63 |      1002 |
| 0.2.9         |              9.3 |      5.33 |      10    |      1051 |
| 0.4.0         |              6.3 |      9.86 |       5.01 |       183 |
| 0.3.2         |              5.7 |     11.48 |       4.06 |       286 |
| 0.3.3         |              1.7 |      0.78 |       1.95 |       220 |
| 0.4.1         |              1   |      0.95 |       0.65 |        23 |
| 0.2.5         |              0.5 |      0.92 |       0.21 |       127 |
| 0.3.1         |              0.4 |      0.15 |       0.57 |        62 |
| 0.2.4         |              0.2 |      0.03 |       0.08 |       126 |
| 0.2.6         |              0   |      0    |       0.02 |        20 |
| 0.2.7         |              0   |      0    |       0.03 |        75 |
| 0.2.8         |              0   |      0    |       0.04 |        21 |
| 0.3.0         |              0   |      0    |       0.08 |        54 |
| 0.3.6         |              0   |      0    |       0    |         1 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             8.93 |       7.09 |     13.38 |       992 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.3 |      84.5 |       93.3 |      6089 |
| BSD     |              8.4 |      15.3 |        6.3 |       397 |
| Windows |              0.1 |       0   |        0   |        80 |
| SunOS   |              0   |       0   |        0   |         5 |
| Darwin  |              0   |       0   |        0.1 |        13 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            28.08 |      24.42 |        24.5 |     38.91 |      1053 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     40.24 |            271 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       480 |
| None                                       |       417 |
| obfs3, obfs4                               |        57 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3, obfs4                        |         6 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         5 |
| obfs3, obfs4, scramblesuit                 |         5 |
| fte, meek, obfs3, obfs4                    |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| meek, meek                                 |         1 |
| obfs2, obfs3                               |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

