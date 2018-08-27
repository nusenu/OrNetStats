---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-08-27 14:00 UTC**

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
| [Jordan &lt;jordan@yui.cat&gt;](endtoend-correlation-groups#jordan-jordanyuicat)                               | 0.19        | 0.04       | 4         | 3               | 2018-06-26     | 1                           |
| [abuse-node49 AT posteo DOT de](endtoend-correlation-groups#abuse-node49-at-posteo-dot-de)                     | 0.16        | 0.04       | 6         | 6               | 2018-08-25     | 2                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca) | 0.07        | 0.34       | 7         | 2               | 2018-02-11     | 5                           |
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain)      | 0.02        | 0.09       | 2         | 2               | 2018-08-15     | 1                           |
| **Total**                                                                                                      | **0.44**    | **0.51**   | **19**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |     11.84 |        27 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)      |      2.82 |         7 | 2014-04-09   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |      2.67 |         9 | 2015-05-22   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |      2.36 |        11 | 2017-12-05   |
| [abuse aT nectodoT--onion](https://metrics.torproject.org/rs.html#search/family:162F7E752504C49A656FF1E9669E0B9572CE4870)                                 |      2.1  |         6 | 2015-08-27   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      2.06 |         4 | 2014-11-21   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://metrics.torproject.org/rs.html#search/family:578E007E5E4535FBFEF7758D8587B07B4C8C5D06)    |      1.91 |         6 | 2014-04-08   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://metrics.torproject.org/rs.html#search/family:185663B7C12777F052B2C2D23D7A239D8DA88A0F) |      1.71 |         5 | 2011-10-06   |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](https://metrics.torproject.org/rs.html#search/family:0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)               |      1.66 |         4 | 2017-11-29   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      1.64 |        12 | 2013-06-11   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                     |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.7  |         6 | 2014-04-22   |
| [email:tor appliedprivacy.net twitter:applied priv](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |       1.47 |        19 | 2017-06-13   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)         |       1.06 |        17 | 2015-05-16   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                  |       0.85 |         8 | 2015-01-29   |
| [sirmatt ksu edu 0x94FBBB0A](https://metrics.torproject.org/rs.html#search/family:7272A578FD463764A95862B871878CA045F177A3)                            |       0.84 |         4 | 2017-02-25   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                  |       0.79 |         3 | 2018-04-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88) |       0.79 |         7 | 2016-01-03   |
| [TotorBE AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:25990FC54D7268C914170A118EE4EE75025451DA)                              |       0.76 |         2 | 2016-10-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |       0.74 |         3 | 2015-04-22   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                              |       0.73 |         5 | 2017-10-24   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                        |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                            |            2.832 |     11.84 |       0    |        27 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)       |            1.126 |      0    |       1.7  |         7 | 2014-04-22   |
| [email:tor appliedprivacy.net twitter:applied priv](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |            0.963 |      0.17 |       1.47 |        20 | 2017-06-13   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:379FB450010D17078B3766C2273303C358C3A442)      |            0.676 |      2.82 |       0    |         7 | 2014-04-09   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://metrics.torproject.org/rs.html#search/family:03C3069E814E296EB18776EB61B1ECB754ED89FE)            |            0.663 |      0    |       1.06 |        17 | 2015-05-16   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)              |            0.651 |      2.67 |       0.01 |        10 | 2013-08-22   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)     |            0.565 |      2.36 |       0    |        11 | 2017-12-05   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                     |            0.533 |      0    |       0.85 |         8 | 2015-01-29   |
| [DFRI &lt;tor AT dfri dot se&gt; - 1Muz37TfXVBiJKRJkAqTNo](https://metrics.torproject.org/rs.html#search/family:185663B7C12777F052B2C2D23D7A239D8DA88A0F) |            0.525 |      1.71 |       0.18 |         8 | 2010-02-17   |
| [sirmatt ksu edu 0x94FBBB0A](https://metrics.torproject.org/rs.html#search/family:7272A578FD463764A95862B871878CA045F177A3)                               |            0.524 |      0    |       0.84 |         4 | 2017-02-25   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------|-----------------:|-----------:|----------:|----------:|
| Online S.a.s.          |            14.47 |      17.19 |     10.01 |       341 |
| OVH SAS                |            14.01 |      16.06 |     13.17 |       543 |
| Hetzner Online GmbH    |             7.25 |       8.01 |      0.78 |       342 |
| Joshua Peter McQuistan |             3.35 |       0.67 |     11.84 |        31 |
| myLoc managed IT AG    |             2.15 |       2.62 |      1.76 |        35 |
| SURFnet bv             |             1.79 |       1.53 |      3.4  |        25 |
| Host Europe GmbH       |             1.7  |       2.52 |      0    |        35 |
| FranTech Solutions     |             1.67 |       1.06 |      3.51 |        42 |
| netcup GmbH            |             1.58 |       2.21 |      0.57 |        46 |
| DigitalOcean, LLC      |             1.26 |       1.28 |      0.1  |       197 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.3         |             54.6 |     66.35 |      52.17 |      2788 |
| 0.3.2         |             14.8 |      8.79 |      17.2  |      1048 |
| 0.2.9         |             14.7 |      9.55 |      15.32 |      1355 |
| 0.3.4         |              7.6 |      8.22 |       8.54 |       230 |
| 0.3.1         |              3.5 |      4.91 |       3.32 |       246 |
| 0.2.5         |              1.8 |      1.19 |       1.55 |       247 |
| 0.2.4         |              1   |      0.16 |       0.46 |       191 |
| 0.2.7         |              0.6 |      0.03 |       0.45 |       142 |
| 0.3.0         |              0.5 |      0    |       0.52 |        67 |
| 0.3.5         |              0.3 |      0.75 |       0.26 |        17 |
| 0.2.8         |              0.1 |      0    |       0.1  |        32 |
| 0.2.6         |              0   |      0.01 |       0.05 |        26 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             4.19 |       3.15 |      1.41 |       705 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.3 |      88.7 |       90   |      5852 |
| BSD     |              9.3 |      11.1 |        9.6 |       398 |
| Windows |              0.1 |       0   |        0.1 |        85 |
| Darwin  |              0   |       0   |        0   |        15 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            25.09 |      24.06 |        22.8 |     30.39 |       871 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     32.07 |            194 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       288 |
| None                                       |       275 |
| obfs3, obfs4                               |        43 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3, obfs4                        |         7 |
| obfs3                                      |         6 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| fte, obfs3, obfs4                          |         2 |
| meek                                       |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

