---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-12-31 10:00 UTC**

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
| [abuse-node49 AT posteo DOT de](endtoend-correlation-groups#abuse-node49-at-posteo-dot-de)                                     | 0.37        | 0.57       | 14        | 6               | 2019-12-15     | 2                           |
| [bobs.house AT mail.ru 36j52chsdz962ivcpN1xfPXkJz](endtoend-correlation-groups#bobshouse-at-mailru-36j52chsdz962ivcpn1xfpxkjz) | 0.21        | 0.3        | 7         | 2               | 2019-11-13     | 1                           |
| [see https://www.artikel5ev.de/torcontact/](endtoend-correlation-groups#see-httpswwwartikel5evdetorcontact)                    | 0.13        | 0.31       | 11        | 6               | 2019-12-29     | 1                           |
| [runtime-error at riseup dot net](endtoend-correlation-groups#runtime-erroratriseupdotnet)                                     | 0.09        | 0.18       | 3         | 3               | 2019-07-19     | 1                           |
| [Steven S &lt;katsalmovies@gmail.com&gt;](endtoend-correlation-groups#steven-s-katsalmoviesgmailcom)                           | 0.03        | 0.19       | 3         | 2               | 2019-10-04     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                           | 0.02        | 0.04       | 2         | 2               | 2019-10-25     | 1                           |
| [report at dustin dot in tor-relay.co](endtoend-correlation-groups#reportatdustindotin-tor-relayco)                            | 0.01        | 0.08       | 2         | 2               | 2019-12-01     | 1                           |
| **Total**                                                                                                                      | **0.86**    | **1.67**   | **42**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                            |     15.42 |        50 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      8.72 |        15 | 2018-03-23   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      5.22 |        17 | 2016-12-23   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |      5.08 |        16 | 2018-03-21   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      4.49 |        50 | 2016-08-22   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |      3.01 |        54 | 2019-04-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      2.71 |        13 | 2015-05-22   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      2.69 |        12 | 2013-06-11   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      2.47 |        15 | 2014-04-09   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      1.81 |        12 | 2017-12-05   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |       1.88 |        14 | 2018-10-05   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                            |       1.57 |        18 | 2019-01-05   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88)    |       1.07 |         8 | 2016-01-03   |
| [abuse@for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                                    |       0.96 |        10 | 2019-03-16   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                      |       0.93 |         6 | 2018-09-25   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                                 |       0.82 |         5 | 2017-10-24   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:1A7A2516A961F2838F7F94786A8811BE82F9CFFE)                                     |       0.81 |        21 | 2018-08-28   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                                 |       0.78 |         5 | 2016-09-06   |
| [63540827](https://metrics.torproject.org/rs.html#search/family:63540827C4832D214984EA47B7A68C593F9F862F)                                                 |       0.72 |         2 | 2018-12-12   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://metrics.torproject.org/rs.html#search/family:021047C51A57254D263DDB8B9277CA1C286D600E) |       0.65 |        10 | 2014-04-09   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                            |            5.05  |     15.42 |       1.57 |        68 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            2.431 |      8.72 |       0.24 |        19 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.358 |      5.22 |       0    |        17 | 2016-12-23   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |            1.324 |      5.08 |       0    |        16 | 2018-03-21   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            1.238 |      0    |       1.88 |        14 | 2018-10-05   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            1.17  |      4.49 |       0    |        50 | 2016-08-22   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |            0.808 |      3.01 |       0.03 |        55 | 2019-04-05   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.729 |      2.69 |       0.04 |        13 | 2013-06-11   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |            0.707 |      2.71 |       0    |        13 | 2015-05-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88)    |            0.706 |      0    |       1.07 |         8 | 2016-01-03   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                        |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH            |            14.21 |      19.62 |      0.29 |       383 |
| OVH SAS                        |            12.13 |      15.16 |      6.45 |       504 |
| Online S.a.s.                  |             9.22 |      12.4  |      3.3  |       279 |
| Joshua Peter McQuistan         |             4.31 |       0.08 |     15.42 |        53 |
| myLoc managed IT AG            |             2.73 |       3.5  |      1.65 |        45 |
| netcup GmbH                    |             2.54 |       3.2  |      0.18 |       124 |
| Foundation for Applied Privacy |             2.35 |       0.12 |      8.72 |        16 |
| FranTech Solutions             |             2.07 |       1.1  |      4.89 |        87 |
| 1&amp;1 Internet SE            |             1.41 |       1.8  |      0.11 |        40 |
| SURFnet bv                     |             1.37 |       0.36 |      2.47 |        24 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.1         |             33.8 |     41.87 |      31.85 |      1922 |
| 0.4.2         |             30   |     39.3  |      26.55 |      1627 |
| 0.3.5         |             19.8 |      8.42 |      23.21 |      1530 |
| 0.4.0         |             10.1 |      7.77 |      11.16 |       438 |
| 0.2.9         |              4.1 |      1.24 |       4.86 |       591 |
| 0.4.3         |              1.8 |      1.37 |       2.34 |        41 |
| 0.2.4         |              0   |      0    |       0    |        15 |
| 0.2.5         |              0   |      0    |       0    |        13 |
| 0.2.6         |              0   |      0    |       0    |         2 |
| 0.2.7         |              0   |      0    |       0    |         4 |
| 0.2.8         |              0   |      0    |       0    |         1 |
| 0.3.0         |              0   |      0    |       0    |         1 |
| 0.3.1         |              0   |      0    |       0    |         3 |
| 0.3.2         |              0   |      0    |       0    |        27 |
| 0.3.3         |              0   |      0    |       0    |         8 |
| 0.3.4         |              0   |      0    |       0    |        53 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|                0 |          0 |         0 |       127 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             89.9 |      84.9 |       91.1 |      5701 |
| BSD     |              9.8 |      14.9 |        8.6 |       460 |
| Windows |              0.1 |       0   |        0   |        43 |
| Darwin  |              0   |       0   |        0   |         8 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            31.65 |       30.1 |       27.87 |     39.23 |      1212 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|      40.3 |            316 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       762 |
| None                                       |       428 |
| obfs3, obfs4                               |        58 |
| fte, obfs3, obfs4, scramblesuit, websocket |        20 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| meek                                       |         5 |
| obfs2, obfs3, obfs4                        |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| obfs3                                      |         3 |
| fte, meek, obfs3, obfs4                    |         2 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek, meek                                 |         1 |
| obfs3, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

