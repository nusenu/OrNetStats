---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-07-29 17:00 UTC**

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

| Contact                                                                                              | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-----------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com) | 0.01        | 0.02       | 2         | 2               | 2019-10-25     | 1                           |
| **Total**                                                                                            | **0.01**    | **0.02**   | **2**     |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     20.1  |       113 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)  |      7.68 |        32 | 2018-03-21   |
| [exitrelays@protonmail.com](https://metrics.torproject.org/rs.html#search/family:0828A52E57E4C426742B9264A210394202CD44D4)                                |      6.5  |        30 | 2020-07-08   |
| [kleinendorstwiebe AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:01C05513D12F63AE9E72588E8EAB459028C44689)                       |      5.71 |        27 | 2020-06-20   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      3.77 |        18 | 2018-03-01   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.56 |        17 | 2016-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      3.43 |        98 | 2016-08-22   |
| [Digitalcourage Tor Team &lt;tor-abuse@digitalcourage.](https://metrics.torproject.org/rs.html#search/family:22296CB6AE56609A96F02FB843AB7B4B0A31CAF4)    |      2.73 |        17 | 2016-05-27   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      2.01 |        19 | 2013-06-11   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      1.49 |        15 | 2014-04-09   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                             |   Guard(%) |   #Relays | First Seen   |
|:-----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)         |       2.19 |        27 | 2019-01-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)           |       1.42 |        14 | 2018-10-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE) |       1.19 |        25 | 2015-05-16   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                      |       0.79 |         5 | 2016-09-06   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)   |       0.77 |        15 | 2018-01-07   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                      |       0.73 |         5 | 2017-10-24   |
| [torrelaysaregreat@gmail.com](https://metrics.torproject.org/rs.html#search/family:1323D34C2FA4AE0EC4EEA9853F3464693EF428E7)                   |       0.73 |        23 | 2018-08-28   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:04D9CEA8D778ABA130B014F758C2BCADD31DA05E)            |       0.64 |        28 | 2019-02-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)           |       0.59 |         3 | 2015-04-22   |
| [Peter Gerber &lt;tor@arbitrary.ch&gt;](https://metrics.torproject.org/rs.html#search/family:3F43D0584A2613C9DB631382FF486DC6B95EA1C8)         |       0.56 |         8 | 2019-01-20   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                       |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:---------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                   |            7.572 |     20.1  |       2.19 |       144 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737) |            2.305 |      7.68 |       0    |        32 | 2018-03-21   |
| [exitrelays@protonmail.com](https://metrics.torproject.org/rs.html#search/family:0828A52E57E4C426742B9264A210394202CD44D4)                               |            1.95  |      6.5  |       0    |        30 | 2020-07-08   |
| [kleinendorstwiebe AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:01C05513D12F63AE9E72588E8EAB459028C44689)                      |            1.713 |      5.71 |       0    |        27 | 2020-06-20   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)       |            1.198 |      3.77 |       0.11 |        22 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)   |            1.069 |      3.56 |       0    |        17 | 2016-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)   |            1.03  |      3.43 |       0    |        98 | 2016-08-22   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                     |            0.859 |      0    |       1.42 |        14 | 2018-10-05   |
| [Digitalcourage Tor Team &lt;tor-abuse@digitalcourage.](https://metrics.torproject.org/rs.html#search/family:22296CB6AE56609A96F02FB843AB7B4B0A31CAF4)   |            0.82  |      2.73 |       0    |        17 | 2016-05-27   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)           |            0.721 |      0    |       1.19 |        25 | 2015-05-16   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                 |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                 |            15.63 |      15.43 |     19.66 |       548 |
| Hetzner Online GmbH     |            15.35 |      22.59 |      0.06 |       404 |
| Online S.a.s.           |             7.41 |      10.87 |      2.02 |       236 |
| Joshua Peter McQuistan  |             7.1  |       1.42 |     20.1  |       138 |
| F3 Netze e.V.           |             2.3  |       0    |      7.68 |        32 |
| netcup GmbH             |             2.06 |       2.51 |      0.57 |       109 |
| myLoc managed IT AG     |             1.79 |       2.33 |      1.06 |        45 |
| Liteserver Holding B.V. |             1.77 |       0    |      5.91 |        32 |
| Zwiebelfreunde e.V.     |             1.28 |       0    |      4.29 |        22 |
| 1&amp;1 Internet SE     |             1.23 |       1.49 |      0.12 |        39 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.3         |             60.2 |     68.66 |      55.39 |      3463 |
| 0.4.2         |             21   |     24.66 |      19.78 |      1422 |
| 0.3.5         |             11.8 |      1.61 |      16.75 |      1031 |
| 0.4.1         |              3.2 |      0.49 |       4.45 |       229 |
| 0.4.4         |              2.3 |      0.52 |       3.47 |       105 |
| 0.4.5         |              1.3 |      4.03 |       0.13 |       112 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             4.55 |       4.58 |      4.53 |       341 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.7 |      93.2 |       92.4 |      5831 |
| BSD     |              7   |       6.6 |        7.4 |       456 |
| Windows |              0.1 |       0   |        0   |        40 |
| SunOS   |              0   |       0   |        0   |         4 |
| Darwin  |              0   |       0   |        0   |         7 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            36.43 |      30.74 |       29.64 |        51 |      1511 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     52.22 |            543 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1025 |
| None                                       |       421 |
| obfs3, obfs4                               |        75 |
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

