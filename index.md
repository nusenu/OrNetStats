---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-09-06 12:00 UTC**

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

| Contact                                                                                                      | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](endtoend-correlation-groups#kevin-hicks-adminfissionrelaysnet) | 0.69        | 0.31       | 23        | 11              | 2020-08-10     | 1                           |
| [see https://www.artikel5ev.de/torcontact/](endtoend-correlation-groups#see-httpswwwartikel5evdetorcontact)  | 0.24        | 0.56       | 16        | 10              | 2020-08-28     | 1                           |
| [tomas.vanagas@knf.vu.lt tor-relay.co](endtoend-correlation-groups#tomasvanagasknfvult-tor-relayco)          | 0.04        | 0.07       | 2         | 2               | 2020-04-28     | 1                           |
| [comments at worldofmatthew dot com](endtoend-correlation-groups#commentsatworldofmatthewdotcom)             | 0.02        | 0.03       | 2         | 2               | 2020-09-03     | 1                           |
| **Total**                                                                                                    | **0.99**    | **0.97**   | **43**    |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     20.05 |       123 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)  |      8.69 |        32 | 2018-03-21   |
| [Digitalcourage e.V. email:tor-abuse digitalcourag](https://metrics.torproject.org/rs.html#search/family:027E75C92F1231AE5F7BD4E1536696FE3040C460)        |      5.72 |        30 | 2020-07-06   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      4.56 |        22 | 2018-03-01   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.89 |        17 | 2016-12-23   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      2.67 |        19 | 2013-06-11   |
| [ian@ian.sh](https://metrics.torproject.org/rs.html#search/family:0C9D7DB63BE030E5CA32E25606632AEB85840F4C)                                               |      2.36 |        46 | 2020-07-04   |
| [exitno@elude.in](https://metrics.torproject.org/rs.html#search/family:48D934E776B739D38F9EAFDCFD85203C6A68A67B)                                          |      1.68 |         9 | 2020-08-06   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      1.61 |        15 | 2014-04-09   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:09DCA3360179C6C8A5A20DDDE1C54662965EF1BA)                                    |      1.45 |        36 | 2019-04-05   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                             |   Guard(%) |   #Relays | First Seen   |
|:-----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:02758CD398E3F842EF82478078AAAE0273770DB2)         |       1.81 |        21 | 2019-01-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)           |       1.42 |        14 | 2018-10-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE) |       1.32 |        25 | 2015-05-16   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)   |       0.66 |        14 | 2018-01-07   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                      |       0.66 |         5 | 2017-10-24   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:04D9CEA8D778ABA130B014F758C2BCADD31DA05E)            |       0.64 |        30 | 2019-02-23   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                      |       0.62 |         5 | 2016-09-06   |
| [63540827](https://metrics.torproject.org/rs.html#search/family:63540827C4832D214984EA47B7A68C593F9F862F)                                      |       0.62 |         2 | 2018-12-12   |
| [torrelaysaregreat@gmail.com](https://metrics.torproject.org/rs.html#search/family:1A7A2516A961F2838F7F94786A8811BE82F9CFFE)                   |       0.6  |        23 | 2018-08-28   |
| [Peter Gerber &lt;tor@arbitrary.ch&gt;](https://metrics.torproject.org/rs.html#search/family:3F43D0584A2613C9DB631382FF486DC6B95EA1C8)         |       0.53 |         8 | 2019-01-20   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |            6.876 |     20.05 |       1.81 |       144 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)  |            2.536 |      8.69 |       0    |        32 | 2018-03-21   |
| [Digitalcourage e.V. email:tor-abuse digitalcourag](https://metrics.torproject.org/rs.html#search/family:027E75C92F1231AE5F7BD4E1536696FE3040C460)        |            1.669 |      5.72 |       0    |        30 | 2020-07-06   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            1.409 |      4.56 |       0.12 |        27 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.137 |      3.89 |       0    |        17 | 2016-12-23   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.803 |      0    |       1.42 |        14 | 2018-10-05   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.794 |      2.67 |       0.02 |        20 | 2013-06-11   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)            |            0.75  |      0    |       1.32 |        25 | 2015-05-16   |
| [ian@ian.sh](https://metrics.torproject.org/rs.html#search/family:0C9D7DB63BE030E5CA32E25606632AEB85840F4C)                                               |            0.707 |      2.36 |       0.03 |        50 | 2020-07-04   |
| [exitno@elude.in](https://metrics.torproject.org/rs.html#search/family:48D934E776B739D38F9EAFDCFD85203C6A68A67B)                                          |            0.491 |      1.68 |       0    |         9 | 2020-08-06   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH    |            17.08 |      23.92 |      0.13 |       515 |
| OVH SAS                |            12.06 |      14.8  |     10.83 |       588 |
| Online S.a.s.          |             6.91 |      10.49 |      2.56 |       240 |
| Joshua Peter McQuistan |             6.44 |       1.05 |     20.05 |       137 |
| F3 Netze e.V.          |             2.53 |       0    |      8.69 |        32 |
| Zwiebelfreunde e.V.    |             2.16 |       0    |      7.41 |        38 |
| netcup GmbH            |             2.12 |       2.62 |      0.57 |       129 |
| FranTech Solutions     |             1.79 |       0.85 |      4.18 |       116 |
| myLoc managed IT AG    |             1.77 |       2.57 |      1.03 |        47 |
| Linode, LLC            |             1.45 |       0.59 |      0.16 |       273 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.3         |             69.9 |     85.77 |      60.39 |      4355 |
| 0.4.2         |             12.9 |      9.64 |      15.12 |      1093 |
| 0.3.5         |             11.3 |      2.39 |      15.99 |      1017 |
| 0.4.1         |              2.4 |      0.5  |       3.85 |       194 |
| 0.4.4         |              1.9 |      0.93 |       2.68 |       107 |
| 0.4.5         |              1.3 |      0.73 |       1.93 |        34 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             2.48 |       3.85 |       0.5 |       194 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.7 |      91.5 |       92.5 |      6277 |
| BSD     |              7   |       8.4 |        7.2 |       444 |
| Windows |              0.1 |       0   |        0   |        37 |
| Darwin  |              0   |       0   |        0   |         4 |
| SunOS   |              0   |       0   |        0   |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            36.07 |      30.78 |       25.63 |     55.18 |      1464 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     56.14 |            481 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1159 |
| None                                       |       405 |
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

