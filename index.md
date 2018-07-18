---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-07-18 19:00 UTC**

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

| Contact                                                                                        | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-----------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [Cheena &lt;cheena @ cheena . net&gt;](endtoend-correlation-groups#cheena-cheena--cheena--net) | 0.13        | 0.03       | 4         | 3               | 2018-06-14     | 1                           |
| [tor at releasing dot fun](endtoend-correlation-groups#toratreleasingdotfun)                   | 0.03        | 0.11       | 4         | 4               | 2018-07-04     | 1                           |
| [DuckSounds31@aol.com](endtoend-correlation-groups#ducksounds31aolcom)                         | 0.01        | 0.04       | 3         | 3               | 2018-03-02     | 1                           |
| **Total**                                                                                      | **0.17**    | **0.18**   | **11**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |     10.27 |        27 | 2016-01-25   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      3.68 |        13 | 2015-05-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88)    |      3.23 |         7 | 2017-10-03   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)      |      2.96 |         7 | 2014-04-09   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC)    |      2.64 |         7 | 2016-12-23   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.41 |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      2.39 |        11 | 2017-12-05   |
| [abuse aT nectodoT--onion](https://metrics.torproject.org/rs.html#search/family:162F7E752504C49A656FF1E9669E0B9572CE4870)                                 |      2.01 |         6 | 2015-08-27   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06)    |      1.88 |         6 | 2014-04-08   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      1.79 |        12 | 2013-06-11   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |       1.76 |         7 | 2014-04-22   |
| [tor AT appliedprivacy.net](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)                             |       1.36 |        13 | 2017-06-13   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       1.14 |        17 | 2015-05-16   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |       0.98 |         8 | 2015-01-29   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.92 |         7 | 2016-01-03   |
| [https://onioncount.github.io/ https://onionpop.g](https://metrics.torproject.org/rs.html#search/family:068308AD070849A71B8C1DB06C2509E82C40B908)      |       0.91 |         6 | 2016-08-10   |
| [abuse AT torworld.org - BTC 34yFiqwbcUA5MYSvUcpj](https://metrics.torproject.org/rs.html#search/family:157106182B9F33663CAEDCD883D302316331DE5E)      |       0.82 |        10 | 2016-10-28   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                  |       0.79 |         3 | 2018-04-22   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.75 |         5 | 2017-10-24   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.71 |         2 | 2015-04-22   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.725 |     10.27 |       0    |        27 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            1.063 |      0    |       1.76 |         7 | 2014-04-22   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.989 |      3.68 |       0.02 |        14 | 2013-08-22   |
| [tor AT appliedprivacy.net](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)                             |            0.899 |      0    |       1.36 |        16 | 2017-06-13   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0FF233C8D78A17B8DB7C8257D2E05CD5AA7C6B88) |            0.857 |      3.23 |       0    |         7 | 2017-10-03   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)   |            0.784 |      2.96 |       0    |         7 | 2014-04-09   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |            0.7   |      2.64 |       0    |         7 | 2016-12-23   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |            0.691 |      0    |       1.14 |        17 | 2015-05-16   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.641 |      2.41 |       0    |         1 | 2014-04-19   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |            0.634 |      2.39 |       0    |        11 | 2017-12-05   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                   |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:--------------------------|-----------------:|-----------:|----------:|----------:|
| Online S.a.s.             |            13.44 |      15.86 |      9.83 |       343 |
| OVH SAS                   |            13.22 |      16.37 |      8.88 |       538 |
| Hetzner Online GmbH       |             7.39 |       8.76 |      0.6  |       341 |
| Joshua Peter McQuistan    |             2.83 |       0.06 |     10.27 |        31 |
| SURFnet bv                |             1.87 |       1.62 |      3.34 |        25 |
| netcup GmbH               |             1.78 |       2.15 |      0.44 |        46 |
| Host Europe GmbH          |             1.74 |       2.74 |      0.15 |        32 |
| myLoc managed IT AG       |             1.65 |       2.22 |      0.68 |        40 |
| DigitalOcean, LLC         |             1.39 |       1.62 |      0.2  |       215 |
| NForce Entertainment B.V. |             1.38 |       0.21 |      4.58 |        24 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.3         |             50.1 |     60.3  |      49.22 |      2536 |
| 0.3.2         |             19.6 |     16.16 |      21.26 |      1299 |
| 0.2.9         |             14.4 |      7.32 |      15.48 |      1382 |
| 0.3.4         |              5.8 |      8.28 |       5.9  |       185 |
| 0.3.1         |              4.7 |      4.74 |       4.39 |       323 |
| 0.2.5         |              2.1 |      1.43 |       1.87 |       274 |
| 0.2.4         |              1.1 |      0.26 |       0.49 |       216 |
| 0.2.7         |              0.6 |      0.03 |       0.42 |       155 |
| 0.3.0         |              0.5 |      0.04 |       0.56 |        92 |
| 0.3.5         |              0.4 |      1.11 |       0.22 |        14 |
| 0.2.8         |              0.1 |      0.25 |       0.08 |        32 |
| 0.2.6         |              0   |      0.01 |       0.05 |        28 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             4.62 |       3.49 |      2.05 |       797 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.6 |      90.5 |       89.9 |      6008 |
| BSD     |              9   |       9.4 |        9.8 |       373 |
| Windows |              0.1 |       0   |        0.1 |       101 |
| Darwin  |              0   |       0   |        0   |        16 |
| SunOS   |              0   |       0   |        0   |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            24.49 |      25.68 |       21.73 |     26.66 |       821 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     29.78 |            188 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports              |   Bridges |
|:----------------------------------|----------:|
| obfs4                             |       164 |
| None                              |       106 |
| obfs3, obfs4                      |        22 |
| obfs2, obfs3, obfs4               |         4 |
| obfs3, obfs4, scramblesuit        |         3 |
| fte, obfs3, obfs4                 |         1 |
| fte, obfs4                        |         1 |
| meek                              |         1 |
| obfs2, obfs3                      |         1 |
| obfs2, obfs3, obfs4, scramblesuit |         1 |
| obfs3, scramblesuit               |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

