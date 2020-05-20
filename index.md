---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-05-20 15:00 UTC**

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
| [abuse-contact@to-surf-and-protect.net](endtoend-correlation-groups#abuse-contactto-surf-and-protectnet)                       | 1.35        | 20.86      | 148       | 4               | 2020-03-27     | 1                           |
| [https://www.torservers.net/donate.html &lt;support .A](endtoend-correlation-groups#httpswwwtorserversnetdonatehtml-support-a) | 0.02        | 3.25       | 17        | 4               | 2019-02-06     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                           | 0.01        | 0.01       | 2         | 2               | 2019-10-25     | 1                           |
| **Total**                                                                                                                      | **1.38**    | **24.12**  | **167**   |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     21.04 |       140 | 2016-01-25   |
| [johntor336@hotmail.com](https://metrics.torproject.org/rs.html#search/family:0077440D06BF55C02432CD9B6E30D74A1E193095)                                   |     15.21 |        86 | 2020-04-13   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |      6.05 |        32 | 2018-03-21   |
| [loribthorpe@hotmail.com](https://metrics.torproject.org/rs.html#search/family:00BC71A338099F9A387C3BF314A5BD4FB48A6FB9)                                  |      3.54 |        62 | 2020-02-05   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      3.4  |        18 | 2018-03-01   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.39 |        17 | 2016-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      2.42 |        50 | 2016-08-22   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      1.86 |        19 | 2013-06-11   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:09DCA3360179C6C8A5A20DDDE1C54662965EF1BA)                                    |      1.85 |        36 | 2019-04-05   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      1.66 |        11 | 2017-12-05   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |       1.55 |        14 | 2018-10-05   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)              |       0.87 |        20 | 2018-01-07   |
| [abuse@for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                                    |       0.86 |        11 | 2019-03-16   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                      |       0.84 |         8 | 2018-09-25   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                                 |       0.79 |         5 | 2017-10-24   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                                 |       0.77 |         4 | 2018-08-17   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:14E72D4DA10B66353E583F26EE04AC0D563EA7EF)                       |       0.75 |        32 | 2019-02-23   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://metrics.torproject.org/rs.html#search/family:021047C51A57254D263DDB8B9277CA1C286D600E) |       0.74 |         9 | 2014-04-09   |
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |       0.7  |       143 | 2016-01-25   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:12B1A5769D38FF47CF68C2235E1BDA315DF400F2)                                     |       0.7  |        25 | 2018-08-28   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |            7.465 |     21.04 |       0.7  |       146 | 2016-01-25   |
| [johntor336@hotmail.com](https://metrics.torproject.org/rs.html#search/family:0077440D06BF55C02432CD9B6E30D74A1E193095)                                   |            5.162 |     15.21 |       0.13 |        86 | 2020-04-13   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |            2.047 |      6.05 |       0.04 |        32 | 2018-03-21   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            1.21  |      3.4  |       0.12 |        21 | 2017-06-13   |
| [loribthorpe@hotmail.com](https://metrics.torproject.org/rs.html#search/family:00BC71A338099F9A387C3BF314A5BD4FB48A6FB9)                                  |            1.2   |      3.54 |       0.02 |        62 | 2020-02-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.151 |      3.39 |       0.03 |        17 | 2016-12-23   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.892 |      0    |       1.55 |        14 | 2018-10-05   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            0.822 |      2.42 |       0.02 |        50 | 2016-08-22   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.648 |      1.86 |       0.04 |        20 | 2013-06-11   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:09DCA3360179C6C8A5A20DDDE1C54662965EF1BA)                                    |            0.632 |      1.85 |       0    |        37 | 2019-04-05   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                        |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                        |            17.38 |      15.64 |     24.13 |       669 |
| Hetzner Online GmbH            |            14.65 |      22.5  |      0.6  |       370 |
| Joshua Peter McQuistan         |             7.44 |       0.6  |     21.04 |       146 |
| Online S.a.s.                  |             7.34 |      11.08 |      1.92 |       247 |
| netcup GmbH                    |             2.53 |       2.94 |      0.59 |       111 |
| FranTech Solutions             |             2.07 |       0.84 |      4.64 |       109 |
| F3 Netze e.V.                  |             2.04 |       0.04 |      6.05 |        32 |
| myLoc managed IT AG            |             1.96 |       2.85 |      0.89 |        46 |
| Foundation for Applied Privacy |             1.15 |       0.03 |      3.4  |        18 |
| NForce Entertainment B.V.      |             1.13 |       0.45 |      2.23 |        23 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.2         |             53.5 |     66.42 |      45.99 |      3251 |
| 0.4.3         |             24   |     25.13 |      23.7  |      1224 |
| 0.3.5         |             14.3 |      6.67 |      18.51 |      1181 |
| 0.4.1         |              6.8 |      1.5  |       9.92 |       425 |
| 0.4.4         |              1.1 |      0.26 |       1.85 |        48 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             1.17 |       1.85 |      0.26 |        48 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.4 |      92.1 |       92.5 |      5566 |
| BSD     |              7.3 |       7.7 |        7.2 |       451 |
| Windows |              0.1 |       0   |        0.1 |        44 |
| Darwin  |              0   |       0   |        0   |         8 |
| SunOS   |              0   |       0   |        0   |         3 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            35.71 |      31.29 |       28.37 |     47.47 |      1401 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     48.23 |            480 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       687 |
| None                                       |       409 |
| obfs3, obfs4                               |        64 |
| fte, obfs3, obfs4, scramblesuit, websocket |        19 |
| meek                                       |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
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

