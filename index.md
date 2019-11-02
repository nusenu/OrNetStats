---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-11-02 08:00 UTC**

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
| [runtime-error at riseup dot net](endtoend-correlation-groups#runtime-erroratriseupdotnet)                                     | 0.05        | 0.14       | 3         | 3               | 2019-07-19     | 1                           |
| [Steven S &lt;katsalmovies@gmail.com&gt;](endtoend-correlation-groups#steven-s-katsalmoviesgmailcom)                           | 0.05        | 0.21       | 3         | 2               | 2019-10-04     | 1                           |
| [bobs.house AT mail.ru 36j52chsdz962ivcpN1xfPXkJz](endtoend-correlation-groups#bobshouse-at-mailru-36j52chsdz962ivcpn1xfpxkjz) | 0.01        | 0.22       | 3         | 2               | 2019-09-17     | 1                           |
| **Total**                                                                                                                      | **0.11**    | **0.57**   | **9**     |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                            |     13.95 |        50 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      7.95 |        50 | 2016-08-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      7.64 |        12 | 2018-03-23   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |      5.68 |        54 | 2019-04-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      5.63 |        17 | 2016-12-23   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      4.43 |        13 | 2013-06-11   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:6BCB964AB74E23F8986BDA905697D3A6BE08AF28)                        |      3.32 |         8 | 2018-03-21   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      2.46 |        15 | 2014-04-09   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      2.3  |        13 | 2015-05-22   |
| [D3803AA31B027F22D58904C1B2F867E0FB438BC9 contactt](https://metrics.torproject.org/rs.html#search/family:1297DB025DDDC46ADCB9D232E15B02E65272FE72)        |      1.91 |         4 | 2019-08-11   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |       1.94 |        14 | 2018-10-05   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                         |       1.44 |        15 | 2019-01-05   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       1.03 |         8 | 2016-01-03   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                   |       0.94 |         7 | 2018-09-25   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |       0.84 |         5 | 2016-09-06   |
| [abuse AT for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                              |       0.68 |         8 | 2019-04-28   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.67 |         5 | 2017-10-24   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.65 |         3 | 2015-04-22   |
| [63540827](https://metrics.torproject.org/rs.html#search/family:63540827C4832D214984EA47B7A68C593F9F862F)                                              |       0.57 |         2 | 2018-12-12   |
| [email:tor appliedprivacy.net twitter:applied priv](https://metrics.torproject.org/rs.html#search/family:113143469021882C3A4B82F084F8125B08EE471E)     |       0.55 |         7 | 2017-06-13   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                            |            4.515 |     13.95 |       1.44 |        67 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            2.306 |      7.64 |       0.55 |        19 | 2017-06-13   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            2.03  |      7.95 |       0    |        50 | 2016-08-22   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |            1.466 |      5.68 |       0.02 |        55 | 2019-04-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.438 |      5.63 |       0    |        17 | 2016-12-23   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            1.251 |      0    |       1.94 |        14 | 2018-10-05   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            1.162 |      4.43 |       0.04 |        14 | 2013-06-11   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:6BCB964AB74E23F8986BDA905697D3A6BE08AF28)                        |            0.849 |      3.32 |       0    |         8 | 2018-03-21   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88)    |            0.666 |      0    |       1.03 |         8 | 2016-01-03   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |            0.629 |      2.46 |       0    |        15 | 2014-04-09   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                        |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH            |            14.96 |      19.66 |      0.1  |       394 |
| OVH SAS                        |            11.8  |      15.57 |      4.67 |       515 |
| Online S.a.s.                  |             8.12 |      10.94 |      2.87 |       273 |
| Joshua Peter McQuistan         |             3.82 |       0.41 |     13.95 |        54 |
| Choopa, LLC                    |             3.61 |       5.27 |      0    |       241 |
| myLoc managed IT AG            |             2.33 |       3.01 |      0.85 |        45 |
| Foundation for Applied Privacy |             2.22 |       0.43 |      7.64 |        16 |
| Quintex Alliance Consulting    |             2.03 |       0    |      7.95 |        50 |
| FranTech Solutions             |             2    |       0.73 |      5.94 |        72 |
| netcup GmbH                    |             1.91 |       2.61 |      0.11 |        95 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.1         |             51.6 |     71.12 |      44.93 |      2732 |
| 0.3.5         |             24.5 |     10.95 |      28.55 |      1752 |
| 0.4.0         |             13.2 |      9.36 |      15.08 |       659 |
| 0.2.9         |              5   |      2.72 |       5.37 |       670 |
| 0.4.2         |              4.7 |      5.34 |       5.1  |       121 |
| 0.3.4         |              0.6 |      0.14 |       0.82 |        69 |
| 0.4.3         |              0.1 |      0.34 |       0.1  |         9 |
| 0.2.4         |              0   |      0    |       0    |        15 |
| 0.2.5         |              0   |      0    |       0    |         9 |
| 0.2.8         |              0   |      0    |       0    |         1 |
| 0.3.0         |              0   |      0    |       0    |        12 |
| 0.3.1         |              0   |      0    |       0    |         4 |
| 0.3.2         |              0   |      0    |       0.01 |        14 |
| 0.3.3         |              0   |      0    |       0    |         8 |
| 0.3.6         |              0   |      0    |       0    |         1 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             0.71 |       0.84 |      0.14 |       133 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             89.8 |      83.4 |       91.6 |      5545 |
| BSD     |              9.9 |      16.4 |        8.1 |       436 |
| Windows |              0.1 |       0   |        0.1 |        38 |
| Darwin  |              0   |       0   |        0   |         7 |
| SunOS   |              0   |       0   |        0.1 |         6 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            30.51 |      27.03 |       26.01 |     42.16 |      1109 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     43.22 |            295 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       673 |
| None                                       |       401 |
| obfs3, obfs4                               |        84 |
| fte, obfs3, obfs4, scramblesuit, websocket |        20 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| meek                                       |         5 |
| obfs2, obfs3, obfs4                        |         5 |
| obfs3, obfs4, scramblesuit                 |         5 |
| fte, meek, obfs3, obfs4                    |         2 |
| obfs3                                      |         2 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek, meek                                 |         1 |
| obfs2, obfs3                               |         1 |
| obfs3, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

