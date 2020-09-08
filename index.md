---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-09-08 13:00 UTC**

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
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](endtoend-correlation-groups#kevin-hicks-adminfissionrelaysnet) | 0.71        | 0.32       | 23        | 11              | 2020-08-10     | 1                           |
| [see https://www.artikel5ev.de/torcontact/](endtoend-correlation-groups#see-httpswwwartikel5evdetorcontact)  | 0.25        | 0.57       | 17        | 10              | 2020-09-07     | 15                          |
| [tomas.vanagas@knf.vu.lt tor-relay.co](endtoend-correlation-groups#tomasvanagasknfvult-tor-relayco)          | 0.04        | 0.07       | 2         | 2               | 2020-04-28     | 1                           |
| **Total**                                                                                                    | **1.00**    | **0.96**   | **42**    |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     19.68 |       123 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)  |      8.3  |        32 | 2018-03-21   |
| [Digitalcourage e.V. email:tor-abuse digitalcourag](https://metrics.torproject.org/rs.html#search/family:027E75C92F1231AE5F7BD4E1536696FE3040C460)        |      5.59 |        30 | 2020-07-06   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      4.65 |        22 | 2018-03-01   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.78 |        17 | 2016-12-23   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      2.67 |        19 | 2013-06-11   |
| [ian@ian.sh](https://metrics.torproject.org/rs.html#search/family:0C9D7DB63BE030E5CA32E25606632AEB85840F4C)                                               |      2.34 |        46 | 2020-07-04   |
| [exitno@elude.in](https://metrics.torproject.org/rs.html#search/family:48D934E776B739D38F9EAFDCFD85203C6A68A67B)                                          |      1.86 |         9 | 2020-08-06   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      1.56 |        15 | 2014-04-09   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:09DCA3360179C6C8A5A20DDDE1C54662965EF1BA)                                    |      1.48 |        36 | 2019-04-05   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                             |   Guard(%) |   #Relays | First Seen   |
|:-----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:02758CD398E3F842EF82478078AAAE0273770DB2)         |       1.79 |        21 | 2019-01-05   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE) |       1.45 |        25 | 2015-05-16   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)           |       1.37 |        14 | 2018-10-05   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)   |       0.68 |        14 | 2018-01-07   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:04D9CEA8D778ABA130B014F758C2BCADD31DA05E)            |       0.64 |        29 | 2019-02-23   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                      |       0.64 |         5 | 2017-10-24   |
| [abuse@for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                         |       0.63 |        10 | 2019-03-16   |
| [63540827](https://metrics.torproject.org/rs.html#search/family:63540827C4832D214984EA47B7A68C593F9F862F)                                      |       0.61 |         2 | 2018-12-12   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                      |       0.59 |         4 | 2018-08-17   |
| [torrelaysaregreat@gmail.com](https://metrics.torproject.org/rs.html#search/family:1A7A2516A961F2838F7F94786A8811BE82F9CFFE)                   |       0.58 |        23 | 2018-08-28   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |            6.723 |     19.68 |       1.79 |       144 | 2016-01-25   |
| [F3 Netze &lt;abuse@f3netze.de&gt; email:abuse f3netze.d](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)  |            2.411 |      8.3  |       0    |        32 | 2018-03-21   |
| [Digitalcourage e.V. email:tor-abuse digitalcourag](https://metrics.torproject.org/rs.html#search/family:027E75C92F1231AE5F7BD4E1536696FE3040C460)        |            1.623 |      5.59 |       0    |        30 | 2020-07-06   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            1.441 |      4.65 |       0.13 |        27 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.099 |      3.78 |       0    |        17 | 2016-12-23   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)            |            0.818 |      0    |       1.45 |        25 | 2015-05-16   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.789 |      2.67 |       0.02 |        20 | 2013-06-11   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.772 |      0    |       1.37 |        14 | 2018-10-05   |
| [ian@ian.sh](https://metrics.torproject.org/rs.html#search/family:0C9D7DB63BE030E5CA32E25606632AEB85840F4C)                                               |            0.704 |      2.34 |       0.03 |        50 | 2020-07-04   |
| [exitno@elude.in](https://metrics.torproject.org/rs.html#search/family:48D934E776B739D38F9EAFDCFD85203C6A68A67B)                                          |            0.54  |      1.86 |       0    |         9 | 2020-08-06   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH    |            17.02 |      23.62 |      0.13 |       490 |
| OVH SAS                |            12.16 |      14.98 |     10.8  |       589 |
| Online S.a.s.          |             6.72 |      10.35 |      2.4  |       241 |
| Joshua Peter McQuistan |             6.27 |       0.99 |     19.68 |       137 |
| F3 Netze e.V.          |             2.41 |       0    |      8.3  |        32 |
| Zwiebelfreunde e.V.    |             2.11 |       0    |      7.29 |        38 |
| netcup GmbH            |             2.08 |       2.6  |      0.59 |       129 |
| myLoc managed IT AG    |             1.78 |       2.68 |      0.97 |        46 |
| FranTech Solutions     |             1.77 |       0.84 |      4.17 |       119 |
| Linode, LLC            |             1.66 |       0.6  |      0.15 |       276 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.3         |             69.9 |     85.48 |      60.59 |      4300 |
| 0.4.2         |             12.9 |      9.77 |      15.16 |      1088 |
| 0.3.5         |             11.3 |      2.5  |      15.89 |      1027 |
| 0.4.1         |              2.3 |      0.48 |       3.68 |       188 |
| 0.4.4         |              2   |      0.97 |       2.83 |       111 |
| 0.4.5         |              1.2 |      0.77 |       1.83 |        32 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             2.36 |       3.68 |      0.48 |       188 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.5 |      91.2 |       92.2 |      6212 |
| BSD     |              7.2 |       8.6 |        7.5 |       451 |
| SunOS   |              0   |       0   |        0   |         5 |
| Darwin  |              0   |       0   |        0   |         5 |
| Windows |              0   |       0   |        0   |        36 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            35.35 |      30.36 |       24.73 |     54.43 |      1478 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     55.27 |            491 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1164 |
| None                                       |       406 |
| obfs3, obfs4                               |        71 |
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

