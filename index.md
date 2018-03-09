---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-03-09 21:00 UTC**

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

| Contact                                                                                                        | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:---------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)           | 0.11        | 0.22       | 3         | 2               | 2016-08-28     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca) | 0.02        | 0.3        | 7         | 2               | 2018-02-11     | 4                           |
| **Total**                                                                                                      | **0.13**    | **0.52**   | **10**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |     14.08 |        26 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      5.3  |        13 | 2016-12-23   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)     |      3.12 |        11 | 2017-12-05   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.78 |         1 | 2014-04-19   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.6  |         7 | 2013-07-10   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      2.51 |         6 | 2017-11-29   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      2.28 |         7 | 2014-04-09   |
| [abuse aT nectodoT--onion](https://metrics.torproject.org/rs.html#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                                 |      2.01 |         6 | 2015-08-27   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      1.87 |         6 | 2014-04-08   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://metrics.torproject.org/rs.html#search/family:A10C4F666D27364036B562823E5830BC448E046A) |      1.67 |         5 | 2011-10-06   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.94 |         7 | 2014-04-22   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://metrics.torproject.org/rs.html#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)    |       1.25 |         5 | 2015-06-01   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       1.18 |         5 | 2017-10-24   |
| [info omuravpn.com](https://metrics.torproject.org/rs.html#search/family:94C0F99BA44AA4A6767C71333B8A66DBD1BC08C7)                                     |       1.1  |         5 | 2017-01-05   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |       1.02 |         6 | 2016-08-10   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:D6103DC78470C070840C74D0D1F41AEC3E5DE1B3)           |       1    |        10 | 2018-01-07   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       0.96 |        16 | 2015-10-10   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       0.91 |         3 | 2015-04-22   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://metrics.torproject.org/rs.html#search/family:B08E51FED96A7A7A6081ACC96299713F3F171B3A)            |       0.75 |         9 | 2017-02-08   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       0.75 |         6 | 2016-01-03   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            3.452 |     14.08 |       0    |        26 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |            1.298 |      5.3  |       0    |        13 | 2016-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            1.015 |      0    |       1.94 |         7 | 2014-04-22   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://metrics.torproject.org/rs.html#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)    |            0.895 |      0.97 |       1.25 |         8 | 2015-06-01   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |            0.766 |      3.12 |       0    |        11 | 2017-12-05   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |            0.719 |      2.51 |       0.19 |         8 | 2016-01-26   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.681 |      2.78 |       0    |         1 | 2014-04-19   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)           |            0.651 |      2.6  |       0    |         8 | 2013-07-10   |
| [tor-abuse&lt;at&gt;mailbox&lt;dot&gt;org](https://metrics.torproject.org/rs.html#search/family:5AE78E639DA2795C32EEE11CE5014546289777B8)              |            0.623 |      1.57 |       0.45 |         4 | 2017-12-20   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |            0.618 |      0    |       1.18 |         5 | 2017-10-24   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            14.81 |      20.32 |      7.1  |       508 |
| Online S.a.s.               |            10.12 |      12.53 |     10.79 |       366 |
| Hetzner Online GmbH         |             7.36 |       5.41 |      2.87 |       305 |
| DigitalOcean, LLC           |             5.79 |       8.01 |      2.48 |       304 |
| Host Europe GmbH            |             2.03 |       3.77 |      0    |        34 |
| SOFTplus Entwicklungen GmbH |             1.42 |       0.27 |      5.22 |        19 |
| NForce Entertainment B.V.   |             1.28 |       0.08 |      4.85 |        18 |
| THC Projects SRL            |             1.22 |       2.32 |      0    |        17 |
| Contabo GmbH                |             1.2  |       2.01 |      0.23 |        48 |
| SURFnet bv                  |             1.15 |       1.69 |      0.94 |        10 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             51.4 |     48.22 |      52.16 |      2461 |
| 0.3.3         |             13.8 |     25.3  |      13.31 |       352 |
| 0.2.9         |             13.5 |      9.24 |      13.14 |      1190 |
| 0.3.1         |             13.1 |     11.17 |      13.21 |       995 |
| 0.2.5         |              3.5 |      2.75 |       3.97 |       466 |
| 0.3.0         |              1.3 |      0.42 |       1.44 |       215 |
| 0.2.4         |              0.9 |      0.38 |       1.09 |       252 |
| 0.3.4         |              0.9 |      2.31 |       0.66 |        20 |
| 0.2.7         |              0.7 |      0.13 |       0.71 |       187 |
| 0.2.8         |              0.2 |      0.01 |       0.18 |        42 |
| 0.2.6         |              0.1 |      0    |       0.07 |        38 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.17 |       3.33 |      0.95 |       692 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.7 |      90.4 |       89.1 |      5741 |
| BSD     |              9   |       9.3 |       10.7 |       329 |
| Windows |              0.1 |       0   |        0   |       107 |
| Darwin  |              0   |       0   |        0   |         9 |
| SunOS   |              0   |       0   |        0   |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            21.26 |      21.25 |       18.51 |     25.49 |       702 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     30.69 |            157 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1035 |
| None                                       |       580 |
| obfs3, obfs4, scramblesuit                 |       245 |
| obfs3, obfs4                               |        55 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        18 |
| obfs2, obfs3                               |        10 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| meek                                       |         3 |
| scramblesuit                               |         3 |
| fte, obfs3, obfs4                          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| fte, scramblesuit                          |         1 |
| meek, meek                                 |         1 |
| meek, obfs4                                |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

