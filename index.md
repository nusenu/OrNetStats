---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-04-19 09:00 UTC**

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
| [abuse-contact@to-surf-and-protect.net](endtoend-correlation-groups#abuse-contactto-surf-and-protectnet) | 1.11        | 16.22      | 125       | 3               | 2020-03-26     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)     | 0.01        | 0.02       | 2         | 2               | 2019-10-25     | 1                           |
| **Total**                                                                                                | **1.12**    | **16.24**  | **127**   |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:05F5BB75DA007361CE03770393033D4D52836D8A)                    |     17.28 |       106 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |      9.09 |        32 | 2018-03-21   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      6.59 |        18 | 2018-03-01   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      4.13 |        17 | 2016-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      3.38 |        50 | 2016-08-22   |
| [loribthorpe@hotmail.com](https://metrics.torproject.org/rs.html#search/family:00BC71A338099F9A387C3BF314A5BD4FB48A6FB9)                                  |      3.36 |        62 | 2020-02-05   |
| [abusetor1234@protonmail.com](https://metrics.torproject.org/rs.html#search/family:072DBE9FDC36A1CF63EABE3A27C196AEED97386A)                              |      2.68 |        48 | 2020-03-21   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      2.57 |        19 | 2013-06-11   |
| [mleachman00@gmail.com](https://metrics.torproject.org/rs.html#search/family:008661B2709B32E339D0F94619A37CE77E9234D7)                                    |      1.93 |        39 | 2020-02-29   |
| [johntor336@hotmail.com](https://metrics.torproject.org/rs.html#search/family:015958818FA01CF937EA3F66FCB813D8B3840EDB)                                   |      1.87 |        53 | 2020-04-13   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                            |       1.75 |        30 | 2019-01-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |       1.51 |        14 | 2018-10-05   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                      |       0.97 |         8 | 2018-09-25   |
| [abuse@for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                                    |       0.87 |        10 | 2019-03-16   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)              |       0.79 |        15 | 2018-01-07   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:12B1A5769D38FF47CF68C2235E1BDA315DF400F2)                                     |       0.69 |        25 | 2018-08-28   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                                 |       0.66 |         5 | 2016-09-06   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                                 |       0.65 |         5 | 2017-10-24   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://metrics.torproject.org/rs.html#search/family:13557448AD1632BF080757C2FF7769BB23DF1DF3) |       0.63 |         7 | 2014-04-09   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88)    |       0.63 |         8 | 2016-01-03   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0548884511A51EEA08CD464B016E4F93E9F81072)                    |            6.415 |     17.28 |       1.75 |       150 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |            2.711 |      9.09 |       0    |        32 | 2018-03-21   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            2.022 |      6.59 |       0.09 |        21 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.232 |      4.13 |       0    |        17 | 2016-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            1.009 |      3.38 |       0    |        50 | 2016-08-22   |
| [loribthorpe@hotmail.com](https://metrics.torproject.org/rs.html#search/family:00BC71A338099F9A387C3BF314A5BD4FB48A6FB9)                                  |            1.004 |      3.36 |       0    |        62 | 2020-02-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.906 |      0    |       1.51 |        14 | 2018-10-05   |
| [abusetor1234@protonmail.com](https://metrics.torproject.org/rs.html#search/family:072DBE9FDC36A1CF63EABE3A27C196AEED97386A)                              |            0.801 |      2.68 |       0    |        48 | 2020-03-21   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.79  |      2.57 |       0.04 |        20 | 2013-06-11   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                      |            0.581 |      0    |       0.97 |         8 | 2018-09-25   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                        |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH            |            16.01 |      22.66 |      0.96 |       405 |
| OVH SAS                        |            13.27 |      14.74 |     13.38 |       701 |
| Online S.a.s.                  |             8.01 |      11.22 |      3.22 |       280 |
| Joshua Peter McQuistan         |             7.01 |       0.9  |     17.4  |       200 |
| F3 Netze e.V.                  |             2.71 |       0    |      9.09 |        32 |
| netcup GmbH                    |             2.66 |       3.26 |      0.51 |       125 |
| myLoc managed IT AG            |             2.08 |       2.63 |      1.54 |        46 |
| Foundation for Applied Privacy |             1.96 |       0    |      6.59 |        18 |
| FranTech Solutions             |             1.72 |       0.78 |      3.9  |       133 |
| NForce Entertainment B.V.      |             1.28 |       0.46 |      3.08 |        25 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.2         |             68   |     86.38 |      59.47 |      4120 |
| 0.3.5         |             15.1 |      7.05 |      18.52 |      1528 |
| 0.4.1         |              7.5 |      1.96 |      10.29 |       542 |
| 0.4.3         |              3.2 |      2.28 |       3.82 |       144 |
| 0.4.0         |              2.8 |      0.28 |       4.3  |       105 |
| 0.2.9         |              1.8 |      1.02 |       1.88 |       318 |
| 0.4.4         |              1.3 |      1    |       1.68 |        45 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.99 |       7.87 |      2.31 |       468 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.6 |      89.3 |       92.4 |      6257 |
| BSD     |              8.1 |      10.6 |        7.3 |       454 |
| Windows |              0.1 |       0   |        0   |        44 |
| SunOS   |              0   |       0   |        0   |         4 |
| Darwin  |              0   |       0   |        0   |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            37.01 |      30.32 |       31.46 |     51.42 |      1464 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     52.33 |            416 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       777 |
| None                                       |       399 |
| obfs3, obfs4                               |        65 |
| fte, obfs3, obfs4, scramblesuit, websocket |        19 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         5 |
| obfs2, obfs3, obfs4                        |         4 |
| obfs3, obfs4, scramblesuit                 |         4 |
| obfs3                                      |         2 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
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

