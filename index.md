---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-05-15 11:00 UTC**

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
| [abuse-contact@to-surf-and-protect.net](endtoend-correlation-groups#abuse-contactto-surf-and-protectnet) | 1.01        | 21.52      | 148       | 4               | 2020-03-27     | 1                           |
| [tor-abuse&lt;at&gt;mailbox&lt;dot&gt;org](endtoend-correlation-groups#tor-abuseatmailboxdotorg)         | 0.11        | 0.23       | 5         | 5               | 2020-05-15     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)     | 0.01        | 0.01       | 2         | 2               | 2019-10-25     | 1                           |
| **Total**                                                                                                | **1.13**    | **21.76**  | **155**   |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     21.73 |       140 | 2016-01-25   |
| [johntor336@hotmail.com](https://metrics.torproject.org/rs.html#search/family:0077440D06BF55C02432CD9B6E30D74A1E193095)                                   |     13.68 |        86 | 2020-04-13   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |      5.24 |        28 | 2018-03-21   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.95 |        17 | 2016-12-23   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      3.73 |        18 | 2018-03-01   |
| [loribthorpe@hotmail.com](https://metrics.torproject.org/rs.html#search/family:00BC71A338099F9A387C3BF314A5BD4FB48A6FB9)                                  |      3.71 |        59 | 2020-02-05   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      2.6  |        50 | 2016-08-22   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:09DCA3360179C6C8A5A20DDDE1C54662965EF1BA)                                    |      1.81 |        36 | 2019-04-05   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      1.77 |        18 | 2013-06-11   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      1.69 |        11 | 2017-12-05   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |       1.53 |        14 | 2018-10-05   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                      |       0.96 |         8 | 2018-09-25   |
| [abuse@for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                                    |       0.86 |        10 | 2019-03-16   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)              |       0.81 |        15 | 2018-01-07   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                                 |       0.81 |         5 | 2017-10-24   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:12B1A5769D38FF47CF68C2235E1BDA315DF400F2)                                     |       0.74 |        26 | 2018-08-28   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                                 |       0.69 |         4 | 2018-08-17   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://metrics.torproject.org/rs.html#search/family:063BD3BF8C110617E7CA09C96C0EDC0270329F0B) |       0.68 |         9 | 2014-04-09   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:14E72D4DA10B66353E583F26EE04AC0D563EA7EF)                       |       0.67 |        29 | 2019-02-23   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)            |       0.6  |        23 | 2015-05-16   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |            7.199 |     21.73 |       0.41 |       146 | 2016-01-25   |
| [johntor336@hotmail.com](https://metrics.torproject.org/rs.html#search/family:0077440D06BF55C02432CD9B6E30D74A1E193095)                                   |            4.365 |     13.68 |       0    |        86 | 2020-04-13   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |            1.673 |      5.24 |       0    |        28 | 2018-03-21   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.261 |      3.95 |       0    |        17 | 2016-12-23   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            1.243 |      3.73 |       0.09 |        21 | 2017-06-13   |
| [loribthorpe@hotmail.com](https://metrics.torproject.org/rs.html#search/family:00BC71A338099F9A387C3BF314A5BD4FB48A6FB9)                                  |            1.183 |      3.71 |       0    |        59 | 2020-02-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.885 |      0    |       1.53 |        14 | 2018-10-05   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            0.829 |      2.6  |       0    |        50 | 2016-08-22   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:09DCA3360179C6C8A5A20DDDE1C54662965EF1BA)                                    |            0.598 |      1.81 |       0    |        37 | 2019-04-05   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.587 |      1.77 |       0.03 |        19 | 2013-06-11   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                        |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                        |            16.85 |      15.84 |     22.42 |       732 |
| Hetzner Online GmbH            |            15.44 |      22.83 |      0.6  |       412 |
| Online S.a.s.                  |             7.92 |      11.74 |      2.25 |       273 |
| Joshua Peter McQuistan         |             7.11 |       0.24 |     21.73 |       145 |
| netcup GmbH                    |             2.6  |       3.15 |      0.56 |       122 |
| FranTech Solutions             |             1.94 |       0.69 |      4.64 |       109 |
| myLoc managed IT AG            |             1.92 |       2.69 |      0.94 |        46 |
| F3 Netze e.V.                  |             1.67 |       0    |      5.24 |        28 |
| NForce Entertainment B.V.      |             1.2  |       0.53 |      2.39 |        24 |
| Foundation for Applied Privacy |             1.19 |       0    |      3.73 |        18 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.2         |             70.3 |     88.46 |      60.48 |      4325 |
| 0.3.5         |             13.9 |      6.65 |      17.7  |      1201 |
| 0.4.1         |              6.9 |      1.62 |       9.78 |       453 |
| 0.4.3         |              3.2 |      2    |       4.18 |       142 |
| 0.4.0         |              2.9 |      0.1  |       4.53 |        98 |
| 0.2.9         |              1.4 |      0.82 |       1.41 |       273 |
| 0.4.4         |              1.1 |      0.3  |       1.88 |        45 |
| 0.3.6         |              0   |      0    |       0    |         1 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.51 |       7.83 |      1.23 |       417 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.5 |      91.9 |       92.6 |      5978 |
| BSD     |              7.1 |       7.9 |        7.1 |       468 |
| Windows |              0.1 |       0   |        0.1 |        48 |
| Darwin  |              0   |       0   |        0   |         8 |
| SunOS   |              0   |       0   |        0   |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            35.03 |      29.62 |       27.61 |     48.74 |      1446 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     49.68 |            482 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       706 |
| None                                       |       405 |
| obfs3, obfs4                               |        65 |
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
| meek, meek, obfs4                          |         1 |
| meek, obfs3, obfs4                         |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs3, scramblesuit                        |         1 |
| obfs4, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

