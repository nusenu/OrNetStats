---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-08-11 15:00 UTC**

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

| Contact                                                                                             | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:----------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [tomas.vanagas@knf.vu.lt tor-relay.co](endtoend-correlation-groups#tomasvanagasknfvult-tor-relayco) | 0.02        | 0.06       | 2         | 2               | 2020-04-28     | 1                           |
| **Total**                                                                                           | **0.02**    | **0.06**   | **2**     |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     17.83 |       113 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)  |      7.87 |        32 | 2018-03-21   |
| [exitrelays@protonmail.com](https://metrics.torproject.org/rs.html#search/family:0828A52E57E4C426742B9264A210394202CD44D4)                                |      7.28 |        30 | 2020-07-08   |
| [kleinendorstwiebe AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:01C05513D12F63AE9E72588E8EAB459028C44689)                       |      5.39 |        27 | 2020-06-20   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      3.51 |        22 | 2018-03-01   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.3  |        17 | 2016-12-23   |
| [Digitalcourage Tor Team &lt;tor-abuse@digitalcourage.](https://metrics.torproject.org/rs.html#search/family:22296CB6AE56609A96F02FB843AB7B4B0A31CAF4)    |      2.85 |        17 | 2016-05-27   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      1.75 |        19 | 2013-06-11   |
| [ian@ian.sh](https://metrics.torproject.org/rs.html#search/family:0C9D7DB63BE030E5CA32E25606632AEB85840F4C)                                               |      1.56 |        32 | 2020-07-04   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      1.51 |        15 | 2014-04-09   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                             |   Guard(%) |   #Relays | First Seen   |
|:-----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [cockcockcockcock at cock dot li](https://metrics.torproject.org/rs.html#search/family:0219C961F781986D60EA94C59644AF34C6078B20)               |       2.39 |        31 | 2020-08-02   |
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:02758CD398E3F842EF82478078AAAE0273770DB2)         |       2.29 |        31 | 2019-01-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)           |       1.43 |        14 | 2018-10-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE) |       1.32 |        25 | 2015-05-16   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                      |       0.75 |         5 | 2017-10-24   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                      |       0.72 |         5 | 2016-09-06   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)   |       0.71 |        14 | 2018-01-07   |
| [63540827](https://metrics.torproject.org/rs.html#search/family:63540827C4832D214984EA47B7A68C593F9F862F)                                      |       0.64 |         2 | 2018-12-12   |
| [abuse@for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                         |       0.62 |        10 | 2019-03-16   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:14E72D4DA10B66353E583F26EE04AC0D563EA7EF)            |       0.61 |        27 | 2019-02-23   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                       |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:---------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                   |            6.643 |     17.83 |       2.29 |       144 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737) |            2.346 |      7.87 |       0    |        32 | 2018-03-21   |
| [exitrelays@protonmail.com](https://metrics.torproject.org/rs.html#search/family:0828A52E57E4C426742B9264A210394202CD44D4)                               |            2.171 |      7.28 |       0    |        30 | 2020-07-08   |
| [kleinendorstwiebe AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:01C05513D12F63AE9E72588E8EAB459028C44689)                      |            1.605 |      5.39 |       0    |        27 | 2020-06-20   |
| [cockcockcockcock at cock dot li](https://metrics.torproject.org/rs.html#search/family:0219C961F781986D60EA94C59644AF34C6078B20)                         |            1.412 |      0.07 |       2.39 |        32 | 2020-08-02   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)       |            1.112 |      3.51 |       0.11 |        26 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)   |            0.985 |      3.3  |       0    |        17 | 2016-12-23   |
| [Digitalcourage Tor Team &lt;tor-abuse@digitalcourage.](https://metrics.torproject.org/rs.html#search/family:22296CB6AE56609A96F02FB843AB7B4B0A31CAF4)   |            0.85  |      2.85 |       0    |        17 | 2016-05-27   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                     |            0.833 |      0    |       1.43 |        14 | 2018-10-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)           |            0.769 |      0    |       1.32 |        25 | 2015-05-16   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                 |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                 |            17.23 |      17.95 |     20.54 |       615 |
| Hetzner Online GmbH     |            15.92 |      22.63 |      0.05 |       443 |
| Online S.a.s.           |             7.05 |      11.07 |      1.74 |       234 |
| Joshua Peter McQuistan  |             6.14 |       1.43 |     17.83 |       138 |
| Liteserver Holding B.V. |             2.66 |       0    |      8.92 |        74 |
| netcup GmbH             |             2.36 |       2.81 |      0.57 |       118 |
| F3 Netze e.V.           |             2.34 |       0    |      7.87 |        32 |
| myLoc managed IT AG     |             1.85 |       2.59 |      1.02 |        44 |
| Zwiebelfreunde e.V.     |             1.26 |       0    |      4.25 |        22 |
| Contabo GmbH            |             1.1  |       1.69 |      0.12 |        83 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.3         |             61.3 |     70.11 |      55.32 |      3879 |
| 0.4.2         |             20   |     26.27 |      17.59 |      1356 |
| 0.3.5         |             13   |      1.73 |      18.87 |      1064 |
| 0.4.1         |              2.8 |      0.53 |       4.27 |       218 |
| 0.4.4         |              2.4 |      0.71 |       3.78 |       118 |
| 0.4.5         |              0.2 |      0.62 |       0.15 |        16 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|              3.1 |       4.42 |      1.16 |       234 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93   |      93.4 |       92.7 |      6091 |
| BSD     |              6.7 |       6.4 |        7   |       458 |
| Windows |              0   |       0   |        0   |        41 |
| Darwin  |              0   |       0   |        0   |         8 |
| SunOS   |              0   |       0   |        0   |         3 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            33.49 |      29.13 |       27.66 |     45.48 |      1423 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     46.53 |            461 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                   |   Bridges |
|:---------------------------------------|----------:|
| obfs4                                  |      1039 |
| None                                   |       410 |
| obfs3, obfs4                           |        71 |
| meek                                   |         4 |
| obfs3, obfs4, scramblesuit             |         4 |
| obfs2, obfs3, obfs4                    |         3 |
| obfs3                                  |         2 |
| fte, obfs2, obfs3, obfs4, scramblesuit |         1 |
| fte, obfs3, obfs4                      |         1 |
| fte, obfs3, obfs4, scramblesuit        |         1 |
| fte, obfs4                             |         1 |
| meek, meek                             |         1 |
| meek, obfs3, obfs4                     |         1 |
| obfs3, scramblesuit                    |         1 |
| obfs4, scramblesuit                    |         1 |
| obfs4, websocket                       |         1 |
| websocket                              |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

