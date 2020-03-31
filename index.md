---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-03-31 16:00 UTC**

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
| [abuse-contact@to-surf-and-protect.net](endtoend-correlation-groups#abuse-contactto-surf-and-protectnet) | 0.88        | 10.05      | 136       | 5               | 2020-03-26     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)     | 0.03        | 0.02       | 2         | 2               | 2019-10-25     | 1                           |
| **Total**                                                                                                | **0.91**    | **10.07**  | **138**   |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                    |      9.92 |        69 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |      8.6  |        32 | 2018-03-21   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      8.28 |        18 | 2018-03-01   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      5.1  |        50 | 2016-08-22   |
| [loribthorpe@hotmail.com](https://metrics.torproject.org/rs.html#search/family:00BC71A338099F9A387C3BF314A5BD4FB48A6FB9)                                  |      4.55 |        63 | 2020-02-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      4.49 |        17 | 2016-12-23   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      3.75 |        19 | 2013-06-11   |
| [mleachman00@gmail.com](https://metrics.torproject.org/rs.html#search/family:008661B2709B32E339D0F94619A37CE77E9234D7)                                    |      2.14 |        39 | 2020-02-29   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:0C6842CCF836DE08EFEA0BD6C1471AE3463B9B71)                                    |      2.12 |        35 | 2019-04-05   |
| [thomaspli1@hotmail.com](https://metrics.torproject.org/rs.html#search/family:061182496BB51D14DC663EE57B6F1F60AF90F092)                                   |      2.07 |        76 | 2020-01-29   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |       1.52 |        14 | 2018-10-05   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                            |       1.46 |        18 | 2019-01-05   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                      |       1.01 |         8 | 2018-09-25   |
| [abuse@for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                                    |       0.97 |        10 | 2019-03-16   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                                 |       0.87 |         5 | 2016-09-06   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)              |       0.85 |        15 | 2018-01-07   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://metrics.torproject.org/rs.html#search/family:021047C51A57254D263DDB8B9277CA1C286D600E) |       0.75 |         9 | 2014-04-09   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:12B1A5769D38FF47CF68C2235E1BDA315DF400F2)                                     |       0.72 |        25 | 2018-08-28   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                                 |       0.71 |         5 | 2017-10-24   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:04D9CEA8D778ABA130B014F758C2BCADD31DA05E)                       |       0.7  |        28 | 2019-02-23   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                            |            3.779 |      9.92 |       1.46 |        87 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |            2.473 |      8.6  |       0    |        32 | 2018-03-21   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            2.44  |      8.28 |       0.09 |        21 | 2017-06-13   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            1.466 |      5.1  |       0    |        50 | 2016-08-22   |
| [loribthorpe@hotmail.com](https://metrics.torproject.org/rs.html#search/family:00BC71A338099F9A387C3BF314A5BD4FB48A6FB9)                                  |            1.309 |      4.55 |       0    |        63 | 2020-02-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.292 |      4.49 |       0    |        17 | 2016-12-23   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            1.106 |      3.75 |       0.04 |        20 | 2013-06-11   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.963 |      0    |       1.52 |        14 | 2018-10-05   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)              |            0.659 |      0.41 |       0.85 |        22 | 2018-01-07   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                      |            0.639 |      0    |       1.01 |         8 | 2018-09-25   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                        |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH            |            16.33 |      23.07 |      1.15 |       399 |
| OVH SAS                        |            13.44 |      14.78 |     12.83 |       693 |
| Online S.a.s.                  |             8.09 |      10.86 |      2.86 |       281 |
| Joshua Peter McQuistan         |             3.46 |       0.28 |     10.92 |       172 |
| netcup GmbH                    |             2.5  |       2.95 |      0.56 |       122 |
| F3 Netze e.V.                  |             2.47 |       0    |      8.6  |        32 |
| FranTech Solutions             |             2.4  |       1.23 |      5.38 |       264 |
| Foundation for Applied Privacy |             2.38 |       0    |      8.28 |        18 |
| myLoc managed IT AG            |             2.32 |       2.86 |      1.6  |        45 |
| Quintex Alliance Consulting    |             1.46 |       0    |      5.1  |        50 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.2         |             63.4 |     81.45 |      55.4  |      3865 |
| 0.3.5         |             17.5 |     10.69 |      20.55 |      1859 |
| 0.4.1         |              8.9 |      2.34 |      11.86 |       640 |
| 0.4.0         |              3.4 |      0.33 |       4.56 |       125 |
| 0.4.3         |              3.4 |      2.68 |       4.04 |       134 |
| 0.2.9         |              1.5 |      0.84 |       1.86 |       324 |
| 0.4.4         |              1.5 |      1.63 |       1.69 |        45 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             6.58 |       8.12 |      2.81 |       494 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.6 |      85.8 |       92.3 |      6369 |
| BSD     |              9.1 |      14   |        7.4 |       453 |
| Windows |              0.1 |       0.1 |        0   |        43 |
| SunOS   |              0   |       0   |        0.1 |         5 |
| Darwin  |              0   |       0   |        0   |         6 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            35.67 |       29.4 |       29.52 |     51.04 |      1435 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     52.18 |            453 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       855 |
| None                                       |       406 |
| obfs3, obfs4                               |        62 |
| fte, obfs3, obfs4, scramblesuit, websocket |        19 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         5 |
| obfs2, obfs3, obfs4                        |         4 |
| obfs3, obfs4, scramblesuit                 |         4 |
| obfs3                                      |         3 |
| fte, meek, obfs3, obfs4                    |         2 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek, meek                                 |         1 |
| meek, obfs3, obfs4                         |         1 |
| obfs2, obfs3                               |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs3, scramblesuit                        |         1 |
| obfs4, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

