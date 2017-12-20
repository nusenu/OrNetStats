---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-12-20 20:00 UTC**

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
| [https://onioncount.github.io/ https://onionpop.g](endtoend-correlation-groups#httpsonioncountgithubio--httpsonionpopg)                  | 0.98        | 0.31       | 8         | 2               | 2016-08-10     | 1                           |
| [0x7A8647DB Daniel Winzen &lt;d@winzen4.de&gt; - 1CHvjeMJ](endtoend-correlation-groups#0x7a8647db-daniel-winzen-dwinzen4de---1chvjemj)   | 0.44        | 0.4        | 9         | 7               | 2017-08-13     | 1                           |
| [ricksybusiness@riseup.net](endtoend-correlation-groups#ricksybusinessriseupnet)                                                         | 0.38        | 0.08       | 4         | 3               | 2017-10-23     | 1                           |
| [see https://www.artikel5ev.de/torcontact/](endtoend-correlation-groups#see-httpswwwartikel5evdetorcontact)                              | 0.38        | 0.4        | 9         | 6               | 2017-12-05     | 1                           |
| [sirmatt ksu edu 0x94FBBB0A https://onioncount.gith](endtoend-correlation-groups#sirmatt-ksu-edu-0x94fbbb0a-httpsonioncountgith)         | 0.36        | 1.16       | 4         | 2               | 2017-05-30     | 1                           |
| [Viktor &lt;vnikolov AT vnikolov dot cz&gt;](endtoend-correlation-groups#viktor-vnikolov-at-vnikolov-dot-cz)                             | 0.24        | 1.66       | 8         | 4               | 2017-12-12     | 1                           |
| [abuse AT torworld.org - BTC 17iwdtpmgHdPt15twdT2](endtoend-correlation-groups#abuse-at-torworldorg---btc-17iwdtpmghdpt15twdt2)          | 0.19        | 1.24       | 8         | 5               | 2017-12-12     | 1                           |
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.18        | 0.2        | 4         | 3               | 2017-11-29     | 1                           |
| [abuse@to-surf-and-protect.net](endtoend-correlation-groups#abuseto-surf-and-protectnet)                                                 | 0.11        | 9.42       | 25        | 4               | 2016-12-02     | 1                           |
| [Walter Heukels &lt;walter@badexample.net&gt;](endtoend-correlation-groups#walter-heukels-walterbadexamplenet)                           | 0.11        | 1.08       | 2         | 2               | 2015-05-04     | 1                           |
| [PGP key 0x3ee63e8a6beba798](endtoend-correlation-groups#pgp-key-0x3ee63e8a6beba798)                                                     | 0.1         | 0.07       | 2         | 2               | 2017-11-24     | 1                           |
| [milksteak@tfwno.gf](endtoend-correlation-groups#milksteaktfwnogf)                                                                       | 0.09        | 0.01       | 2         | 2               | 2017-10-07     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.08        | 0.4        | 2         | 2               | 2017-02-16     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb) | 0.08        | 0.91       | 13        | 2               | 2016-04-01     | 1                           |
| [https://www.torservers.net/donate.html &lt;support .A](endtoend-correlation-groups#httpswwwtorserversnetdonatehtml-support-a)           | 0.06        | 4.34       | 11        | 3               | 2017-11-01     | 1                           |
| [0xDD7831FC Matthias Kretschmann &lt;m AT kretschmann](endtoend-correlation-groups#0xdd7831fc-matthias-kretschmann-m-at-kretschmann-)    | 0.05        | 0.28       | 2         | 2               | 2016-05-09     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                     | 0.04        | 0.18       | 2         | 2               | 2016-08-28     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                                 | 0.04        | 0.03       | 3         | 3               | 2017-10-01     | 1                           |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](endtoend-correlation-groups#tornoisebridgenet-admintornoisebridgenet)            | 0.03        | 1.45       | 9         | 3               | 2017-08-14     | 1                           |
| [Zack Weinberg https://www.owlfolio.org/contact/](endtoend-correlation-groups#zack-weinberg-httpswwwowlfolioorgcontact)                  | 0.03        | 0.05       | 2         | 2               | 2014-04-08     | 1                           |
| **Total**                                                                                                                                | **3.97**    | **23.67**  | **129**   |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                         |   Exit(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)       |      3.42 |         1 | 2014-04-19   |
| [tor@m5isupport.com](https://atlas.torproject.org/#details/E11789392E13A5C248F20084F9D03E4D437188AF)                                       |      1.69 |         1 | 2017-11-19   |
| [abuse@blockone.cz - 1DGEy5TrULnUns8T2CN97WnD8pTHLD](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)       |      1.19 |         1 | 2017-07-20   |
| [Walter Heukels &lt;walter@badexample.net&gt;](https://atlas.torproject.org/#details/7DD29A65C370B86B5BE706EA3B1417745714C8AF)             |      1.08 |         1 | 2015-05-04   |
| [abuse at emeraldonion dot org](https://atlas.torproject.org/#details/CA9739E2805A3CD73CF75BBCB6785C32394240E3)                            |      1.05 |         1 | 2017-08-30   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#details/FE3587D12AACD55486E7024A5EC8CE0994643BA0)                            |      1.01 |         1 | 2016-07-28   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#details/379FB450010D17078B3766C2273303C358C3A442)      |      0.97 |         1 | 2014-04-09   |
| [John Doe johndoe@novogara.com](https://atlas.torproject.org/#details/0593F5255316748247EBA76353A3A61F62224903)                            |      0.9  |         1 | 2017-09-05   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#details/A6B0521C4C1FB91FB66398AAD523AD773E82E77E) |      0.89 |         1 | 2015-02-02   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#details/90FD830C357A5109AB3C505287713F1AC811174C)    |      0.86 |         1 | 2015-02-21   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                      |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#details/9844B981A80B3E4B50897098E2D65167E6AEF127)    |       0.54 |         1 | 2016-08-24   |
| [Random Person &lt;nobody AT example dot com&gt;](https://atlas.torproject.org/#details/85F277DFE886353598A51D3CAB04DD3F6EBB427D)       |       0.52 |         1 | 2017-12-09   |
| [enigma AT= s0ny doT--- net](https://atlas.torproject.org/#details/42B4F52C5B11E4D39855F654955425B0D5A0598B)                            |       0.52 |         1 | 2017-02-13   |
| [87C08DDF](https://atlas.torproject.org/#details/87C08DDFD32C62F3C56D371F9774D27BFDBB807B)                                              |       0.42 |         1 | 2017-01-19   |
| [replace k with c : kontakt @ zwiebeltoralf . de](https://atlas.torproject.org/#details/1AF72E8906E6C49481A791A6F8F84F8DFEBBB2BA)       |       0.41 |         1 | 2016-11-26   |
| [91A32B95](https://atlas.torproject.org/#details/91A32B95CC1213704ACF19D7021AD40BDC318204)                                              |       0.4  |         1 | 2016-07-26   |
| [0xF771597D61F018F5 &lt;jon DOT amund02 AT gmail dot c](https://atlas.torproject.org/#details/7F2C51C5FE4249CE32E023105D37C1E6B85B2311) |       0.38 |         1 | 2017-06-10   |
| [ricksybusiness@riseup.net](https://atlas.torproject.org/#details/01AE2DE314276C82FCCC3603A1C2F3238E6544C9)                             |       0.38 |         1 | 2016-08-10   |
| [cubox at irc.freenode.org](https://atlas.torproject.org/#details/09A1AE88A78746AA9EC1BD5953E84F61CB763BCA)                             |       0.36 |         1 | 2017-12-02   |
| [admin@meinecloud.me](https://atlas.torproject.org/#details/74D6D1E8BF5159066768F48C1EA4951C9C97BEF9)                                   |       0.32 |         1 | 2015-06-04   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626) |            0.806 |      3.42 |       0    |         1 | 2014-04-19   |
| [tor@m5isupport.com](https://atlas.torproject.org/#details/E11789392E13A5C248F20084F9D03E4D437188AF)                                 |            0.4   |      1.69 |       0    |         1 | 2017-11-19   |
| [admin &lt;tor AT dezponia dot se&gt;](https://atlas.torproject.org/#details/BF50E09EED25B82861CF95E1AAA42DCFEF53E5D1)               |            0.281 |      0    |       0    |         1 | 2014-04-09   |
| [abuse@blockone.cz - 1DGEy5TrULnUns8T2CN97WnD8pTHLD](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144) |            0.281 |      1.19 |       0    |         1 | 2017-07-20   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#details/9844B981A80B3E4B50897098E2D65167E6AEF127) |            0.273 |      0    |       0.54 |         1 | 2016-08-24   |
| [Random Person &lt;nobody AT example dot com&gt;](https://atlas.torproject.org/#details/85F277DFE886353598A51D3CAB04DD3F6EBB427D)    |            0.262 |      0    |       0.52 |         1 | 2017-12-09   |
| [enigma AT= s0ny doT--- net](https://atlas.torproject.org/#details/42B4F52C5B11E4D39855F654955425B0D5A0598B)                         |            0.26  |      0    |       0.52 |         1 | 2017-02-13   |
| [4A99D158](https://atlas.torproject.org/#details/4A99D15855E0781771780961C367B4F83D2F17B7)                                           |            0.26  |      0    |       0    |         1 | 2017-09-15   |
| [Walter Heukels &lt;walter@badexample.net&gt;](https://atlas.torproject.org/#details/7DD29A65C370B86B5BE706EA3B1417745714C8AF)       |            0.255 |      1.08 |       0    |         1 | 2015-05-04   |
| [abuse at emeraldonion dot org](https://atlas.torproject.org/#details/CA9739E2805A3CD73CF75BBCB6785C32394240E3)                      |            0.249 |      1.05 |       0    |         1 | 2017-08-30   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                     |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:----------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                     |            15.66 |      16.36 |      6.36 |       512 |
| Online S.a.s.               |            10.88 |      12.92 |     11.51 |       398 |
| Hetzner Online GmbH         |             7.3  |       9.32 |      0.86 |       292 |
| DigitalOcean, LLC           |             4.47 |       5.66 |      1.39 |       299 |
| Host Europe GmbH            |             2.61 |       4.29 |      0    |        43 |
| THC Projects SRL            |             1.53 |       3.04 |      0    |        21 |
| myLoc managed IT AG         |             1.39 |       1.98 |      0.46 |        43 |
| SOFTplus Entwicklungen GmbH |             1.25 |       0.06 |      5.02 |        18 |
| SURFnet bv                  |             1.09 |       0.32 |      0.82 |        12 |
| ISPpro Internet KG          |             0.97 |       1.82 |      0    |        27 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.1         |             56.7 |     61.47 |      54.81 |      2868 |
| 0.2.9         |             14.8 |     10.53 |      15.78 |      1285 |
| 0.3.0         |              9.1 |      6.48 |       8.99 |       506 |
| 0.3.2         |              8.1 |     14.08 |       7.69 |       271 |
| 0.2.5         |              5.6 |      4.21 |       7.01 |       610 |
| 0.2.7         |              1.8 |      0.36 |       2.36 |       285 |
| 0.2.4         |              1.3 |      0.14 |       1.71 |       338 |
| 0.3.3         |              1   |      2.34 |       0.25 |        13 |
| 0.2.8         |              0.7 |      0.24 |       0.93 |        86 |
| 0.2.6         |              0.3 |      0.12 |       0.42 |        55 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             3.59 |        4.5 |      0.63 |       678 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             91.2 |      89.2 |       92.1 |      5831 |
| BSD     |              8.3 |      10.7 |        7.5 |       299 |
| Windows |              0.1 |       0   |        0   |       152 |
| SunOS   |              0.1 |       0   |        0.2 |         4 |
| Darwin  |              0   |       0   |        0   |        12 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.71 |      18.06 |       14.89 |     25.95 |       588 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     31.32 |            131 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1193 |
| None                                       |       609 |
| obfs3, obfs4, scramblesuit                 |       191 |
| obfs3, obfs4                               |        63 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs3                                      |        19 |
| obfs2, obfs3                               |        10 |
| obfs3, scramblesuit                        |         9 |
| obfs2, obfs3, obfs4                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         5 |
| fte, obfs3, obfs4                          |         4 |
| obfs2, obfs3, obfs4, scramblesuit          |         2 |
| obfs4, scramblesuit                        |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| meek                                       |         1 |
| meek, obfs4                                |         1 |
| scramblesuit                               |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

