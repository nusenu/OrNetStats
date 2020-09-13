---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-09-13 06:00 UTC**

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
| [tomas.vanagas@knf.vu.lt tor-relay.co](endtoend-correlation-groups#tomasvanagasknfvult-tor-relayco)  | 0.02        | 0.06       | 2         | 2               | 2020-04-28     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com) | 0.01        | 0.01       | 2         | 2               | 2019-10-25     | 1                           |
| **Total**                                                                                            | **0.03**    | **0.07**   | **4**     |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     18.52 |       123 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)  |      8.67 |        32 | 2018-03-21   |
| [Digitalcourage e.V. email:tor-abuse digitalcourag](https://metrics.torproject.org/rs.html#search/family:027E75C92F1231AE5F7BD4E1536696FE3040C460)        |      5.55 |        31 | 2016-05-27   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      4.15 |        22 | 2018-03-01   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.88 |        17 | 2016-12-23   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      2.63 |        19 | 2013-06-11   |
| [BlackHatsMatter@protonmail.com](https://metrics.torproject.org/rs.html#search/family:05363963D91D350C62440199E065695EB629E978)                           |      2.55 |        35 | 2020-08-25   |
| [exit abuse@posteo.net](https://metrics.torproject.org/rs.html#search/family:0694244F5E80089976608450E4154F8444C06948)                                    |      2.53 |        29 | 2020-09-04   |
| [ian@ian.sh](https://metrics.torproject.org/rs.html#search/family:0C9D7DB63BE030E5CA32E25606632AEB85840F4C)                                               |      2.2  |        44 | 2020-07-04   |
| [exitno@elude.in](https://metrics.torproject.org/rs.html#search/family:48D934E776B739D38F9EAFDCFD85203C6A68A67B)                                          |      1.84 |         9 | 2020-08-06   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                             |   Guard(%) |   #Relays | First Seen   |
|:-----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:02758CD398E3F842EF82478078AAAE0273770DB2)         |       2.1  |        21 | 2019-01-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)           |       1.33 |        14 | 2018-10-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE) |       1.26 |        25 | 2015-05-16   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)   |       0.81 |        15 | 2018-01-07   |
| [Peter Gerber &lt;tor@arbitrary.ch&gt;](https://metrics.torproject.org/rs.html#search/family:3F43D0584A2613C9DB631382FF486DC6B95EA1C8)         |       0.72 |         8 | 2019-01-20   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                      |       0.65 |         5 | 2017-10-24   |
| [torrelaysaregreat@gmail.com](https://metrics.torproject.org/rs.html#search/family:12B1A5769D38FF47CF68C2235E1BDA315DF400F2)                   |       0.62 |        23 | 2018-08-28   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:04D9CEA8D778ABA130B014F758C2BCADD31DA05E)            |       0.56 |        29 | 2019-02-23   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                      |       0.56 |         4 | 2018-08-17   |
| [abuse@for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                         |       0.53 |        10 | 2019-03-16   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |            6.512 |     18.52 |       2.1  |       144 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)  |            2.476 |      8.67 |       0    |        32 | 2018-03-21   |
| [Digitalcourage e.V. email:tor-abuse digitalcourag](https://metrics.torproject.org/rs.html#search/family:027E75C92F1231AE5F7BD4E1536696FE3040C460)        |            1.586 |      5.55 |       0    |        31 | 2016-05-27   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            1.271 |      4.15 |       0.12 |        27 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.108 |      3.88 |       0    |        17 | 2016-12-23   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.777 |      2.63 |       0.04 |        20 | 2013-06-11   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.774 |      0    |       1.33 |        14 | 2018-10-05   |
| [BlackHatsMatter@protonmail.com](https://metrics.torproject.org/rs.html#search/family:05363963D91D350C62440199E065695EB629E978)                           |            0.773 |      2.55 |       0.07 |        44 | 2020-08-25   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)            |            0.732 |      0    |       1.26 |        25 | 2015-05-16   |
| [exit abuse@posteo.net](https://metrics.torproject.org/rs.html#search/family:0694244F5E80089976608450E4154F8444C06948)                                    |            0.724 |      2.53 |       0    |        29 | 2020-09-04   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH    |            16.66 |      24.32 |      0.11 |       429 |
| OVH SAS                |            11.68 |      14.29 |      9.29 |       567 |
| Online S.a.s.          |             7.06 |      10.26 |      2.31 |       256 |
| Joshua Peter McQuistan |             6.01 |       1.24 |     18.52 |       137 |
| F3 Netze e.V.          |             2.47 |       0    |      8.67 |        32 |
| netcup GmbH            |             2.19 |       2.77 |      0.57 |       128 |
| Zwiebelfreunde e.V.    |             2.05 |       0    |      7.19 |        38 |
| FranTech Solutions     |             1.98 |       0.56 |      5.34 |       123 |
| myLoc managed IT AG    |             1.73 |       2.48 |      1.01 |        47 |
| Linode, LLC            |             1.4  |       0.72 |      0.07 |       254 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.3         |             69.3 |     86.07 |      61.58 |      4211 |
| 0.4.2         |             13.4 |      9.44 |      15.03 |      1070 |
| 0.3.5         |             12.1 |      2.39 |      16.35 |      1025 |
| 0.4.4         |              1.9 |      1.11 |       2.55 |       110 |
| 0.4.1         |              1.8 |      0.26 |       2.64 |       169 |
| 0.4.5         |              1.2 |      0.7  |       1.81 |        33 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|              1.8 |       2.64 |      0.26 |       169 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.8 |      91.8 |       92.9 |      6073 |
| BSD     |              6.9 |       8   |        6.8 |       458 |
| SunOS   |              0   |       0   |        0.1 |         5 |
| Darwin  |              0   |       0   |        0   |         5 |
| Windows |              0   |       0   |        0   |        32 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            36.29 |       30.8 |        28.2 |     53.28 |      1491 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     53.74 |            491 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1159 |
| None                                       |       409 |
| obfs3, obfs4                               |        72 |
| fte, obfs3, obfs4, scramblesuit            |        21 |
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
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs3, scramblesuit                        |         1 |
| obfs4, scramblesuit                        |         1 |
| obfs4, websocket                           |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

