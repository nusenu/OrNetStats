---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-02-27 16:00 UTC**

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
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                           | 0.09        | 0.3        | 3         | 2               | 2016-08-28     | 1                           |
| [https://www.torservers.net/donate.html &lt;support .A](endtoend-correlation-groups#httpswwwtorserversnetdonatehtml-support-a) | 0.06        | 2.63       | 12        | 3               | 2018-02-19     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                 | 0.05        | 0.62       | 7         | 2               | 2018-02-11     | 5                           |
| [wambo@cock.li](endtoend-correlation-groups#wambocockli)                                                                       | 0.05        | 0.03       | 2         | 2               | 2018-01-30     | 1                           |
| [tor-mngr AT scalaire DOT fr](endtoend-correlation-groups#tor-mngr-at-scalaire-dot-fr)                                         | 0.01        | 0.25       | 2         | 2               | 2017-11-27     | 1                           |
| **Total**                                                                                                                      | **0.26**    | **3.83**   | **26**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      8.07 |        32 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:C5A53BCC174EF8FD0DCB223E4AA929FA557DEDB2)    |      4.17 |        30 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      3.14 |        13 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |      2.74 |        11 | 2017-12-05   |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](https://metrics.torproject.org/rs.html#search/family:0EB06AD78563BDB1D3B5F5AE83C6B608BA4A4005) |      2.43 |        22 | 2016-11-12   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](https://metrics.torproject.org/rs.html#search/family:84D361B736A8CD1E8818D0FC186892E91AB76881) |      2.13 |        11 | 2013-06-11   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://metrics.torproject.org/rs.html#search/family:7016E939A2DD6EF2FB66A33F1DD45357458B737F)    |      1.78 |         8 | 2014-04-16   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      1.76 |         7 | 2014-04-09   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      1.67 |         7 | 2013-07-10   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      1.51 |         6 | 2017-11-29   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       1.34 |        17 | 2015-10-10   |
| [tor-relays@lists.torproject.org](https://metrics.torproject.org/rs.html#search/family:151BDD000832E22385680E456E4B94220317B122)                          |       0.96 |        10 | 2017-07-02   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://metrics.torproject.org/rs.html#search/family:B08E51FED96A7A7A6081ACC96299713F3F171B3A)               |       0.87 |         9 | 2017-02-08   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:71539D1911ECB826069A4D156771AC4F9F4632A7)              |       0.8  |         9 | 2018-01-07   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       0.68 |         7 | 2016-01-03   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       0.68 |         7 | 2014-04-22   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       0.58 |         6 | 2016-08-10   |
| [Anders Burmeister &lt;anders.burmeister AT protonmail](https://metrics.torproject.org/rs.html#search/family:92412EA1B9AA887D462B51D816777002F4D58907)    |       0.58 |         6 | 2017-02-11   |
| [0x7A8647DB Daniel Winzen &lt;d@winzen4.de&gt; - 1CHvjeMJ](https://metrics.torproject.org/rs.html#search/family:72B19BAABE6846DF96EA2A50C28F4DC15A920041) |       0.55 |         6 | 2016-05-16   |
| [see https://www.artikel5ev.de/torcontact/](https://metrics.torproject.org/rs.html#search/family:22404A3E87F2D7FE2FC6359FDE71B6DC2D6E730F)                |       0.49 |         9 | 2014-06-09   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |            1.669 |      8.07 |       0    |        32 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:C5A53BCC174EF8FD0DCB223E4AA929FA557DEDB2)    |            0.863 |      4.17 |       0    |        30 | 2016-08-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |            0.732 |      0    |       1.34 |        19 | 2015-05-16   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |            0.649 |      3.14 |       0    |        13 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |            0.566 |      2.74 |       0    |        11 | 2017-12-05   |
| [0x7A8647DB Daniel Winzen &lt;d@winzen4.de&gt; - 1CHvjeMJ](https://metrics.torproject.org/rs.html#search/family:72B19BAABE6846DF96EA2A50C28F4DC15A920041) |            0.545 |      0.96 |       0.55 |        11 | 2016-05-16   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](https://metrics.torproject.org/rs.html#search/family:84D361B736A8CD1E8818D0FC186892E91AB76881) |            0.519 |      2.13 |       0.04 |        13 | 2013-06-11   |
| [tor-relays@lists.torproject.org](https://metrics.torproject.org/rs.html#search/family:151BDD000832E22385680E456E4B94220317B122)                          |            0.516 |      0    |       0.96 |        10 | 2017-07-02   |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](https://metrics.torproject.org/rs.html#search/family:0EB06AD78563BDB1D3B5F5AE83C6B608BA4A4005) |            0.502 |      2.43 |       0    |        22 | 2016-11-12   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:D6103DC78470C070840C74D0D1F41AEC3E5DE1B3)              |            0.482 |      0    |       0.8  |        10 | 2018-01-07   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            13.83 |      18.32 |      9.38 |       503 |
| Online S.a.s.               |            10.23 |      12.29 |     10.48 |       370 |
| Hetzner Online GmbH         |             5.69 |       7.66 |      1.19 |       276 |
| DigitalOcean, LLC           |             5.39 |       6.61 |      3.09 |       281 |
| Contabo GmbH                |             1.33 |       1.96 |      0.84 |        47 |
| Host Europe GmbH            |             1.11 |       1.94 |      0    |        32 |
| Linode, LLC                 |             1.03 |       0.38 |      1.01 |       167 |
| Cogent Communications       |             0.99 |       1.67 |      0    |        30 |
| ISPpro Internet KG          |             0.96 |       1.52 |      0    |        30 |
| SOFTplus Entwicklungen GmbH |             0.95 |       0.24 |      4    |        19 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             48.9 |     46.23 |      50.96 |      2265 |
| 0.3.1         |             16.1 |     11.15 |      18.03 |      1075 |
| 0.2.9         |             13.8 |     10.2  |      12.26 |      1148 |
| 0.3.3         |             10.2 |     22.75 |       9.18 |       297 |
| 0.2.5         |              4.3 |      4.18 |       4.42 |       473 |
| 0.3.0         |              2.2 |      1.4  |       2.19 |       232 |
| 0.2.4         |              1.5 |      2.05 |       1.28 |       240 |
| 0.2.7         |              1.5 |      0.41 |       1.34 |       205 |
| 0.3.4         |              0.5 |      1.5  |       0    |        17 |
| 0.2.6         |              0.1 |      0.08 |       0.12 |        35 |
| 0.2.8         |              0.1 |      0.01 |       0.15 |        35 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.55 |       4.95 |      3.96 |       712 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.5 |      92   |       92   |      5531 |
| BSD     |              6.8 |       7.6 |        7.6 |       314 |
| Windows |              0.3 |       0.2 |        0   |       105 |
| SunOS   |              0.1 |       0   |        0.1 |         4 |
| Darwin  |              0   |       0   |        0   |        11 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.49 |      20.25 |       14.21 |     23.31 |       635 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     26.46 |            155 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1053 |
| None                                       |       584 |
| obfs3, obfs4, scramblesuit                 |       247 |
| obfs3, obfs4                               |        52 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        17 |
| obfs2, obfs3                               |         9 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| fte, obfs3, obfs4                          |         3 |
| meek                                       |         3 |
| scramblesuit                               |         3 |
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

