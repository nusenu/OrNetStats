---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-03-12 11:00 UTC**

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

| Contact                                                                                                                       | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                          | 0.08        | 0.33       | 3         | 2               | 2016-08-28     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                | 0.05        | 0.45       | 7         | 2               | 2018-02-11     | 4                           |
| [http://tor.jonny.mobi &lt;torsupport .AT. jonny .DOT.](endtoend-correlation-groups#httptorjonnymobi-torsupport-at-jonny-dot) | 0.03        | 0.18       | 7         | 2               | 2018-03-02     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                  | 0.01        | 0.31       | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                                     | **0.17**    | **1.27**   | **19**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |     13.72 |        26 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |      6.19 |        13 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      3.22 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |      3.12 |        11 | 2017-12-05   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |      2.38 |         7 | 2014-04-09   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)            |      2.1  |         6 | 2017-11-29   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)           |      2.1  |         7 | 2013-07-10   |
| [abuse aT nectodoT--onion](https://metrics.torproject.org/rs.html#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                              |      2.09 |         6 | 2015-08-27   |
| [Datashield, Inc. abuse@xor.sc](https://metrics.torproject.org/rs.html#details/D8FF84E5E29A92F09F8263D4662627ECC479B108)                               |      1.82 |         1 | 2018-02-24   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:9BA84E8C90083676F86C7427C8D105925F13716C) |      1.79 |         6 | 2014-04-08   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.75 |         7 | 2014-04-22   |
| [33b pm.me](https://metrics.torproject.org/rs.html#search/family:CAE7A1CD26DCA17DDAB0BFA3DA11DFE4D5020537)                                             |       1.7  |         8 | 2015-10-19   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       1.19 |         5 | 2017-10-24   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       1.15 |         7 | 2016-01-03   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |       1.15 |         6 | 2016-08-10   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://metrics.torproject.org/rs.html#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)    |       1.14 |         5 | 2015-06-01   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:D6103DC78470C070840C74D0D1F41AEC3E5DE1B3)           |       1.02 |        10 | 2018-01-07   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.01 |         3 | 2015-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       1    |        16 | 2015-10-10   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://metrics.torproject.org/rs.html#search/family:B08E51FED96A7A7A6081ACC96299713F3F171B3A)            |       0.75 |         9 | 2017-02-08   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            3.447 |     13.72 |       0    |        26 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55) |            1.556 |      6.19 |       0    |        13 | 2016-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.931 |      0    |       1.75 |         7 | 2014-04-22   |
| [33b pm.me](https://metrics.torproject.org/rs.html#search/family:CAE7A1CD26DCA17DDAB0BFA3DA11DFE4D5020537)                                             |            0.906 |      0    |       1.7  |         8 | 2015-10-19   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://metrics.torproject.org/rs.html#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)    |            0.834 |      0.89 |       1.14 |         8 | 2015-06-01   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.81  |      3.22 |       0    |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:8D093C9C2B42BC224A5319A660A6CF5EDEFE839F)  |            0.784 |      3.12 |       0    |        11 | 2017-12-05   |
| [tor-abuse&lt;at&gt;mailbox&lt;dot&gt;org](https://metrics.torproject.org/rs.html#search/family:5AE78E639DA2795C32EEE11CE5014546289777B8)              |            0.681 |      1.65 |       0.5  |         4 | 2017-12-20   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)      |            0.638 |      0.1  |       1.15 |         7 | 2016-08-10   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |            0.632 |      0    |       1.19 |         5 | 2017-10-24   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            14.27 |      19.34 |      7.22 |       512 |
| Online S.a.s.               |            10.98 |      14.08 |     10.55 |       370 |
| Hetzner Online GmbH         |             6.7  |       5.25 |      2.86 |       305 |
| DigitalOcean, LLC           |             6.24 |       7.72 |      2.62 |       308 |
| Host Europe GmbH            |             1.86 |       3.37 |      0.01 |        36 |
| NForce Entertainment B.V.   |             1.56 |       0.07 |      5.87 |        19 |
| SOFTplus Entwicklungen GmbH |             1.26 |       0.17 |      4.66 |        18 |
| THC Projects SRL            |             1.22 |       2.3  |      0    |        17 |
| SURFnet bv                  |             1.22 |       1.77 |      1.11 |         9 |
| Contabo GmbH                |             1.21 |       2.01 |      0.21 |        46 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.2         |             52.3 |     47.63 |      53.95 |      2524 |
| 0.3.3         |             14.1 |     26.13 |      13.15 |       353 |
| 0.2.9         |             13.1 |      9.53 |      12.41 |      1187 |
| 0.3.1         |             12.5 |     10.1  |      12.45 |       918 |
| 0.2.5         |              3.5 |      2.84 |       3.85 |       472 |
| 0.3.0         |              1.1 |      0.27 |       1.58 |       212 |
| 0.2.4         |              1   |      0.58 |       1.1  |       254 |
| 0.3.4         |              1   |      2.69 |       0.48 |        21 |
| 0.2.7         |              0.7 |      0.14 |       0.69 |       187 |
| 0.2.8         |              0.2 |      0.03 |       0.19 |        38 |
| 0.2.6         |              0   |      0.01 |       0.09 |        37 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.02 |       3.47 |      1.01 |       690 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.1 |      89.9 |       88.2 |      5732 |
| BSD     |              9.5 |       9.9 |       11.5 |       325 |
| Windows |              0.1 |       0   |        0   |       104 |
| Darwin  |              0   |       0   |        0   |        11 |
| SunOS   |              0   |       0   |        0.1 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            21.23 |      21.87 |       17.05 |     26.48 |       694 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     32.05 |            152 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1014 |
| None                                       |       587 |
| obfs3, obfs4, scramblesuit                 |       245 |
| obfs3, obfs4                               |        54 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        18 |
| obfs2, obfs3                               |        10 |
| obfs2, obfs3, obfs4                        |         7 |
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

