---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-02-27 15:00 UTC**

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

| Contact                                                                                                                     | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:----------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)                   | 0.12        | 0.12       | 6         | 6               | 2018-12-23     | 1                           |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](endtoend-correlation-groups#accessnoworg-abuse-at-accessnow-dot-org) | 0.04        | 1.83       | 13        | 2               | 2019-02-13     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                        | 0.03        | 0.03       | 2         | 2               | 2016-08-28     | 1                           |
| [&lt;nobody AT example dot com&gt;](endtoend-correlation-groups#nobody-at-example-dot-com)                                  | 0.01        | 0.05       | 2         | 2               | 2018-11-22     | 1                           |
| [Jelle Jansen &lt;tormail@gigawebs.net&gt;](endtoend-correlation-groups#jelle-jansen-tormailgigawebsnet)                    | 0.01        | 0.02       | 3         | 3               | 2019-01-09     | 2                           |
| **Total**                                                                                                                   | **0.21**    | **2.05**   | **26**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).


## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Exit(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                         |     15.92 |        46 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:041646640AB306EA74B001966E86169B04CC88D2) |      7.08 |        23 | 2017-02-23   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |      6.36 |        17 | 2016-12-23   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |      5.36 |         8 | 2018-04-05   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      2.77 |        13 | 2015-05-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      1.9  |         4 | 2014-11-21   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      1.88 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      1.83 |        12 | 2017-12-05   |
| [tor-operator@privateinternetaccess.com](https://metrics.torproject.org/rs.html#search/family:3F62F05E859D7F98B086F702A31F7714D566E49A)                |      1.66 |         5 | 2018-12-11   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06) |      1.41 |         7 | 2014-04-08   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:0D12D8E72DED99EE31BB0C57789352BED0CEEEFF)     |       1.19 |        12 | 2017-06-13   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       1.11 |        19 | 2015-05-16   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |       0.88 |         4 | 2018-08-17   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |       0.87 |        15 | 2016-12-11   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:3B4C5729F829CA2E895B81AF834A63DB336D0FFE)           |       0.83 |        13 | 2018-01-07   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.81 |         3 | 2015-04-22   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.71 |         5 | 2017-10-24   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                         |       0.67 |        15 | 2019-01-05   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.67 |         8 | 2016-01-03   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:39F91959416763AFD34DBEEC05474411B964B2DC)                                  |       0.62 |        15 | 2018-08-28   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                         |            4.319 |     15.92 |       0.67 |        61 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            2.083 |      5.36 |       1.19 |        20 | 2017-06-13   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:041646640AB306EA74B001966E86169B04CC88D2) |            1.729 |      7.08 |       0    |        23 | 2017-02-23   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |            1.553 |      6.36 |       0    |        17 | 2016-12-23   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:13E8EB1D9FD7470AA87A47DC93538E88340A0903)      |            0.898 |      1.04 |       0.87 |        20 | 2016-10-28   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.749 |      0    |       0.54 |        12 | 2018-01-31   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.717 |      0    |       1.11 |        19 | 2015-05-16   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.677 |      2.77 |       0    |        13 | 2015-05-22   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |            0.654 |      0    |       0.88 |         5 | 2016-09-06   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:3B4C5729F829CA2E895B81AF834A63DB336D0FFE)           |            0.538 |      0    |       0.83 |        13 | 2018-01-07   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                                                          |            14.19 |      17.06 |      9.66 |       588 |
| Hetzner Online GmbH                                              |            12.68 |      16.36 |      0.12 |       404 |
| Online S.a.s.                                                    |            10.86 |      13.67 |      5.3  |       332 |
| Joshua Peter McQuistan                                           |             4.22 |       0.53 |     15.87 |        48 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             1.97 |       1.02 |      5.36 |        17 |
| netcup GmbH                                                      |             1.75 |       2.1  |      0.18 |        74 |
| iomart Cloud Services Limited.                                   |             1.72 |       2.36 |      0    |        21 |
| Quintex Alliance Consulting                                      |             1.72 |       0    |      7.08 |        23 |
| DigitalOcean, LLC                                                |             1.64 |       1.55 |      1.33 |       230 |
| SURFnet bv                                                       |             1.63 |       1.45 |      2.8  |        26 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.5         |             40.5 |     47.09 |      38.39 |      2358 |
| 0.3.4         |             27.6 |     18.63 |      32.23 |      1560 |
| 0.2.9         |             10   |      5.95 |      10.57 |      1117 |
| 0.3.3         |              8.7 |     17.09 |       5.83 |       450 |
| 0.4.0         |              6.6 |      8.97 |       5.88 |       186 |
| 0.3.2         |              3.8 |      1.71 |       4.95 |       253 |
| 0.2.5         |              0.7 |      0.17 |       0.6  |       156 |
| 0.3.1         |              0.7 |      0.16 |       0.88 |        74 |
| 0.2.4         |              0.4 |      0.27 |       0.11 |       142 |
| 0.3.0         |              0.2 |      0    |       0.4  |        61 |
| 0.2.7         |              0.1 |      0.01 |       0.05 |        85 |
| 0.2.6         |              0   |      0    |       0.03 |        20 |
| 0.2.8         |              0   |      0.06 |       0.06 |        19 |
| 0.3.6         |              0   |      0    |       0    |         2 |
| 0.4.1         |              0   |      0    |       0.03 |         4 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             6.42 |       7.15 |      2.41 |       816 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.2 |      88.6 |       91.6 |      5935 |
| BSD     |              8.4 |      11.1 |        8.1 |       387 |
| Windows |              0.2 |       0.3 |        0   |        93 |
| Darwin  |              0   |       0   |        0   |        14 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            26.32 |      24.69 |       24.07 |     32.31 |       979 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     35.57 |            211 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       464 |
| None                                       |       390 |
| obfs3, obfs4                               |        54 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3, obfs4                        |         7 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         5 |
| obfs3, obfs4, scramblesuit                 |         3 |
| fte, meek, obfs3, obfs4                    |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| obfs2, obfs3                               |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

