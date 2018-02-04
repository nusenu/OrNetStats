---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-02-04 14:00 UTC**

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

| Contact                                                                                                                              | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-------------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [abuse AT torworld.org - BTC 17iwdtpmgHdPt15twdT2](endtoend-correlation-groups#abuse-at-torworldorg---btc-17iwdtpmghdpt15twdt2)      | 0.41        | 0.83       | 10        | 7               | 2018-01-23     | 8                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                 | 0.13        | 0.23       | 3         | 2               | 2016-08-28     | 1                           |
| [oliver.farnan@cs.ox.ac.uk](endtoend-correlation-groups#oliverfarnancsoxacuk)                                                        | 0.07        | 0.01       | 2         | 2               | 2018-02-02     | 1                           |
| [ninja.turtle5@aol.com](endtoend-correlation-groups#ninjaturtle5aolcom)                                                              | 0.03        | 0.05       | 4         | 2               | 2018-01-30     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                             | 0.02        | 0.02       | 3         | 3               | 2017-10-01     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv) | 0.02        | 0.1        | 3         | 3               | 2018-01-21     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                         | 0.01        | 0.3        | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                                            | **0.69**    | **1.54**   | **27**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                            |   Exit(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |     13    |        33 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |      5.31 |        12 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |      3.22 |        11 | 2017-12-05   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.96 |         1 | 2014-04-19   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |      2.95 |        10 | 2017-11-29   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)           |      2.26 |         7 | 2013-07-10   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |      2.15 |         5 | 2014-04-09   |
| [John Doe johndoe@novogara.com](https://atlas.torproject.org/#details/0593F5255316748247EBA76353A3A61F62224903)                               |      2.14 |         1 | 2017-09-05   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C) |      1.98 |         6 | 2014-04-08   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                              |      1.9  |         5 | 2015-08-27   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [0ED0EA32](https://atlas.torproject.org/#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       2.31 |         5 | 2017-10-24   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |       2.22 |         6 | 2016-08-10   |
| [god AT universe.org](https://atlas.torproject.org/#search/family:F3CEC87ED91E0B0B1D86BE4D7DE90F00B607ECAF)                                   |       1.27 |         2 | 2016-10-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.2  |         2 | 2015-04-22   |
| [poiuty@protonmail.com - 1YWqF3SGnQMkwgfGasrNmYv1XG](https://atlas.torproject.org/#search/family:CFEC9600E877776982C3161B6A98812871F2A07F)    |       1.19 |         3 | 2016-01-26   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       1.08 |        12 | 2015-10-10   |
| [&lt;roottor00@multivac.io&gt; - 1LLnvMu2s4BaF2LmsqV8Ruw](https://atlas.torproject.org/#details/1C90D3AEADFF3BCD079810632C8B85637924A58E)     |       0.9  |         1 | 2014-04-08   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       0.9  |         5 | 2014-04-22   |
| [0x9501B909 Random Person &lt;deep.thought AT riseup d](https://atlas.torproject.org/#search/family:3F39BC367D7FCF3F631C49190F4D0C4312307A8F) |       0.79 |         7 | 2017-02-20   |
| [Anders Burmeister &lt;anders.burmeister AT protonmail](https://atlas.torproject.org/#search/family:92412EA1B9AA887D462B51D816777002F4D58907) |       0.75 |         6 | 2017-02-11   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            3.554 |     13    |       0    |        33 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |            1.452 |      5.31 |       0    |        12 | 2016-12-23   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |            1.109 |      0.37 |       2.22 |         7 | 2016-08-10   |
| [0ED0EA32](https://atlas.torproject.org/#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |            1.044 |      0    |       2.31 |         5 | 2017-10-24   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.916 |      2.95 |       0.24 |        12 | 2016-01-26   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |            0.881 |      3.22 |       0    |        11 | 2017-12-05   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.811 |      2.96 |       0    |         1 | 2014-04-19   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.769 |      0    |       1.2  |         3 | 2015-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.714 |      0    |       1.08 |        19 | 2015-05-16   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://atlas.torproject.org/#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)    |            0.662 |      1.26 |       0.22 |         7 | 2015-06-01   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            16.73 |      24.66 |      7.17 |       502 |
| Online S.a.s.               |             9.85 |      10.67 |     11.43 |       386 |
| Hetzner Online GmbH         |             7.03 |       8.09 |      1.29 |       299 |
| DigitalOcean, LLC           |             4.23 |       6.02 |      1.36 |       305 |
| SOFTplus Entwicklungen GmbH |             1.53 |       0.24 |      5.07 |        19 |
| Host Europe GmbH            |             1.48 |       0.96 |      0    |        31 |
| SURFnet bv                  |             1.47 |       1.75 |      1.06 |        12 |
| NForce Entertainment B.V.   |             1.37 |       0.05 |      4.58 |        16 |
| Voxility S.R.L.             |             1.22 |       0.48 |      3.1  |        16 |
| myLoc managed IT AG         |             1.01 |       1.74 |      0.36 |        37 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             43.3 |     56.74 |      39.2  |      2099 |
| 0.3.1         |             26.4 |     19.56 |      29.04 |      1487 |
| 0.2.9         |             12.5 |      9.45 |      13.06 |      1174 |
| 0.2.5         |              5   |      3.56 |       5.02 |       513 |
| 0.3.3         |              5   |      4.97 |       5.22 |       113 |
| 0.3.0         |              3.9 |      3.77 |       4.05 |       303 |
| 0.2.4         |              1.7 |      1.18 |       2.48 |       270 |
| 0.2.7         |              1.5 |      0.32 |       1.68 |       241 |
| 0.2.8         |              0.2 |      0.3  |       0.06 |        41 |
| 0.2.6         |              0.1 |      0.06 |       0.11 |        38 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             7.38 |       8.34 |      5.35 |       852 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             89.7 |      91.2 |       89.4 |      5831 |
| BSD     |              9.8 |       8.6 |       10.2 |       287 |
| Windows |              0.1 |       0   |        0   |       123 |
| SunOS   |              0.1 |       0   |        0.2 |         4 |
| Darwin  |              0   |       0   |        0   |         8 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|             19.8 |      21.17 |       17.01 |     21.69 |       617 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|      26.8 |            147 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1093 |
| None                                       |       591 |
| obfs3, obfs4, scramblesuit                 |       246 |
| obfs3, obfs4                               |        55 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        18 |
| obfs2, obfs3                               |        10 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs3, scramblesuit                        |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         3 |
| scramblesuit                               |         3 |
| fte, obfs3, obfs4                          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| meek, obfs4                                |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

