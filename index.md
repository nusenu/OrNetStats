---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2019-03-31 07:00 UTC**

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

| Contact                                                                                                   | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:----------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain) | 0.11        | 0.1        | 6         | 6               | 2018-12-23     | 1                           |
| [Jelle Jansen &lt;tormail@gigawebs.net&gt;](endtoend-correlation-groups#jelle-jansen-tormailgigawebsnet)  | 0.03        | 0.01       | 4         | 4               | 2019-01-09     | 2                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)      | 0.02        | 0.09       | 3         | 2               | 2016-08-28     | 1                           |
| [DuckSounds31@aol.com](endtoend-correlation-groups#ducksounds31aolcom)                                    | 0.01        | 0.02       | 4         | 4               | 2018-03-02     | 2                           |
| **Total**                                                                                                 | **0.17**    | **0.22**   | **17**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0B3C8C2B2B1A1CA4429B9649F533BEB4D7470AEA)                         |     13.22 |        44 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |      6.3  |        17 | 2016-12-23   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |      6.09 |         9 | 2018-04-05   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:041646640AB306EA74B001966E86169B04CC88D2) |      5.02 |        26 | 2017-02-23   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      2.64 |        13 | 2015-05-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.29 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      1.95 |        12 | 2017-12-05   |
| [tor-operator@privateinternetaccess.com](https://metrics.torproject.org/rs.html#search/family:3F62F05E859D7F98B086F702A31F7714D566E49A)                |      1.62 |         5 | 2018-12-11   |
| [18CFB7BA](https://metrics.torproject.org/rs.html#search/family:18CFB7BA07F13AEABF50A7148786DA68773B2498)                                              |      1.61 |         2 | 2018-12-15   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      1.48 |         4 | 2014-11-21   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                 |   Guard(%) |   #Relays | First Seen   |
|:---------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)     |       1.14 |        19 | 2015-05-16   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)               |       1.11 |        11 | 2018-01-31   |
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                     |       1.04 |        17 | 2019-01-05   |
| [email:tor appliedprivacy.net twitter:applied priv](https://metrics.torproject.org/rs.html#search/family:113143469021882C3A4B82F084F8125B08EE471E) |       0.93 |        10 | 2017-06-13   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                          |       0.83 |         4 | 2018-08-17   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:3B4C5729F829CA2E895B81AF834A63DB336D0FFE)       |       0.77 |        13 | 2018-01-07   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)  |       0.75 |        14 | 2016-12-11   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                          |       0.66 |         5 | 2017-10-24   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:39F91959416763AFD34DBEEC05474411B964B2DC)                              |       0.65 |        16 | 2018-08-28   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)               |       0.63 |         3 | 2015-04-22   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:0677DF0B05ECDA2EF45F26C3332731043BB89AB8)                         |            3.921 |     13.22 |       1.04 |        61 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            2.1   |      6.09 |       0.93 |        19 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |            1.546 |      6.3  |       0    |        17 | 2016-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:041646640AB306EA74B001966E86169B04CC88D2) |            1.232 |      5.02 |       0    |        26 | 2017-02-23   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:13E8EB1D9FD7470AA87A47DC93538E88340A0903)      |            0.821 |      1.01 |       0.75 |        19 | 2016-10-28   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.744 |      0    |       1.14 |        19 | 2015-05-16   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.724 |      0    |       1.11 |        11 | 2018-01-31   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.647 |      2.64 |       0    |        13 | 2015-05-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.559 |      2.29 |       0    |         1 | 2014-04-19   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                              |            0.54  |      0    |       0.83 |         4 | 2018-08-17   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| Hetzner Online GmbH                                              |            13.85 |      18.13 |      0.13 |       420 |
| OVH SAS                                                          |            13.3  |      16.71 |      7.84 |       567 |
| Online S.a.s.                                                    |            11.2  |      12.91 |      6.39 |       319 |
| Joshua Peter McQuistan                                           |             3.33 |       0.14 |     13.22 |        46 |
| netcup GmbH                                                      |             2.05 |       2.17 |      0.66 |        77 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             2.01 |       0.8  |      6.09 |        17 |
| iomart Cloud Services Limited.                                   |             1.93 |       2.98 |      0    |        19 |
| NForce Entertainment B.V.                                        |             1.68 |       1.21 |      3.35 |        32 |
| myLoc managed IT AG                                              |             1.53 |       1.89 |      0.28 |        37 |
| SURFnet bv                                                       |             1.5  |       1.26 |      2.75 |        26 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.5         |             53.9 |     70.5  |      47.43 |      3066 |
| 0.3.4         |             20.5 |      8.93 |      26.43 |      1057 |
| 0.2.9         |              9.6 |      5.43 |      10.16 |      1071 |
| 0.4.0         |              6.6 |     10.08 |       5.73 |       184 |
| 0.3.2         |              3.2 |      1.8  |       4.03 |       236 |
| 0.3.3         |              3   |      1.72 |       3.59 |       290 |
| 0.4.1         |              0.9 |      0.87 |       1.13 |        20 |
| 0.2.5         |              0.5 |      0.23 |       0.28 |       146 |
| 0.3.1         |              0.5 |      0.2  |       0.75 |        73 |
| 0.2.4         |              0.3 |      0.22 |       0.14 |       135 |
| 0.2.7         |              0.2 |      0    |       0.03 |        75 |
| 0.3.0         |              0.1 |      0    |       0.14 |        57 |
| 0.2.6         |              0   |      0    |       0.02 |        24 |
| 0.2.8         |              0   |      0    |       0.05 |        23 |
| 0.3.6         |              0   |      0    |       0    |         2 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             8.22 |       9.09 |      4.18 |      1061 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.9 |      86.7 |       92   |      5949 |
| BSD     |              8.7 |      13.1 |        7.6 |       383 |
| Windows |              0.1 |       0.1 |        0.1 |        82 |
| Darwin  |              0   |       0   |        0   |        14 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            26.84 |      24.68 |       24.65 |     33.55 |       984 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     34.71 |            215 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       448 |
| None                                       |       392 |
| obfs3, obfs4                               |        55 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3                                      |         6 |
| meek                                       |         5 |
| obfs3, obfs4, scramblesuit                 |         5 |
| fte, meek, obfs3, obfs4                    |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, obfs3                                 |         1 |
| fte, obfs3, obfs4, scramblesuit            |         1 |
| fte, obfs3, obfs4, scramblesuit, websocket |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| marionette                                 |         1 |
| meek, meek                                 |         1 |
| obfs2, obfs3                               |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

