---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-08-11 15:00 UTC**

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
| [samam &lt; at &gt; protonmail.com](endtoend-correlation-groups#samam--at--protonmailcom-)           | 0.14        | 0.07       | 2         | 2               | 2016-03-28     | 1                           |
| [Steven S &lt;katsalmovies@gmail.com&gt;](endtoend-correlation-groups#steven-s-katsalmoviesgmailcom) | 0.04        | 0.12       | 3         | 2               | 2019-07-28     | 1                           |
| **Total**                                                                                            | **0.18**    | **0.19**   | **5**     |                 |                |                             |

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
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |     13.58 |        50 | 2016-08-22   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                            |     10.69 |        42 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      6.26 |        12 | 2018-03-23   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      6.08 |        17 | 2016-12-23   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |      5.42 |        55 | 2019-04-05   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      4.05 |        13 | 2013-06-11   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:6BCB964AB74E23F8986BDA905697D3A6BE08AF28)                        |      2.3  |         4 | 2018-03-21   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      2.28 |        15 | 2014-04-09   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      2.15 |        13 | 2015-05-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      1.72 |         4 | 2014-11-21   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                         |       1.73 |        20 | 2019-01-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |       1.64 |        12 | 2018-10-05   |
| [pastly@tp.o 0x94FBBB0A](https://metrics.torproject.org/rs.html#search/family:2767A9DB46503D09FD0415BA1296B36318520F08)                                |       1.19 |         6 | 2019-06-10   |
| [torrelay@brave.com](https://metrics.torproject.org/rs.html#search/family:6E8E5CA9B6F567416ADA21E990E7746BC223B0C0)                                    |       0.89 |         6 | 2018-03-01   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                   |       0.84 |         6 | 2018-09-25   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:3B4C5729F829CA2E895B81AF834A63DB336D0FFE)           |       0.74 |        12 | 2018-01-07   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |       0.73 |         5 | 2016-09-06   |
| [63540827](https://metrics.torproject.org/rs.html#search/family:63540827C4832D214984EA47B7A68C593F9F862F)                                              |       0.64 |         2 | 2018-12-12   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.57 |         8 | 2016-01-03   |
| [abuse AT for-privacy.net](https://metrics.torproject.org/rs.html#search/family:05250BA7E128350D14ED9A712639AC2EFCFF618B)                              |       0.55 |         8 | 2019-04-15   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                            |            3.667 |     10.69 |       1.73 |        64 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            3.046 |     13.58 |       0    |        50 | 2016-08-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            1.683 |      6.26 |       0.22 |        19 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.363 |      6.08 |       0    |        17 | 2016-12-23   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |            1.26  |      5.42 |       0.06 |        56 | 2019-04-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            1.116 |      0    |       1.64 |        12 | 2018-10-05   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            0.91  |      4.05 |       0    |        14 | 2013-06-11   |
| [pastly@tp.o 0x94FBBB0A](https://metrics.torproject.org/rs.html#search/family:2767A9DB46503D09FD0415BA1296B36318520F08)                                   |            0.811 |      0    |       1.19 |         6 | 2019-06-10   |
| [torrelay@brave.com](https://metrics.torproject.org/rs.html#search/family:6E8E5CA9B6F567416ADA21E990E7746BC223B0C0)                                       |            0.611 |      0    |       0.89 |         6 | 2018-03-01   |
| [retik.eu &lt;retik@systemli.org&gt;](https://metrics.torproject.org/rs.html#search/family:014E24C0CD21D2B9829E841D5EC1D3C415F866BF)                      |            0.577 |      0    |       0.84 |         6 | 2018-09-25   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                                                          |            16.23 |      20.25 |      8.77 |       616 |
| Hetzner Online GmbH                                              |            16.13 |      19.94 |      0.05 |       419 |
| Online S.a.s.                                                    |             7.34 |       8.95 |      4.1  |       301 |
| Quintex Alliance Consulting                                      |             3.04 |       0    |     13.58 |        50 |
| Joshua Peter McQuistan                                           |             2.65 |       0.38 |     10.69 |        45 |
| netcup GmbH                                                      |             2.32 |       2.81 |      0.09 |        92 |
| Iomart Cloud Services Limited                                    |             2.15 |       2.89 |      0    |        21 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             1.62 |       0.14 |      6.26 |        17 |
| 1&amp;1 Internet SE                                              |             1.49 |       2.07 |      0.01 |        36 |
| myLoc managed IT AG                                              |             1.34 |       1.8  |      0.28 |        36 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.0         |             42.9 |     56.46 |      38.49 |      2451 |
| 0.3.5         |             31.8 |     30.48 |      32.04 |      1822 |
| 0.3.4         |             10.4 |      2.36 |      13.67 |       599 |
| 0.2.9         |              6   |      2.07 |       6.95 |       801 |
| 0.4.1         |              3.9 |      7.06 |       3.34 |       128 |
| 0.4.2         |              1.5 |      0.24 |       2.15 |        36 |
| 0.3.2         |              1.4 |      0.6  |       1.64 |       175 |
| 0.3.3         |              1   |      0.44 |       1.26 |       119 |
| 0.2.5         |              0.2 |      0.2  |       0.11 |       104 |
| 0.2.4         |              0.1 |      0.02 |       0.02 |       114 |
| 0.3.1         |              0.1 |      0.01 |       0.24 |        47 |
| 0.2.6         |              0   |      0    |       0    |        26 |
| 0.2.7         |              0   |      0    |       0.01 |        61 |
| 0.2.8         |              0   |      0    |       0.02 |        14 |
| 0.3.0         |              0   |      0    |       0.06 |        51 |
| 0.3.6         |              0   |      0    |       0    |         1 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|            13.71 |      17.08 |      3.65 |      1311 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92   |      85.6 |       93.8 |      5948 |
| BSD     |              7.6 |      14.2 |        5.8 |       451 |
| Darwin  |              0.1 |       0   |        0   |        16 |
| Windows |              0.1 |       0   |        0.1 |        89 |
| SunOS   |              0   |       0   |        0   |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            28.46 |      22.93 |       24.52 |     44.84 |      1089 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     45.76 |            308 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       525 |
| None                                       |       434 |
| obfs3, obfs4                               |        69 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| obfs3                                      |         6 |
| meek                                       |         5 |
| obfs2, obfs3, obfs4                        |         5 |
| obfs3, obfs4, scramblesuit                 |         5 |
| fte, meek, obfs3, obfs4                    |         2 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek, meek                                 |         1 |
| obfs2, obfs3                               |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs3, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

