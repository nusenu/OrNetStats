---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-12-02 07:00 UTC**

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
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb) | 0.1         | 0.7        | 13        | 2               | 2016-04-01     | 4                           |
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.09        | 0.02       | 5         | 5               | 2017-11-29     | 1                           |
| [abuse AT torworld.org - BTC 17iwdtpmgHdPt15twdT2](endtoend-correlation-groups#abuse-at-torworldorg---btc-17iwdtpmghdpt15twdt2)          | 0.08        | 0.24       | 5         | 3               | 2017-12-01     | 2                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                                 | 0.04        | 0.03       | 3         | 3               | 2017-10-01     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.04        | 0.35       | 2         | 2               | 2017-02-16     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                           | 0.03        | 0.83       | 5         | 2               | 2017-06-23     | 1                           |
| **Total**                                                                                                                                | **0.38**    | **2.17**   | **33**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      7.49 |        20 | 2016-01-25   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)       |      5.42 |         9 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      3.84 |         1 | 2014-04-19   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      2.56 |         5 | 2014-04-09   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      2.52 |         6 | 2014-04-08   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                                 |      2.21 |         6 | 2015-08-27   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://atlas.torproject.org/#search/family:9AA3FF35E7A549D2337E962333D366E102FE4D50)              |      2.18 |         8 | 2013-07-10   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://atlas.torproject.org/#search/family:A10C4F666D27364036B562823E5830BC448E046A) |      2.13 |         5 | 2011-10-06   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                    |      2    |         6 | 2016-04-02   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://atlas.torproject.org/#search/family:7016E939A2DD6EF2FB66A33F1DD45357458B737F)    |      1.98 |         8 | 2014-04-16   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                                 |       2.14 |         8 | 2016-07-26   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       1.28 |         7 | 2014-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)            |       1.11 |         7 | 2016-08-10   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                      |       1.1  |         3 | 2015-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                    |       0.99 |        26 | 2014-12-31   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       0.92 |        20 | 2015-05-16   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       0.82 |         7 | 2016-01-03   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://atlas.torproject.org/#search/family:F596E1B1EF98E1DDBBDC934DB722AF54069868F6) |       0.76 |         7 | 2014-04-09   |
| [0ED0EA32](https://atlas.torproject.org/#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                                 |       0.64 |         5 | 2017-10-24   |
| [info omuravpn.com](https://atlas.torproject.org/#search/family:94C0F99BA44AA4A6767C71333B8A66DBD1BC08C7)                                        |       0.64 |         5 | 2017-01-05   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                               |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |            1.579 |      7.49 |       0.34 |        28 | 2016-01-25   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                                 |            1.347 |      0    |       2.14 |         8 | 2016-07-26   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)       |            0.987 |      5.42 |       0    |         9 | 2016-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |            0.804 |      0    |       1.28 |         7 | 2014-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)            |            0.756 |      0.33 |       1.11 |         8 | 2016-08-10   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |            0.699 |      3.84 |       0    |         1 | 2014-04-19   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                      |            0.689 |      0    |       1.1  |         3 | 2015-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                    |            0.652 |      0    |       0.99 |        28 | 2014-12-31   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://atlas.torproject.org/#search/family:F596E1B1EF98E1DDBBDC934DB722AF54069868F6) |            0.602 |      0    |       0.76 |        10 | 2014-04-09   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |            0.588 |      0    |       0.92 |        21 | 2015-05-16   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [Germany](https://atlas.torproject.org/#search/country:de)        |            23.74 |      26.44 |      7.37 |      1347 |
| [France](https://atlas.torproject.org/#search/country:fr)         |            23.28 |      25.74 |     21.05 |       902 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            10.39 |      10.54 |     11.87 |       481 |
| [United States](https://atlas.torproject.org/#search/country:us)  |             9.57 |       7.59 |     13.87 |      1127 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             4.45 |       4.08 |      6.63 |       280 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.64 |       1.82 |      7.69 |       192 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.92 |       2.57 |      4.49 |       106 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             2.82 |       2.71 |      3.75 |       226 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.51 |       2.44 |      3.03 |       138 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             1.82 |       1.77 |      0.52 |       291 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name             |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS             |            16.17 |      19.21 |      9.45 |       570 |
| Online S.a.s.       |            12.98 |      14.35 |     14.91 |       428 |
| Hetzner Online GmbH |             9.94 |      10.11 |      1.66 |       339 |
| DigitalOcean, LLC   |             5.36 |       5.89 |      1.69 |       362 |
| Host Europe GmbH    |             3.09 |       4.51 |      0    |        51 |
| myLoc managed IT AG |             1.6  |       2.29 |      0.5  |        42 |
| THC Projects SRL    |             1.38 |       2.01 |      0    |        25 |
| SURFnet bv          |             1.35 |       1.76 |      1.31 |        12 |
| Contabo GmbH        |             1.29 |       1.69 |      0.56 |        52 |
| Linode, LLC         |             1.02 |       0.23 |      1.52 |       217 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             49.4 |     48.88 |      48.69 |      2650 |
| 0.2.9         |             15.7 |     13.26 |      14.99 |      1398 |
| 0.3.0         |             15.5 |     15.58 |      17.74 |       779 |
| 0.2.5         |              6.7 |      4.77 |       7.14 |       718 |
| 0.3.2         |              6.6 |     15.33 |       5.14 |       225 |
| 0.2.7         |              2.4 |      0.26 |       2.62 |       346 |
| 0.2.4         |              1.5 |      0.12 |       1.69 |       330 |
| 0.2.8         |              1   |      0    |       1.16 |        99 |
| 0.2.6         |              0.4 |      0.11 |       0.61 |        62 |
| 0.3.3         |              0.4 |      1.64 |       0.15 |        10 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             4.47 |       4.94 |       0.5 |       738 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.4 |      89.1 |       91.9 |      6147 |
| BSD     |              7.1 |      10.8 |        7.7 |       318 |
| Windows |              0.1 |       0   |        0   |       128 |
| SunOS   |              0.1 |       0   |        0.2 |         4 |
| Darwin  |              0   |       0   |        0   |        11 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            19.55 |       18.7 |       17.45 |     26.16 |       605 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     32.52 |            118 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1119 |
| None                                       |       535 |
| obfs3, obfs4, scramblesuit                 |       187 |
| obfs3, obfs4                               |        52 |
| obfs3                                      |        17 |
| obfs3, scramblesuit                        |         8 |
| obfs2, obfs3                               |         7 |
| obfs2, obfs3, obfs4                        |         6 |
| fte, obfs3, obfs4                          |         4 |
| meek                                       |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, obfs4, scramblesuit, websocket |         1 |
| obfs4, scramblesuit                        |         1 |
| scramblesuit                               |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

