---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-07-19 06:00 UTC**

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
| [abuse@to-surf-and-protect.net](endtoend-correlation-groups#abuseto-surf-and-protectnet)                  | 1.67        | 12.1       | 61        | 6               | 2019-06-24     | 1                           |
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain) | 0.15        | 0.02       | 7         | 7               | 2019-06-23     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)      | 0.01        | 0.08       | 3         | 2               | 2016-08-28     | 1                           |
| **Total**                                                                                                 | **1.83**    | **12.20**  | **71**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                            |     12.45 |        42 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      8.53 |        50 | 2016-08-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      8.17 |        12 | 2018-03-23   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      6.72 |        17 | 2016-12-23   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |      4.95 |        55 | 2019-04-05   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      3.86 |        13 | 2013-06-11   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      2.61 |        13 | 2015-05-22   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:6BCB964AB74E23F8986BDA905697D3A6BE08AF28)                        |      2.49 |         8 | 2018-03-21   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      2.19 |        15 | 2014-04-09   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      1.88 |        12 | 2017-12-05   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                         |       1.54 |        16 | 2019-01-05   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                   |       0.78 |         6 | 2018-09-25   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |       0.75 |         4 | 2018-08-17   |
| [abuse AT for-privacy.net](https://metrics.torproject.org/rs.html#search/family:05250BA7E128350D14ED9A712639AC2EFCFF618B)                              |       0.74 |         8 | 2019-04-15   |
| [jwbecher@drazisil.com](https://metrics.torproject.org/rs.html#search/family:03310DA245BD3578412B453FC5A5A8538030671E)                                 |       0.73 |         8 | 2018-05-08   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.66 |         8 | 2016-01-03   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.66 |         3 | 2015-04-22   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:375BBF23B8214FD3F375E98ABC0FAE2620E30924)                                  |       0.59 |        21 | 2018-08-28   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:3B4C5729F829CA2E895B81AF834A63DB336D0FFE)           |       0.56 |        11 | 2018-01-07   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.53 |         5 | 2017-10-24   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                            |            3.964 |     12.45 |       1.54 |        58 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            2.165 |      8.17 |       0.26 |        19 | 2017-06-13   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            2.02  |      8.53 |       0    |        50 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.59  |      6.72 |       0    |        17 | 2016-12-23   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |            1.187 |      4.95 |       0    |        56 | 2019-04-05   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.938 |      3.86 |       0.03 |        14 | 2013-06-11   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.704 |      0    |       0.52 |         8 | 2018-10-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |            0.618 |      2.61 |       0    |        13 | 2015-05-22   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:6BCB964AB74E23F8986BDA905697D3A6BE08AF28)                        |            0.589 |      2.49 |       0    |         8 | 2018-03-21   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                                 |            0.552 |      0    |       0.75 |         5 | 2016-09-06   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH                                              |            15.85 |      19.31 |      0.23 |       419 |
| OVH SAS                                                          |            15.57 |      19.77 |      8.97 |       609 |
| Online S.a.s.                                                    |             9.47 |      12.52 |      3.67 |       291 |
| Joshua Peter McQuistan                                           |             3.13 |       0.29 |     12.45 |        46 |
| netcup GmbH                                                      |             2.59 |       3.34 |      0.11 |        89 |
| Iomart Cloud Services Limited                                    |             2.34 |       3.35 |      0    |        21 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             2.09 |       0.15 |      8.17 |        17 |
| Quintex Alliance Consulting                                      |             2.02 |       0    |      8.53 |        50 |
| myLoc managed IT AG                                              |             1.49 |       2.1  |      0.28 |        36 |
| 1&amp;1 Internet SE                                              |             1.4  |       1.94 |      0    |        32 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.5         |             40   |     40.25 |      39.47 |      2386 |
| 0.4.0         |             33.1 |     50.42 |      28.66 |      1687 |
| 0.3.4         |             11.2 |      3.49 |      14.77 |       558 |
| 0.2.9         |              8   |      2.92 |       8.99 |       887 |
| 0.4.1         |              2.2 |      0.32 |       3.09 |        87 |
| 0.3.2         |              1.8 |      1.29 |       1.97 |       178 |
| 0.3.3         |              1.2 |      0.54 |       1.44 |       135 |
| 0.4.2         |              0.9 |      0.3  |       0.71 |        29 |
| 0.3.1         |              0.4 |      0.11 |       0.55 |        53 |
| 0.2.4         |              0.2 |      0.02 |       0.04 |       106 |
| 0.2.5         |              0.2 |      0.2  |       0.17 |       109 |
| 0.2.6         |              0   |      0    |       0    |        24 |
| 0.2.7         |              0   |      0    |       0.03 |        63 |
| 0.2.8         |              0   |      0    |       0.01 |        13 |
| 0.3.0         |              0   |      0    |       0.07 |        50 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|              4.2 |       4.33 |      2.18 |       731 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.2 |      83.4 |       93.6 |      5805 |
| BSD     |              8.4 |      16.4 |        6.1 |       439 |
| Windows |              0.1 |       0   |        0   |        69 |
| Darwin  |              0   |       0   |        0.1 |        12 |
| SunOS   |              0   |       0   |        0   |         4 |
| other   |              0   |       0   |        0   |         1 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            28.36 |      23.56 |        24.1 |     42.96 |      1080 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     44.13 |            303 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       509 |
| None                                       |       421 |
| obfs3, obfs4                               |        69 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| obfs2, obfs3, obfs4                        |         6 |
| obfs3                                      |         6 |
| meek                                       |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| fte, meek, obfs3, obfs4                    |         2 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| meek, meek                                 |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs3, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

