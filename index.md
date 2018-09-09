---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-09-09 16:00 UTC**

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
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca) | 0.07        | 0.32       | 7         | 2               | 2018-02-11     | 5                           |
| [abuse-node49 AT posteo DOT de](endtoend-correlation-groups#abuse-node49-at-posteo-dot-de)                     | 0.05        | 1.12       | 7         | 6               | 2018-09-05     | 1                           |
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)      | 0.02        | 0.14       | 3         | 3               | 2018-08-17     | 1                           |
| **Total**                                                                                                      | **0.14**    | **1.58**   | **17**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |     10.25 |        27 | 2016-01-25   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      2.58 |         9 | 2015-05-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.48 |         1 | 2014-04-19   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)   |      2.45 |         7 | 2014-04-09   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |      2.23 |         7 | 2016-12-23   |
| [Relay Control &lt;office AT universalipsolution dot b](https://metrics.torproject.org/rs.html#search/family:0C2D910C87E9197878C005021E8BF4D2AF0FF17C) |      2.2  |        20 | 2018-07-10   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      2.11 |        11 | 2017-12-05   |
| [abuse aT nectodoT--onion](https://metrics.torproject.org/rs.html#search/family:162F7E752504C49A656FF1E9669E0B9572CE4870)                              |      2.07 |         4 | 2015-08-27   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      1.95 |         4 | 2014-11-21   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06) |      1.92 |         6 | 2014-04-08   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)       |       2.07 |         7 | 2014-04-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |       1.36 |        19 | 2017-06-13   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)            |       1.25 |        17 | 2015-05-16   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                      |       0.88 |         3 | 2015-04-22   |
| [jwbecher@drazisil.com](https://metrics.torproject.org/rs.html#search/family:46FBC671FD6FCE6B298B2BAE3C7AC7D7DDF1365F)                                    |       0.83 |         6 | 2018-05-08   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                     |       0.81 |         8 | 2015-01-29   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88)    |       0.79 |         7 | 2016-01-03   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                     |       0.75 |         3 | 2018-04-22   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)         |       0.75 |         9 | 2016-12-11   |
| [TheEpTic &lt;torrelay@eptic.me&gt; - BTC: 18HoXqpoVicNs5](https://metrics.torproject.org/rs.html#search/family:4204C1B166CCE784CF38B02E4A0C94640A2BECA2) |       0.69 |         6 | 2017-03-29   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-----------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                       |            2.441 |     10.25 |       0    |        27 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)  |            1.277 |      0    |       2.07 |         7 | 2014-04-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)   |            0.936 |      0.4  |       1.36 |        20 | 2017-06-13   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)       |            0.772 |      0    |       1.25 |        17 | 2015-05-16   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)         |            0.624 |      2.58 |       0.01 |        10 | 2013-08-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)        |            0.59  |      2.48 |       0    |         1 | 2014-04-19   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442) |            0.584 |      2.45 |       0    |         7 | 2014-04-09   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)    |            0.555 |      0    |       0.75 |        10 | 2016-10-28   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                 |            0.542 |      0    |       0.88 |         3 | 2015-04-22   |
| [sirmatt ksu edu 0x94FBBB0A](https://metrics.torproject.org/rs.html#search/family:7272A578FD463764A95862B871878CA045F177A3)                          |            0.541 |      0    |       0.19 |         4 | 2017-02-25   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                |            14.27 |      16.99 |     11.49 |       550 |
| Online S.a.s.          |            13.67 |      17.54 |      7.65 |       340 |
| Hetzner Online GmbH    |             8.26 |       8.28 |      0.66 |       351 |
| Joshua Peter McQuistan |             2.99 |       0.03 |     10.25 |        31 |
| myLoc managed IT AG    |             2.44 |       2.81 |      1.87 |        39 |
| SURFnet bv             |             1.87 |       1.72 |      3.39 |        25 |
| FranTech Solutions     |             1.86 |       1.17 |      4.4  |        41 |
| netcup GmbH            |             1.73 |       2.02 |      0.93 |        49 |
| Host Europe GmbH       |             1.72 |       2.61 |      0    |        34 |
| 1&amp;1 Internet SE    |             1.21 |       1.85 |      0.19 |        22 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.3         |             55.5 |     66.8  |      53.84 |      2886 |
| 0.2.9         |             14.4 |      9.29 |      14.57 |      1384 |
| 0.3.2         |             13.8 |      7.71 |      15.57 |      1065 |
| 0.3.4         |              8.6 |     10.8  |       9.13 |       249 |
| 0.3.1         |              2.8 |      2.8  |       3.23 |       220 |
| 0.2.5         |              1.6 |      0.92 |       1.42 |       233 |
| 0.2.4         |              1.2 |      0.33 |       0.5  |       200 |
| 0.2.7         |              0.5 |      0.04 |       0.48 |       137 |
| 0.3.5         |              0.5 |      1.23 |       0.37 |        17 |
| 0.3.0         |              0.4 |      0    |       0.6  |        63 |
| 0.2.8         |              0.1 |      0    |       0.19 |        33 |
| 0.2.6         |              0   |      0.01 |       0.05 |        28 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|              4.1 |       3.27 |      1.32 |       694 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.9 |      88   |       90.9 |      5961 |
| BSD     |              8.7 |      11.8 |        8.7 |       392 |
| SunOS   |              0.1 |       0   |        0.1 |         5 |
| Windows |              0.1 |       0   |        0   |        92 |
| Darwin  |              0   |       0   |        0   |        16 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            25.38 |      23.34 |       23.12 |     32.27 |       876 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     35.01 |            211 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| None                                       |       286 |
| obfs4                                      |       284 |
| obfs3, obfs4                               |        44 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3, obfs4                        |         8 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         3 |
| meek                                       |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs3, obfs4                          |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

