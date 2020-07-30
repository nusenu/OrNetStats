---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-07-30 20:00 UTC**

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

| Contact                                            | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:---------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [ian@ian.sh](endtoend-correlation-groups#ianiansh) | 0.05        | 1.57       | 39        | 12              | 2020-07-30     | 12                          |
| **Total**                                          | **0.05**    | **1.57**   | **39**    |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     20.77 |       113 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)  |      8.17 |        32 | 2018-03-21   |
| [exitrelays@protonmail.com](https://metrics.torproject.org/rs.html#search/family:0828A52E57E4C426742B9264A210394202CD44D4)                                |      6.61 |        30 | 2020-07-08   |
| [kleinendorstwiebe AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:01C05513D12F63AE9E72588E8EAB459028C44689)                       |      6.06 |        27 | 2020-06-20   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      3.77 |        18 | 2018-03-01   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.7  |        17 | 2016-12-23   |
| [Digitalcourage Tor Team &lt;tor-abuse@digitalcourage.](https://metrics.torproject.org/rs.html#search/family:22296CB6AE56609A96F02FB843AB7B4B0A31CAF4)    |      2.87 |        17 | 2016-05-27   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      2    |        19 | 2013-06-11   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      1.53 |        15 | 2014-04-09   |
| [ian@ian.sh](https://metrics.torproject.org/rs.html#search/family:0F59911D698D3FFE2433B7AB31362FB1EA10237F)                                               |      1.52 |        22 | 2020-07-04   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                             |   Guard(%) |   #Relays | First Seen   |
|:-----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:02758CD398E3F842EF82478078AAAE0273770DB2)         |       2.56 |        31 | 2019-01-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)           |       1.41 |        14 | 2018-10-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE) |       1.17 |        25 | 2015-05-16   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                      |       0.81 |         5 | 2016-09-06   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)   |       0.73 |        15 | 2018-01-07   |
| [torrelaysaregreat@gmail.com](https://metrics.torproject.org/rs.html#search/family:1323D34C2FA4AE0EC4EEA9853F3464693EF428E7)                   |       0.73 |        24 | 2018-08-28   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                      |       0.7  |         5 | 2017-10-24   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:04D9CEA8D778ABA130B014F758C2BCADD31DA05E)            |       0.62 |        28 | 2019-02-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)           |       0.57 |         3 | 2015-04-22   |
| [Peter Gerber &lt;tor@arbitrary.ch&gt;](https://metrics.torproject.org/rs.html#search/family:3F43D0584A2613C9DB631382FF486DC6B95EA1C8)         |       0.54 |         8 | 2019-01-20   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |            7.651 |     20.77 |       2.56 |       144 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)  |            2.39  |      8.17 |       0    |        32 | 2018-03-21   |
| [exitrelays@protonmail.com](https://metrics.torproject.org/rs.html#search/family:0828A52E57E4C426742B9264A210394202CD44D4)                                |            1.933 |      6.61 |       0    |        30 | 2020-07-08   |
| [kleinendorstwiebe AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:01C05513D12F63AE9E72588E8EAB459028C44689)                       |            1.775 |      6.06 |       0    |        27 | 2020-06-20   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            1.186 |      3.77 |       0.1  |        23 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.084 |      3.7  |       0    |        17 | 2016-12-23   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.868 |      0    |       1.41 |        14 | 2018-10-05   |
| [Digitalcourage Tor Team &lt;tor-abuse@digitalcourage.](https://metrics.torproject.org/rs.html#search/family:22296CB6AE56609A96F02FB843AB7B4B0A31CAF4)    |            0.842 |      2.87 |       0    |        17 | 2016-05-27   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)            |            0.721 |      0    |       1.17 |        25 | 2015-05-16   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.612 |      2    |       0.04 |        20 | 2013-06-11   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                 |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH     |            15.79 |      22.76 |      0.05 |       405 |
| OVH SAS                 |            15.79 |      15.38 |     20.25 |       548 |
| Online S.a.s.           |             7.42 |      10.67 |      2.09 |       235 |
| Joshua Peter McQuistan  |             7.15 |       1.75 |     20.77 |       138 |
| F3 Netze e.V.           |             2.39 |       0    |      8.17 |        32 |
| netcup GmbH             |             1.92 |       2.41 |      0.51 |       106 |
| myLoc managed IT AG     |             1.84 |       2.38 |      1.04 |        45 |
| Liteserver Holding B.V. |             1.84 |       0    |      6.28 |        32 |
| Zwiebelfreunde e.V.     |             1.31 |       0    |      4.5  |        22 |
| Contabo GmbH            |             1.23 |       1.82 |      0.14 |        87 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.3         |             60.7 |     70.85 |      55.77 |      3468 |
| 0.4.2         |             21   |     25.69 |      19.31 |      1415 |
| 0.3.5         |             12.1 |      1.69 |      16.74 |      1037 |
| 0.4.1         |              3.2 |      0.51 |       4.52 |       228 |
| 0.4.4         |              2.4 |      0.55 |       3.53 |       107 |
| 0.4.5         |              0.3 |      0.67 |       0.12 |        15 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|              3.6 |       4.64 |      1.19 |       243 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.6 |      93.1 |       92.4 |      5728 |
| BSD     |              7.1 |       6.8 |        7.3 |       458 |
| Windows |              0.1 |       0   |        0   |        42 |
| Darwin  |              0   |       0   |        0   |         7 |
| SunOS   |              0   |       0   |        0   |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|             35.7 |      30.51 |       29.85 |     49.05 |      1409 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     50.36 |            448 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1032 |
| None                                       |       424 |
| obfs3, obfs4                               |        74 |
| fte, obfs3, obfs4, scramblesuit            |        23 |
| meek                                       |         4 |
| obfs3, obfs4, scramblesuit                 |         4 |
| obfs2, obfs3, obfs4                        |         3 |
| fte, obfs3, obfs4, scramblesuit, websocket |         2 |
| obfs3                                      |         2 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3, obfs4                          |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek, meek                                 |         1 |
| meek, obfs3, obfs4                         |         1 |
| obfs3, scramblesuit                        |         1 |
| obfs4, scramblesuit                        |         1 |
| obfs4, websocket                           |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

