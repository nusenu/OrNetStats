---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2018-11-03 08:00 UTC**

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

| Contact                                                                                                   | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:----------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [tor-operator@your-emailaddress-domain](endtoend-correlation-groups#tor-operatoryour-emailaddress-domain) | 0.11        | 0.14       | 5         | 5               | 2018-09-25     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)      | 0.03        | 0.14       | 3         | 2               | 2016-08-28     | 1                           |
| [tor@sechsnulldrei.org](endtoend-correlation-groups#torsechsnulldreiorg)                                  | 0.03        | 0.29       | 4         | 2               | 2018-10-19     | 2                           |
| [&lt;nobody AT example dot com&gt;](endtoend-correlation-groups#nobody-at-example-dot-com)                | 0.02        | 0.1        | 2         | 2               | 2018-05-21     | 1                           |
| [wgetdataatprotonmailch tor-relay.co](endtoend-correlation-groups#wgetdataatprotonmailch-tor-relayco)     | 0.01        | 0.06       | 2         | 2               | 2018-09-17     | 1                           |
| **Total**                                                                                                 | **0.20**    | **0.73**   | **16**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |     10.95 |        27 | 2016-01-25   |
| [Datashield, Inc. abuse@xor.sc](https://metrics.torproject.org/rs.html#search/family:233305C289F36AEC5B291C9431AB316016C769CC)                         |      6.48 |         6 | 2018-02-24   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |      3.19 |        13 | 2015-05-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      3.05 |         1 | 2014-04-19   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |      2.85 |        21 | 2016-08-22   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:4BFC9C631A93FF4BA3AA84BC6931B4310C38A263)     |      2.56 |         3 | 2018-04-05   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://metrics.torproject.org/rs.html#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      2.04 |         4 | 2014-11-21   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://metrics.torproject.org/rs.html#search/family:0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED)  |      1.86 |        11 | 2017-12-05   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |      1.85 |         7 | 2016-12-23   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://metrics.torproject.org/rs.html#search/family:93FAB6F91C2EF33D0ACEEF7448177FCA2CEB99A0)   |      1.76 |         5 | 2016-01-22   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |       1.74 |        17 | 2017-06-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)       |       1.2  |         5 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                      |       0.94 |         3 | 2015-04-22   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                                 |       0.86 |         5 | 2017-10-24   |
| [Peter Pan &lt;peterpan@fscore.de&gt;](https://metrics.torproject.org/rs.html#search/family:36B08222339CE4EA4989ECB37CF6D060BDECB486)                     |       0.85 |         3 | 2018-04-22   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:136F9299A5009A4E0E96494E723BDB556FB0A26B)                     |       0.84 |         8 | 2015-01-29   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://metrics.torproject.org/rs.html#search/family:38CC95A8CE92A591D4A5779359BEFFBA13FA1B88)    |       0.77 |         7 | 2016-01-03   |
| [TotorBE AT gmail DOT com](https://metrics.torproject.org/rs.html#search/family:25990FC54D7268C914170A118EE4EE75025451DA)                                 |       0.76 |         3 | 2016-05-29   |
| [0x7A8647DB Daniel Winzen &lt;d@winzen4.de&gt; - 1CHvjeMJ](https://metrics.torproject.org/rs.html#search/family:28A598AF03F9552B19B53ADAC80B4C1C51904B64) |       0.72 |         7 | 2017-07-17   |
| [TheEpTic &lt;torrelay@eptic.me&gt; - BTC: 18HoXqpoVicNs5](https://metrics.torproject.org/rs.html#search/family:4204C1B166CCE784CF38B02E4A0C94640A2BECA2) |       0.67 |         6 | 2017-03-29   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:1084200B44021D308EA4253F256794671B1D099A)                         |            2.614 |     10.95 |       0    |        27 | 2016-01-25   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.649 |      2.56 |       1.74 |        20 | 2017-06-13   |
| [Datashield, Inc. abuse@xor.sc](https://metrics.torproject.org/rs.html#search/family:233305C289F36AEC5B291C9431AB316016C769CC)                         |            1.548 |      6.48 |       0    |         6 | 2018-02-24   |
| [contact@alium.rocks](https://metrics.torproject.org/rs.html#search/family:007FD908E9CFCF59E64FBA42B7571D2CF401BC5D)                                   |            1.138 |      0    |       0    |        17 | 2018-10-06   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://metrics.torproject.org/rs.html#search/family:2F9A6B5ADBE91EC69F55AAFB7DC49619D31B8324)    |            0.811 |      0    |       1.2  |         7 | 2014-04-22   |
| [https://www.digitale-gesellschaft.ch/abuse/](https://metrics.torproject.org/rs.html#search/family:0111BA9B604669E636FFD5B503F382A4B7AD6E80)           |            0.77  |      3.19 |       0.01 |        14 | 2013-08-22   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://metrics.torproject.org/rs.html#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |            0.729 |      3.05 |       0    |         1 | 2014-04-19   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |            0.682 |      2.85 |       0    |        21 | 2016-08-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                   |            0.559 |      0    |       0.94 |         3 | 2015-04-22   |
| [sirmatt ksu edu 0x94FBBB0A](https://metrics.torproject.org/rs.html#search/family:09FA8B4F665AD65D2C2A49870F1AA3BA8811E449)                            |            0.546 |      0.67 |       0.37 |         6 | 2016-11-02   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                                                          |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-----------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                                                          |            14.41 |      18.12 |     10.81 |       579 |
| Online S.a.s.                                                    |            13.37 |      16.86 |      6.8  |       349 |
| Hetzner Online GmbH                                              |            11.39 |      11.33 |      0.53 |       384 |
| Joshua Peter McQuistan                                           |             3.22 |       0.49 |     11.43 |        33 |
| NForce Entertainment B.V.                                        |             2.21 |       0.2  |      8.63 |        30 |
| myLoc managed IT AG                                              |             1.96 |       2.46 |      1.57 |        40 |
| SURFnet bv                                                       |             1.76 |       1.72 |      3.04 |        24 |
| Next Layer Telekommunikationsdienstleistungs- und Beratungs GmbH |             1.52 |       1.53 |      2.56 |        17 |
| netcup GmbH                                                      |             1.24 |       1.48 |      0.2  |        49 |
| FranTech Solutions                                               |             1.23 |       0.81 |      2.62 |        45 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.4         |             50.2 |     61.75 |      47.86 |      2454 |
| 0.3.3         |             18   |     23.96 |      16.2  |      1270 |
| 0.2.9         |             14.4 |      6.01 |      16.58 |      1312 |
| 0.3.2         |              8.8 |      3.4  |      11.29 |       486 |
| 0.3.5         |              4   |      3.36 |       4.48 |       140 |
| 0.3.1         |              1.2 |      0.45 |       1.41 |       132 |
| 0.2.5         |              1   |      0.59 |       0.83 |       194 |
| 0.2.4         |              0.8 |      0.23 |       0.25 |       179 |
| 0.2.7         |              0.4 |      0.03 |       0.46 |       130 |
| 0.3.6         |              0.4 |      0.06 |       0.31 |        17 |
| 0.2.8         |              0.1 |      0    |       0.13 |        31 |
| 0.3.0         |              0.1 |      0.02 |       0.12 |        70 |
| 0.2.6         |              0   |      0.01 |       0.04 |        23 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|            13.23 |      14.87 |      4.82 |      1262 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             90.4 |      86   |       90.7 |      5890 |
| BSD     |              9.1 |      13.2 |        8.9 |       404 |
| Windows |              0.3 |       0.6 |        0   |        93 |
| SunOS   |              0.1 |       0   |        0.1 |         5 |
| Darwin  |              0   |       0   |        0   |        13 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            27.16 |      24.94 |       27.43 |     30.26 |       920 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|      33.2 |            197 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       406 |
| None                                       |       351 |
| obfs3, obfs4                               |        47 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs3                                      |         7 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| obfs3, obfs4, scramblesuit                 |         3 |
| fte, meek, obfs3, obfs4                    |         2 |
| fte, obfs3, obfs4                          |         2 |
| obfs2, obfs3                               |         2 |
| obfs3, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| meek                                       |         1 |
| obfs4, scramblesuit                        |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

