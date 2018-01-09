---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-01-09 07:00 UTC**

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
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-btc---14w) | 0.12        | 0.85       | 11        | 2               | 2016-04-01     | 4                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.06        | 0.31       | 2         | 2               | 2017-02-16     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                                 | 0.01        | 0.03       | 3         | 3               | 2017-10-01     | 1                           |
| **Total**                                                                                                                                | **0.19**    | **1.19**   | **16**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |     11.99 |        27 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |      5.74 |        12 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      3.51 |         1 | 2014-04-19   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      2.79 |         9 | 2016-08-26   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.43 |         3 | 2014-11-04   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.33 |         7 | 2013-07-10   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      2.31 |         5 | 2014-04-09   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      2.2  |         6 | 2014-04-08   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://atlas.torproject.org/#search/family:A10C4F666D27364036B562823E5830BC448E046A) |      1.98 |         5 | 2011-10-06   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                                 |      1.88 |         6 | 2015-08-27   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                         |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799) |       2.31 |         7 | 2014-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)      |       1.92 |        16 | 2015-10-10   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)   |       1.15 |         7 | 2016-08-10   |
| [Servbr Admin &lt;servbr AT mail DOT md&gt;](https://atlas.torproject.org/#search/family:B08E51FED96A7A7A6081ACC96299713F3F171B3A)         |       1.09 |        11 | 2016-04-10   |
| [poiuty@protonmail.com - 1YWqF3SGnQMkwgfGasrNmYv1XG](https://atlas.torproject.org/#search/family:CFEC9600E877776982C3161B6A98812871F2A07F) |       1.06 |         3 | 2016-01-26   |
| [poiuty@protonmail.com - 1YWqF3SGnQMkwgfGasrNmYv1XG](https://atlas.torproject.org/#details/B42AAFC99176BFDA23033191A9F6A7CCFE9F30EA)       |       0.94 |         1 | 2017-12-22   |
| [Alexander K?hrmann &lt;mail att kuehrmann.de&gt;](https://atlas.torproject.org/#details/DBE82FA23B9FE3CB2462A6FCF5289DED3CBF4AEE)         |       0.86 |         1 | 2016-12-16   |
| [0xF771597D61F018F5 &lt;jon DOT amund02 AT gmail dot c](https://atlas.torproject.org/#details/7F2C51C5FE4249CE32E023105D37C1E6B85B2311)    |       0.77 |         1 | 2017-06-10   |
| [&lt;roottor00@splitdna.com&gt; - 1LLnvMu2s4BaF2LmsqV8Ru](https://atlas.torproject.org/#details/1C90D3AEADFF3BCD079810632C8B85637924A58E)  |       0.73 |         1 | 2014-04-08   |
| [73834839](https://atlas.torproject.org/#details/73834839EDF6D650B94A7766BF1FE573BC06F5A1)                                                 |       0.68 |         1 | 2017-12-18   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                               |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |            2.797 |     11.99 |       0    |        27 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)    |            1.339 |      5.74 |       0    |        12 | 2016-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |            1.061 |      0    |       2.31 |         7 | 2014-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |            0.904 |      0    |       1.92 |        19 | 2015-05-16   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://atlas.torproject.org/#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |            0.839 |      2.79 |       0.4  |        12 | 2016-01-26   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |            0.82  |      3.51 |       0    |         1 | 2014-04-19   |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](https://atlas.torproject.org/#search/family:98D10461F6EDF13780D20D7E402E67F40C5ADBD9)       |            0.713 |      1.13 |       0.25 |         6 | 2015-06-01   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://atlas.torproject.org/#search/family:A10C4F666D27364036B562823E5830BC448E046A) |            0.708 |      1.98 |       0.53 |         8 | 2010-02-17   |
| [https://onioncount.github.io/ https://onionpop.g](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.649 |      0.52 |       1.15 |         8 | 2016-08-10   |
| [0ED0EA32](https://atlas.torproject.org/#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                                 |            0.631 |      0    |       0    |         5 | 2017-10-24   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                   |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                   |            16.28 |      17.91 |      8.82 |       512 |
| Online S.a.s.             |             9.65 |      10.94 |     11.94 |       371 |
| Hetzner Online GmbH       |             7.22 |       8.38 |      0.94 |       292 |
| DigitalOcean, LLC         |             5.4  |       6.27 |      1.62 |       306 |
| Host Europe GmbH          |             2.9  |       4.06 |      0    |        43 |
| THC Projects SRL          |             1.44 |       1.98 |      0    |        22 |
| myLoc managed IT AG       |             1.38 |       2.12 |      0.65 |        42 |
| ISPpro Internet KG        |             1.11 |       2.15 |      0    |        29 |
| NForce Entertainment B.V. |             1.01 |       0    |      4.04 |        16 |
| Voxility S.R.L.           |             0.95 |       0.2  |      2.51 |        18 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             55.8 |     51.49 |      57.82 |      2849 |
| 0.2.9         |             14.4 |     10.3  |      15.27 |      1277 |
| 0.3.2         |             12.9 |     27    |      10.74 |       375 |
| 0.3.0         |              6.9 |      3.69 |       6.06 |       403 |
| 0.2.5         |              4.8 |      4.22 |       5.17 |       563 |
| 0.2.7         |              1.9 |      0.37 |       2    |       280 |
| 0.2.4         |              1.7 |      0.05 |       2.22 |       277 |
| 0.3.3         |              0.9 |      2.48 |       0.34 |        18 |
| 0.2.8         |              0.2 |      0.3  |       0.24 |        53 |
| 0.2.6         |              0.1 |      0.03 |       0.08 |        45 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.71 |       4.31 |      0.47 |       602 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.4 |      90.5 |       92.2 |      5710 |
| BSD     |              9.3 |       9.4 |        7.5 |       301 |
| Windows |              0.1 |       0   |        0   |       102 |
| Darwin  |              0   |       0   |        0   |        11 |
| SunOS   |              0   |       0   |        0.1 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.78 |      20.45 |       12.03 |     27.12 |       591 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|      32.7 |            139 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1104 |
| None                                       |       608 |
| obfs3, obfs4, scramblesuit                 |       247 |
| obfs3, obfs4                               |        61 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        18 |
| obfs2, obfs3                               |        10 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3, scramblesuit                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| scramblesuit                               |         3 |
| meek                                       |         2 |
| obfs2, obfs3, obfs4, scramblesuit          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, obfs4                          |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| meek, obfs4                                |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

