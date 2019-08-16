---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-08-16 09:00 UTC**

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
| [Steven S &lt;katsalmovies@gmail.com&gt;](endtoend-correlation-groups#steven-s-katsalmoviesgmailcom) | 0.06        | 0.09       | 3         | 2               | 2019-07-28     | 1                           |
| **Total**                                                                                            | **0.06**    | **0.09**   | **3**     |                 |                |                             |

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
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |     13.33 |        50 | 2016-08-22   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                            |      9.33 |        42 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      6.77 |        12 | 2018-03-23   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |      5.98 |        55 | 2019-04-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      5.71 |        17 | 2016-12-23   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      4.07 |        13 | 2013-06-11   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      2.37 |        13 | 2015-05-22   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |      1.85 |        15 | 2014-04-09   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      1.79 |        12 | 2017-12-05   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:6BCB964AB74E23F8986BDA905697D3A6BE08AF28)                        |      1.61 |         8 | 2018-03-21   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                         |       1.67 |        20 | 2019-01-05   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |       1.25 |        11 | 2018-10-05   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:3B4C5729F829CA2E895B81AF834A63DB336D0FFE)           |       0.76 |        12 | 2018-01-07   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |       0.71 |         5 | 2016-09-06   |
| [abuse AT for-privacy.net](https://metrics.torproject.org/rs.html#search/family:05250BA7E128350D14ED9A712639AC2EFCFF618B)                              |       0.68 |         8 | 2019-04-15   |
| [jwbecher@drazisil.com](https://metrics.torproject.org/rs.html#search/family:03310DA245BD3578412B453FC5A5A8538030671E)                                 |       0.58 |         8 | 2018-05-08   |
| [torrpi1405 at gmail.com](https://metrics.torproject.org/rs.html#search/family:39F91959416763AFD34DBEEC05474411B964B2DC)                               |       0.55 |        19 | 2018-08-28   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.52 |         8 | 2016-01-03   |
| [torrelay@brave.com](https://metrics.torproject.org/rs.html#search/family:6E8E5CA9B6F567416ADA21E990E7746BC223B0C0)                                    |       0.51 |         6 | 2018-03-01   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.47 |         3 | 2015-04-22   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                            |            3.535 |      9.33 |       1.67 |        64 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |            3.438 |     13.33 |       0    |        50 | 2016-08-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            2.042 |      6.77 |       0.46 |        19 | 2017-06-13   |
| [tech@emeraldonion.org](https://metrics.torproject.org/rs.html#search/family:05EAA0696DCB694D6811042348DACD5059FE64AD)                                    |            1.56  |      5.98 |       0.02 |        56 | 2019-04-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |            1.474 |      5.71 |       0    |        17 | 2016-12-23   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |            1.05  |      4.07 |       0    |        14 | 2013-06-11   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |            0.795 |      0    |       1.25 |        12 | 2018-10-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |            0.611 |      2.37 |       0    |        13 | 2015-05-22   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:3B4C5729F829CA2E895B81AF834A63DB336D0FFE)              |            0.528 |      0.17 |       0.76 |        14 | 2018-01-07   |
| [Hart voor Internetvrijheid &lt;abuse AT hartvoorinter](https://metrics.torproject.org/rs.html#search/family:0485027A0A349D454D978F6C1CECDD29EA17769A)    |            0.478 |      1.85 |       0    |        15 | 2014-04-09   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                                                          |            15.53 |      20.37 |      8.02 |       618 |
| Hetzner Online GmbH                                              |            14.44 |      18.47 |      0.07 |       425 |
| Online S.a.s.                                                    |             8.35 |      10.59 |      4.74 |       314 |
| Quintex Alliance Consulting                                      |             3.43 |       0    |     13.33 |        50 |
| Joshua Peter McQuistan                                           |             2.69 |       0.27 |      9.33 |        47 |
| netcup GmbH                                                      |             2.42 |       3.05 |      0.12 |        89 |
| Iomart Cloud Services Limited                                    |             2.23 |       3.2  |      0    |        21 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             1.97 |       0.35 |      6.77 |        17 |
| myLoc managed IT AG                                              |             1.56 |       2.2  |      0.34 |        36 |
| Emerald Onion                                                    |             1.56 |       0.02 |      5.98 |        56 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.0         |             45.1 |     57.76 |      40.89 |      2566 |
| 0.3.5         |             30   |     28.81 |      30.62 |      1754 |
| 0.3.4         |              9.6 |      1.93 |      13.42 |       565 |
| 0.2.9         |              6.4 |      2.55 |       7.61 |       791 |
| 0.4.1         |              4.1 |      6.86 |       2.23 |       126 |
| 0.3.2         |              1.3 |      0.81 |       1.66 |       164 |
| 0.4.2         |              1.1 |      0.42 |       1.61 |        36 |
| 0.3.3         |              1   |      0.53 |       1.19 |       119 |
| 0.2.5         |              0.2 |      0.25 |       0.18 |       100 |
| 0.3.1         |              0.2 |      0.01 |       0.39 |        46 |
| 0.2.4         |              0.1 |      0.02 |       0.01 |       113 |
| 0.2.6         |              0   |      0    |       0    |        26 |
| 0.2.7         |              0   |      0    |       0.02 |        61 |
| 0.2.8         |              0   |      0    |       0.02 |        13 |
| 0.3.0         |              0   |      0    |       0.09 |        52 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|            13.04 |      17.01 |      3.57 |      1259 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.3 |      84.6 |       94   |      5931 |
| BSD     |              8.3 |      15.2 |        5.6 |       444 |
| Darwin  |              0.1 |       0   |        0   |        18 |
| Windows |              0.1 |       0   |        0   |        83 |
| SunOS   |              0   |       0   |        0   |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            29.58 |      23.53 |       24.67 |     45.34 |      1082 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|      46.7 |            314 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       523 |
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
| obfs3, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

