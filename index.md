---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-11-30 07:00 UTC**

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
| [bobs.house AT mail.ru 36j52chsdz962ivcpN1xfPXkJz](endtoend-correlation-groups#bobshouse-at-mailru-36j52chsdz962ivcpn1xfpxkjz) | 0.09        | 0.35       | 4         | 2               | 2019-11-13     | 1                           |
| [runtime-error at riseup dot net](endtoend-correlation-groups#runtime-erroratriseupdotnet)                                     | 0.07        | 0.21       | 3         | 3               | 2019-07-19     | 1                           |
| [Steven S &lt;katsalmovies@gmail.com&gt;](endtoend-correlation-groups#steven-s-katsalmoviesgmailcom)                           | 0.04        | 0.19       | 3         | 2               | 2019-10-04     | 1                           |
| **Total**                                                                                                                      | **0.20**    | **0.75**   | **10**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                            |     16.76 |        50 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      7.52 |        12 | 2018-03-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      5.85 |        50 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      5.5  |        17 | 2016-12-23   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:6BCB964AB74E23F8986BDA905697D3A6BE08AF28)                        |      3.86 |         8 | 2018-03-21   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      3.75 |        13 | 2013-06-11   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |      3.37 |        55 | 2019-04-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      2.45 |        13 | 2015-05-22   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      2.41 |        15 | 2014-04-09   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:2CAEC55A7854FE3CB37BE80328086FDF89E082C4)      |      1.6  |         5 | 2016-01-22   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |       1.97 |        14 | 2018-10-05   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                         |       1.69 |        17 | 2019-01-05   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                   |       0.94 |         6 | 2018-09-25   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.92 |         7 | 2016-01-03   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |       0.86 |         5 | 2016-09-06   |
| [abuse AT for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                              |       0.83 |        10 | 2019-03-16   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:1A7A2516A961F2838F7F94786A8811BE82F9CFFE)                                  |       0.72 |        21 | 2018-08-28   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.67 |         5 | 2017-10-24   |
| [63540827](https://metrics.torproject.org/rs.html#search/family:63540827C4832D214984EA47B7A68C593F9F862F)                                              |       0.66 |         2 | 2018-12-12   |
| [email:tor appliedprivacy.net twitter:applied priv](https://metrics.torproject.org/rs.html#search/family:113143469021882C3A4B82F084F8125B08EE471E)     |       0.65 |         7 | 2017-06-13   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                            |            5.361 |     16.76 |       1.69 |        67 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            2.341 |      7.52 |       0.65 |        19 | 2017-06-13   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            1.495 |      5.85 |       0    |        50 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.403 |      5.5  |       0    |        17 | 2016-12-23   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            1.261 |      0    |       1.97 |        14 | 2018-10-05   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:6BCB964AB74E23F8986BDA905697D3A6BE08AF28)                        |            0.987 |      3.86 |       0    |         8 | 2018-03-21   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.984 |      3.75 |       0.04 |        14 | 2013-06-11   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |            0.876 |      3.37 |       0.02 |        56 | 2019-04-05   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                      |            0.733 |      0    |       0.94 |         7 | 2018-09-25   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88)    |            0.665 |      0    |       0.92 |         8 | 2016-01-03   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                        |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH            |            15.79 |      21.18 |      0.07 |       402 |
| OVH SAS                        |            12.46 |      15.76 |      7.01 |       535 |
| Online S.a.s.                  |             8.47 |      11.46 |      2.91 |       261 |
| Joshua Peter McQuistan         |             4.69 |       0.35 |     16.76 |        54 |
| myLoc managed IT AG            |             2.5  |       3.42 |      1.01 |        47 |
| netcup GmbH                    |             2.29 |       2.79 |      0.12 |       113 |
| Foundation for Applied Privacy |             2.26 |       0.53 |      7.52 |        16 |
| FranTech Solutions             |             2.1  |       0.87 |      4.95 |        77 |
| Iomart Cloud Services Limited  |             1.63 |       2.55 |      0    |        20 |
| Quintex Alliance Consulting    |             1.49 |       0    |      5.85 |        50 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.1         |             57   |     75.6  |      51.11 |      3116 |
| 0.3.5         |             19.6 |      7.89 |      23.51 |      1490 |
| 0.4.0         |             11.4 |      7.34 |      13.12 |       525 |
| 0.4.2         |              5.5 |      5.46 |       6.16 |       143 |
| 0.2.9         |              5.1 |      2.62 |       5.25 |       634 |
| 0.3.4         |              0.5 |      0.15 |       0.71 |        56 |
| 0.3.2         |              0.2 |      0.37 |       0.04 |        24 |
| 0.2.4         |              0   |      0.01 |       0    |        17 |
| 0.2.5         |              0   |      0.03 |       0    |        12 |
| 0.2.6         |              0   |      0    |       0    |         1 |
| 0.2.7         |              0   |      0.32 |       0    |         1 |
| 0.2.8         |              0   |      0    |       0    |         1 |
| 0.3.0         |              0   |      0    |       0    |        12 |
| 0.3.1         |              0   |      0    |       0    |         4 |
| 0.3.3         |              0   |      0.14 |       0    |         7 |
| 0.3.6         |              0   |      0    |       0    |         1 |
| 0.4.3         |              0   |      0    |       0.08 |        13 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             1.08 |       0.76 |      1.04 |       136 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.6 |      86.1 |       91.9 |      5517 |
| BSD     |              9.1 |      13.7 |        7.7 |       448 |
| Windows |              0.1 |       0   |        0.1 |        41 |
| SunOS   |              0   |       0   |        0.1 |         5 |
| Darwin  |              0   |       0   |        0   |         7 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            30.24 |      28.07 |       26.76 |     38.48 |      1151 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     39.41 |            307 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       703 |
| None                                       |       410 |
| obfs3, obfs4                               |        72 |
| fte, obfs3, obfs4, scramblesuit, websocket |        20 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| obfs2, obfs3, obfs4                        |         6 |
| meek                                       |         5 |
| obfs3, obfs4, scramblesuit                 |         5 |
| fte, meek, obfs3, obfs4                    |         2 |
| obfs3                                      |         2 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek, meek                                 |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs3, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

