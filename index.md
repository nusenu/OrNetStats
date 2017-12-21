---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-12-21 11:00 UTC**

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

| Contact                                                                                                                                  | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-----------------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.16        | 0.17       | 4         | 3               | 2017-11-29     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb) | 0.08        | 0.86       | 13        | 2               | 2016-04-01     | 4                           |
| [https://www.torservers.net/donate.html &lt;support .A](endtoend-correlation-groups#httpswwwtorserversnetdonatehtml-support-a)           | 0.07        | 4.28       | 11        | 3               | 2017-11-01     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                                 | 0.06        | 0.03       | 3         | 3               | 2017-10-01     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.05        | 0.39       | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                                                | **0.42**    | **5.73**   | **33**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                               |   Exit(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |     10.3  |        24 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      5.65 |        12 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      3.74 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |      3.23 |        11 | 2017-12-05   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      3.05 |         5 | 2014-04-09   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.46 |         3 | 2014-11-04   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      2.35 |         6 | 2014-04-08   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.09 |         8 | 2013-07-10   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                                 |      1.93 |         6 | 2015-08-27   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://atlas.torproject.org/#search/family:A10C4F666D27364036B562823E5830BC448E046A) |      1.89 |         5 | 2011-10-06   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                                 |       1.85 |         8 | 2016-07-26   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       1.64 |        16 | 2015-10-10   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       1.36 |         7 | 2016-08-10   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:951950A7993CF8A8E05174CF293BE4EA4DEFFF28)                                    |       1.03 |        17 | 2014-12-31   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       1.02 |         6 | 2014-04-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       0.94 |         7 | 2016-01-03   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://atlas.torproject.org/#search/family:F596E1B1EF98E1DDBBDC934DB722AF54069868F6) |       0.86 |         7 | 2014-04-09   |
| [info omuravpn.com](https://atlas.torproject.org/#search/family:94C0F99BA44AA4A6767C71333B8A66DBD1BC08C7)                                        |       0.71 |         6 | 2017-01-05   |
| [Random Person &lt;nobody AT example dot com&gt;](https://atlas.torproject.org/#details/85F277DFE886353598A51D3CAB04DD3F6EBB427D)                |       0.66 |         1 | 2017-12-09   |
| [0x7A8647DB Daniel Winzen &lt;d@winzen4.de&gt; - 1CHvjeMJ](https://atlas.torproject.org/#search/family:72B19BAABE6846DF96EA2A50C28F4DC15A920041) |       0.64 |         5 | 2017-04-09   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                               |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |            2.496 |     10.3  |       0.09 |        28 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |            1.335 |      5.65 |       0    |        12 | 2016-12-23   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                                 |            0.908 |      0    |       1.85 |         8 | 2016-07-26   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |            0.884 |      3.74 |       0    |         1 | 2014-04-19   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |            0.808 |      0    |       1.64 |        17 | 2015-10-10   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |            0.765 |      3.23 |       0    |        11 | 2017-12-05   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.728 |      0.25 |       1.36 |         8 | 2016-08-10   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |            0.72  |      3.05 |       0    |         5 | 2014-04-09   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://atlas.torproject.org/#search/family:A10C4F666D27364036B562823E5830BC448E046A) |            0.654 |      1.89 |       0.42 |         8 | 2010-02-17   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |            0.618 |      0    |       1.02 |         7 | 2014-04-22   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            15.5  |      16.6  |      5.91 |       518 |
| Online S.a.s.               |            10.77 |      12.6  |     12    |       395 |
| Hetzner Online GmbH         |             7.6  |       9.38 |      2    |       295 |
| DigitalOcean, LLC           |             4.45 |       5.58 |      1.46 |       308 |
| Host Europe GmbH            |             2.9  |       4.13 |      0    |        47 |
| THC Projects SRL            |             1.6  |       3.25 |      0    |        21 |
| myLoc managed IT AG         |             1.27 |       1.99 |      0.46 |        42 |
| SOFTplus Entwicklungen GmbH |             1.23 |       0.06 |      4.88 |        18 |
| SURFnet bv                  |             1.11 |       0.32 |      0.78 |        13 |
| Contabo GmbH                |             0.96 |       1.61 |      0.53 |        50 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             57.4 |     61.47 |      56.1  |      2843 |
| 0.2.9         |             14.8 |     10.48 |      15.17 |      1290 |
| 0.3.0         |              9.1 |      5.92 |       9.19 |       504 |
| 0.3.2         |              8   |     14.62 |       7.12 |       267 |
| 0.2.5         |              5.3 |      3.94 |       6.92 |       607 |
| 0.2.7         |              1.8 |      0.4  |       2.23 |       288 |
| 0.2.4         |              1.3 |      0.27 |       1.69 |       312 |
| 0.3.3         |              1   |      2.5  |       0.24 |        14 |
| 0.2.8         |              0.7 |      0.24 |       0.9  |        83 |
| 0.2.6         |              0.3 |      0.12 |       0.39 |        55 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.51 |       4.32 |       0.8 |       655 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.9 |      88.8 |       92   |      5797 |
| BSD     |              8.6 |      11   |        7.6 |       310 |
| Windows |              0.1 |       0   |        0   |       119 |
| SunOS   |              0.1 |       0   |        0.2 |         4 |
| Darwin  |              0   |       0   |        0   |        14 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.43 |      18.15 |       14.14 |     25.83 |       582 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     31.62 |            130 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1176 |
| None                                       |       600 |
| obfs3, obfs4, scramblesuit                 |       191 |
| obfs3, obfs4                               |        62 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        19 |
| obfs2, obfs3                               |         9 |
| obfs3, scramblesuit                        |         9 |
| obfs2, obfs3, obfs4                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| fte, obfs3, obfs4                          |         4 |
| obfs2, obfs3, obfs4, scramblesuit          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| meek                                       |         1 |
| meek, obfs4                                |         1 |
| scramblesuit                               |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

