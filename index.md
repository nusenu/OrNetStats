---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-07-02 19:00 UTC**

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

| Contact                                                                                                  | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:---------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [abuse-contact@to-surf-and-protect.net](endtoend-correlation-groups#abuse-contactto-surf-and-protectnet) | 1.95        | 22.68      | 140       | 5               | 2020-03-27     | 1                           |
| [tomas.vanagas@knf.vu.lt tor-relay.co](endtoend-correlation-groups#tomasvanagasknfvult-tor-relayco)      | 0.03        | 0.07       | 2         | 2               | 2020-04-28     | 1                           |
| **Total**                                                                                                | **1.98**    | **22.75**  | **142**   |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     23.05 |       116 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      6.09 |        18 | 2018-03-01   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |      6.03 |        30 | 2018-03-21   |
| [kleinendorstwiebe AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:01C05513D12F63AE9E72588E8EAB459028C44689)                       |      5.95 |        27 | 2020-06-20   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      5.48 |       100 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.9  |        17 | 2016-12-23   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      2.54 |        19 | 2013-06-11   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      1.79 |        13 | 2015-05-22   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      1.73 |        11 | 2017-12-05   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      1.71 |        15 | 2014-04-09   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                             |   Guard(%) |   #Relays | First Seen   |
|:-----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)           |       1.45 |        14 | 2018-10-05   |
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:02758CD398E3F842EF82478078AAAE0273770DB2)         |       1.25 |        21 | 2019-01-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE) |       1.03 |        23 | 2015-05-16   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)   |       0.9  |        15 | 2018-01-07   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                      |       0.84 |         5 | 2017-10-24   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:1323D34C2FA4AE0EC4EEA9853F3464693EF428E7)                          |       0.69 |        24 | 2018-08-28   |
| [63540827](https://metrics.torproject.org/rs.html#search/family:63540827C4832D214984EA47B7A68C593F9F862F)                                      |       0.69 |         2 | 2018-12-12   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)           |       0.68 |         3 | 2015-04-22   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:14E72D4DA10B66353E583F26EE04AC0D563EA7EF)            |       0.66 |        28 | 2019-02-23   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                      |       0.6  |         4 | 2018-08-17   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |            7.383 |     23.05 |       1.25 |       142 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            1.78  |      6.09 |       0.08 |        21 | 2017-06-13   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |            1.709 |      6.03 |       0    |        30 | 2018-03-21   |
| [kleinendorstwiebe AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:01C05513D12F63AE9E72588E8EAB459028C44689)                       |            1.688 |      5.95 |       0    |        27 | 2020-06-20   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            1.555 |      5.48 |       0    |       100 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.108 |      3.9  |       0    |        17 | 2016-12-23   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.86  |      0    |       1.45 |        14 | 2018-10-05   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.747 |      2.54 |       0.04 |        20 | 2013-06-11   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)              |            0.671 |      0.46 |       0.9  |        23 | 2018-01-07   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)            |            0.616 |      0    |       1.03 |        23 | 2015-05-16   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                        |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH            |            15.02 |      21.25 |      0.46 |       426 |
| OVH SAS                        |            13.65 |      17.7  |      8.64 |       516 |
| Joshua Peter McQuistan         |             7.39 |       1.15 |     23.05 |       142 |
| Online S.a.s.                  |             6.97 |      10.06 |      2.79 |       243 |
| netcup GmbH                    |             2.3  |       2.63 |      0.64 |       123 |
| myLoc managed IT AG            |             1.76 |       2.26 |      1.19 |        46 |
| Foundation for Applied Privacy |             1.72 |       0    |      6.09 |        18 |
| Liteserver Holding B.V.        |             1.71 |       0    |      5.99 |        33 |
| F3 Netze e.V.                  |             1.7  |       0    |      6.03 |        30 |
| Quintex Alliance Consulting    |             1.55 |       0    |      5.48 |       100 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.3         |             48.9 |     48.21 |      48.22 |      2973 |
| 0.4.2         |             30.2 |     41.64 |      25.69 |      1906 |
| 0.3.5         |             12.7 |      2.61 |      17.25 |      1051 |
| 0.4.1         |              4.4 |      1.05 |       6.28 |       277 |
| 0.4.4         |              1.8 |      0.98 |       2.42 |        78 |
| 0.4.5         |              1.7 |      5.48 |       0.11 |       115 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             6.18 |       6.39 |      6.54 |       392 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.9 |      89.9 |       92.1 |      5800 |
| BSD     |              7.8 |       9.9 |        7.6 |       463 |
| Windows |              0.1 |       0   |        0   |        45 |
| SunOS   |              0   |       0   |        0.1 |         4 |
| Darwin  |              0   |       0   |        0   |         7 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            37.22 |      31.41 |       27.73 |     56.54 |      1502 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     57.98 |            519 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       774 |
| None                                       |       476 |
| obfs3, obfs4                               |        75 |
| fte, obfs3, obfs4, scramblesuit            |        25 |
| meek                                       |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| fte, obfs3, obfs4, scramblesuit, websocket |         3 |
| obfs2, obfs3, obfs4                        |         3 |
| obfs3                                      |         2 |
| fte, obfs3, obfs4                          |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek, meek                                 |         1 |
| meek, obfs3, obfs4                         |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs3, scramblesuit                        |         1 |
| obfs4, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

