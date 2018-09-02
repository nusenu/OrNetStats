---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-09-02 07:00 UTC**

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
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca) | 0.08        | 0.41       | 7         | 2               | 2018-02-11     | 5                           |
| [abuse-node49 AT posteo DOT de](endtoend-correlation-groups#abuse-node49-at-posteo-dot-de)                     | 0.06        | 0.52       | 6         | 6               | 2018-08-30     | 2                           |
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)      | 0.02        | 0.1        | 3         | 3               | 2018-08-15     | 1                           |
| [DuckSounds31@aol.com](endtoend-correlation-groups#ducksounds31aolcom)                                         | 0.01        | 0.05       | 3         | 3               | 2018-03-02     | 1                           |
| **Total**                                                                                                      | **0.17**    | **1.08**   | **19**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |     11.85 |        27 | 2016-01-25   |
| [Relay Control &lt;office AT universalipsolution dot b](https://metrics.torproject.org/rs.html#search/family:0C2D910C87E9197878C005021E8BF4D2AF0FF17C)    |      2.89 |        20 | 2018-07-10   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      2.77 |         9 | 2015-05-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)      |      2.61 |         7 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      2.29 |         4 | 2014-11-21   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      2.12 |        11 | 2017-12-05   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06)    |      1.97 |         6 | 2014-04-08   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      1.75 |        12 | 2013-06-11   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://metrics.torproject.org/rs.html#search/family:185663B7C12777F052B2C2D23D7A239D8DA88A0F) |      1.66 |         5 | 2011-10-06   |
| [Rondie &lt;tor AT rondie DOT nl&gt;](https://metrics.torproject.org/rs.html#details/3796D4DA1871FEAC511A7AFA05F3E2888FE05CA1)                            |      1.58 |         1 | 2018-07-14   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |       1.84 |         7 | 2014-04-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |       1.48 |        19 | 2017-06-13   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       0.97 |        17 | 2015-05-16   |
| [jwbecher@drazisil.com](https://metrics.torproject.org/rs.html#search/family:46FBC671FD6FCE6B298B2BAE3C7AC7D7DDF1365F)                                 |       0.96 |         6 | 2018-05-08   |
| [TotorBE AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:25990FC54D7268C914170A118EE4EE75025451DA)                              |       0.94 |         2 | 2016-10-22   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |       0.84 |         8 | 2015-01-29   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.78 |         7 | 2016-01-03   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                  |       0.75 |         3 | 2018-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.74 |         3 | 2015-04-22   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:27C0081F17CA00AAB981122F6A0E49C6CD0A5A6C)           |       0.72 |        10 | 2018-01-07   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.751 |     11.85 |       0    |        27 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            1.142 |      0    |       1.84 |         7 | 2014-04-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            0.976 |      0.23 |       1.48 |        20 | 2017-06-13   |
| [Relay Control &lt;office AT universalipsolution dot b](https://metrics.torproject.org/rs.html#search/family:0C2D910C87E9197878C005021E8BF4D2AF0FF17C) |            0.671 |      2.89 |       0    |        20 | 2018-07-10   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.656 |      2.77 |       0.02 |        10 | 2013-08-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)   |            0.606 |      2.61 |       0    |         7 | 2014-04-09   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.6   |      0    |       0.97 |        17 | 2015-05-16   |
| [jwbecher@drazisil.com](https://metrics.torproject.org/rs.html#search/family:46FBC671FD6FCE6B298B2BAE3C7AC7D7DDF1365F)                                 |            0.597 |      0    |       0.96 |         6 | 2018-05-08   |
| [TotorBE AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:25990FC54D7268C914170A118EE4EE75025451DA)                              |            0.585 |      0    |       0.94 |         3 | 2016-05-29   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |            0.534 |      0    |       0.53 |        11 | 2016-10-28   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                |            14.35 |      16.74 |     12.77 |       545 |
| Online S.a.s.          |            14.11 |      17.88 |      9.06 |       342 |
| Hetzner Online GmbH    |             8.15 |       8.14 |      0.67 |       358 |
| Joshua Peter McQuistan |             2.85 |       0.04 |     11.85 |        29 |
| myLoc managed IT AG    |             2.2  |       2.67 |      1.57 |        37 |
| SURFnet bv             |             1.84 |       1.59 |      3.68 |        25 |
| FranTech Solutions     |             1.7  |       1.07 |      3.65 |        42 |
| Host Europe GmbH       |             1.69 |       2.5  |      0    |        37 |
| netcup GmbH            |             1.52 |       2.09 |      0.71 |        51 |
| DigitalOcean, LLC      |             1.3  |       1.23 |      0.1  |       205 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.3         |             55.7 |     69.32 |      53.45 |      2837 |
| 0.2.9         |             15.3 |      9.78 |      15.19 |      1376 |
| 0.3.2         |             14.4 |      8.22 |      16.62 |       953 |
| 0.3.4         |              7.3 |      7.47 |       8.55 |       235 |
| 0.3.1         |              2.8 |      3.14 |       3    |       232 |
| 0.2.5         |              1.5 |      1.02 |       1.25 |       244 |
| 0.2.4         |              1   |      0.09 |       0.5  |       193 |
| 0.2.7         |              0.5 |      0.08 |       0.41 |       141 |
| 0.3.0         |              0.5 |      0.01 |       0.46 |        67 |
| 0.3.5         |              0.4 |      0.81 |       0.31 |        16 |
| 0.2.8         |              0.1 |      0    |       0.17 |        32 |
| 0.2.6         |              0   |      0    |       0.04 |        23 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.87 |       2.85 |      1.24 |       700 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.6 |      88.8 |       90   |      5810 |
| BSD     |              9   |      11   |        9.5 |       406 |
| Windows |              0.1 |       0   |        0.1 |        85 |
| Darwin  |              0   |       0   |        0   |        13 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            25.22 |      23.64 |       23.23 |     31.12 |       883 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     32.93 |            206 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| None                                       |       284 |
| obfs4                                      |       284 |
| obfs3, obfs4                               |        44 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| fte, obfs3, obfs4                          |         2 |
| meek                                       |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| obfs2, obfs3                               |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

