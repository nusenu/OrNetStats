---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-03-01 16:00 UTC**

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

| Contact                                                                                                                        | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                           | 0.1         | 0.31       | 3         | 2               | 2016-08-28     | 1                           |
| [https://www.torservers.net/donate.html &lt;support .A](endtoend-correlation-groups#httpswwwtorserversnetdonatehtml-support-a) | 0.06        | 2.59       | 12        | 3               | 2018-02-19     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                 | 0.05        | 1.18       | 7         | 2               | 2018-02-11     | 5                           |
| [tor-mngr AT scalaire DOT fr](endtoend-correlation-groups#tor-mngr-at-scalaire-dot-fr)                                         | 0.02        | 0.23       | 2         | 2               | 2017-11-27     | 1                           |
| **Total**                                                                                                                      | **0.23**    | **4.31**   | **24**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Exit(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      7.53 |        32 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:C5A53BCC174EF8FD0DCB223E4AA929FA557DEDB2)    |      3.9  |        30 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      3.06 |        13 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |      2.59 |        11 | 2017-12-05   |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](https://metrics.torproject.org/rs.html#search/family:0EB06AD78563BDB1D3B5F5AE83C6B608BA4A4005) |      2.32 |        22 | 2016-11-12   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:6F4E9FD00D4251D98BE96FB1AA546FE34676A95B) |      2.08 |        10 | 2013-06-11   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://metrics.torproject.org/rs.html#search/family:7016E939A2DD6EF2FB66A33F1DD45357458B737F)    |      1.82 |         8 | 2014-04-16   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      1.64 |         7 | 2014-04-09   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      1.55 |         7 | 2013-07-10   |
| [abuse aT nectodoT--onion](https://metrics.torproject.org/rs.html#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                                 |      1.41 |         6 | 2015-08-27   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       1.41 |        17 | 2015-10-10   |
| [tor-relays@lists.torproject.org](https://metrics.torproject.org/rs.html#search/family:151BDD000832E22385680E456E4B94220317B122)                          |       1.01 |        10 | 2017-07-02   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://metrics.torproject.org/rs.html#search/family:B08E51FED96A7A7A6081ACC96299713F3F171B3A)               |       0.92 |         9 | 2017-02-08   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:71539D1911ECB826069A4D156771AC4F9F4632A7)              |       0.84 |         9 | 2018-01-07   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       0.71 |         7 | 2016-01-03   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       0.71 |         7 | 2014-04-22   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       0.61 |         6 | 2016-08-10   |
| [Anders Burmeister &lt;anders.burmeister AT protonmail](https://metrics.torproject.org/rs.html#search/family:92412EA1B9AA887D462B51D816777002F4D58907)    |       0.61 |         6 | 2017-02-11   |
| [0x7A8647DB Daniel Winzen &lt;d@winzen4.de&gt; - 1CHvjeMJ](https://metrics.torproject.org/rs.html#search/family:72B19BAABE6846DF96EA2A50C28F4DC15A920041) |       0.58 |         6 | 2016-05-16   |
| [0x9501B909 Random Person &lt;deep.thought AT riseup d](https://metrics.torproject.org/rs.html#search/family:3F39BC367D7FCF3F631C49190F4D0C4312307A8F)    |       0.56 |         7 | 2017-02-20   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |            1.607 |      7.53 |       0    |        32 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:C5A53BCC174EF8FD0DCB223E4AA929FA557DEDB2)    |            0.832 |      3.9  |       0    |        30 | 2016-08-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |            0.705 |      0    |       1.41 |        19 | 2015-05-16   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |            0.652 |      3.06 |       0    |        13 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |            0.552 |      2.59 |       0    |        11 | 2017-12-05   |
| [0x7A8647DB Daniel Winzen &lt;d@winzen4.de&gt; - 1CHvjeMJ](https://metrics.torproject.org/rs.html#search/family:72B19BAABE6846DF96EA2A50C28F4DC15A920041) |            0.526 |      0.92 |       0.58 |        11 | 2016-05-16   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:6F4E9FD00D4251D98BE96FB1AA546FE34676A95B) |            0.509 |      2.08 |       0.13 |        12 | 2013-06-11   |
| [tor-relays@lists.torproject.org](https://metrics.torproject.org/rs.html#search/family:151BDD000832E22385680E456E4B94220317B122)                          |            0.496 |      0    |       1.01 |        10 | 2017-07-02   |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](https://metrics.torproject.org/rs.html#search/family:0EB06AD78563BDB1D3B5F5AE83C6B608BA4A4005) |            0.496 |      2.32 |       0    |        22 | 2016-11-12   |
| [see http://tor.piratenpartei-nrw.de](https://metrics.torproject.org/rs.html#search/family:E9289AF85E5EDEC87FD741AB5E4A62D2AF796F01)                      |            0.489 |      0.75 |       0.51 |        22 | 2014-04-11   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            13.85 |      18.54 |      9.58 |       514 |
| Online S.a.s.               |            10.01 |      11.86 |      9.94 |       365 |
| Hetzner Online GmbH         |             5.84 |       7.62 |      1.11 |       293 |
| DigitalOcean, LLC           |             5.27 |       6.76 |      2.74 |       297 |
| Contabo GmbH                |             1.31 |       1.89 |      0.78 |        46 |
| Linode, LLC                 |             1.15 |       0.39 |      1.26 |       180 |
| Host Europe GmbH            |             1.06 |       1.88 |      0    |        32 |
| Cogent Communications       |             0.93 |       1.54 |      0    |        28 |
| Choopa, LLC                 |             0.92 |       0.42 |      0    |        97 |
| SOFTplus Entwicklungen GmbH |             0.92 |       0.25 |      3.76 |        19 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             48.5 |     47.48 |      49.72 |      2303 |
| 0.3.1         |             15.6 |     11.22 |      16.97 |      1055 |
| 0.2.9         |             14.2 |     10.67 |      12.15 |      1130 |
| 0.3.3         |             11   |     21.62 |      11.48 |       324 |
| 0.2.5         |              4.2 |      4.36 |       4.25 |       474 |
| 0.3.0         |              2.2 |      1.27 |       2.52 |       223 |
| 0.2.4         |              1.4 |      1.34 |       1.25 |       251 |
| 0.2.7         |              1.4 |      0.51 |       1.24 |       205 |
| 0.3.4         |              0.5 |      1.4  |       0.06 |        16 |
| 0.2.8         |              0.2 |      0.01 |       0.16 |        39 |
| 0.2.6         |              0.1 |      0.08 |       0.15 |        34 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.44 |       5.17 |      3.21 |       713 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.5 |      91.1 |       91.8 |      5564 |
| BSD     |              6.9 |       8.6 |        7.8 |       305 |
| Windows |              0.3 |       0.1 |        0.1 |       106 |
| SunOS   |              0.1 |       0   |        0.2 |         4 |
| Darwin  |              0   |       0.1 |        0   |        10 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.39 |      20.14 |       13.76 |     23.73 |       649 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     26.76 |            157 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1034 |
| None                                       |       579 |
| obfs3, obfs4, scramblesuit                 |       246 |
| obfs3, obfs4                               |        55 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        17 |
| obfs2, obfs3                               |        11 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         3 |
| scramblesuit                               |         3 |
| fte, obfs3, obfs4                          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| fte, scramblesuit                          |         1 |
| meek, meek                                 |         1 |
| meek, obfs4                                |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

