---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-07-27 15:00 UTC**

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
| [see https://www.artikel5ev.de/torcontact/](endtoend-correlation-groups#see-httpswwwartikel5evdetorcontact)                              | 0.54        | 0.28       | 14        | 10              | 2017-04-27     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-btc---14w) | 0.12        | 0.62       | 12        | 2               | 2016-04-01     | 4                           |
| [George Shuklin &lt;george.shuklin@gmail.com&gt;](endtoend-correlation-groups#george-shuklin-georgeshuklingmailcom)                      | 0.04        | 0.01       | 2         | 2               | 2016-07-21     | 1                           |
| [Abuse Department &lt;abuse AT hartvoorinternetvrijhei](endtoend-correlation-groups#abuse-department-abuse-at-hartvoorinternetvrijhei)   | 0.03        | 1.7        | 2         | 2               | 2015-09-06     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)     | 0.03        | 0.21       | 6         | 6               | 2017-07-23     | 1                           |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](endtoend-correlation-groups#tornoisebridgenet-admintornoisebridgenet)            | 0.01        | 1.13       | 5         | 2               | 2017-05-21     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           | 0.01        | 0.69       | 3         | 3               | 2016-08-08     | 1                           |
| **Total**                                                                                                                                | **0.78**    | **4.64**   | **44**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                            |   Exit(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |      5.33 |         7 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |      4.52 |        21 | 2016-01-25   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |      3.91 |         4 | 2014-11-21   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:E34E25D958D46DDE5092385B14117C9B301DC0E9)  |      2.66 |        17 | 2014-05-19   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C) |      2.46 |         6 | 2014-04-08   |
| [29C92C85](https://atlas.torproject.org/#details/29C92C854E0F6652A77F3A8B231D6932993969E8)                                                    |      2.28 |         1 | 2017-04-10   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                              |      2.15 |         7 | 2015-08-27   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                 |      2.15 |         6 | 2016-04-02   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      1.97 |         1 | 2014-04-19   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |      1.89 |         3 | 2014-02-13   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)       |       1.75 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                    |       1.22 |        32 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                      |       1.19 |         3 | 2015-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)            |       1.13 |        22 | 2015-05-16   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)       |       1.04 |         6 | 2016-12-23   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)           |       1.04 |         7 | 2016-08-10   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:8672E8A01B4D3FA4C0BBE21C740D4506302EA487)                         |       0.91 |         6 | 2016-03-10   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                     |       0.87 |        10 | 2014-04-10   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F)    |       0.61 |         6 | 2016-01-03   |
| [0x7A8647DB Daniel Winzen &lt;d@winzen4.de&gt; - 1CHvjeMJ](https://atlas.torproject.org/#search/family:72B19BAABE6846DF96EA2A50C28F4DC15A920041) |       0.58 |         5 | 2016-05-16   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.275 |      4.52 |       0.46 |        29 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            1.178 |      0    |       1.75 |         7 | 2014-04-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            1.137 |      5.33 |       0    |         7 | 2014-04-09   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |            1.102 |      1.89 |       1.04 |         9 | 2014-02-13   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.84  |      0    |       1.22 |        38 | 2014-12-23   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.834 |      3.91 |       0    |         4 | 2014-11-21   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.803 |      0    |       1.19 |         3 | 2015-04-22   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |            0.788 |      0.4  |       1.04 |        10 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.763 |      0    |       1.13 |        22 | 2015-05-16   |
| [sirmatt ksu edu 0x94FBBB0A](https://atlas.torproject.org/#search/family:68CECB9ECDF5EFE8FF23C25B926D756FB346FD92)                            |            0.637 |      1.54 |       0.46 |        10 | 2015-06-01   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.0         |             38.5 |     39.55 |      38.93 |      2157 |
| 0.2.9         |             31.4 |     26.24 |      33.24 |      1884 |
| 0.2.5         |              9.1 |      9.91 |       8.54 |       968 |
| 0.2.7         |              7.3 |      5.24 |       6.95 |       814 |
| 0.2.8         |              5.3 |      6.18 |       5.39 |       313 |
| 0.3.1         |              3.6 |      6.95 |       2.87 |       150 |
| 0.2.4         |              3.3 |      3.49 |       3.19 |       555 |
| 0.2.6         |              0.7 |      0.56 |       0.77 |        87 |
| 0.3.2         |              0.4 |      1.84 |       0.08 |        16 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93.2 |      91.5 |       93.7 |      6418 |
| BSD     |              6.3 |       8.4 |        5.9 |       337 |
| SunOS   |              0.1 |       0   |        0.1 |         4 |
| Windows |              0.1 |       0   |        0   |       158 |
| Darwin  |              0   |       0   |        0.1 |        13 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            17.81 |      17.31 |       14.91 |     24.07 |       571 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     31.09 |            133 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1667 |
| None                                       |       643 |
| obfs3, obfs4, scramblesuit                 |       478 |
| obfs3, obfs4                               |        85 |
| obfs3                                      |        25 |
| fte, obfs3, obfs4, scramblesuit            |        24 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| scramblesuit                               |        18 |
| obfs2, obfs3                               |        11 |
| obfs3, scramblesuit                        |         9 |
| obfs2, obfs3, obfs4                        |         7 |
| fte, obfs3, obfs4                          |         4 |
| meek                                       |         4 |
| obfs2, obfs3, obfs4, scramblesuit          |         3 |
| obfs4, scramblesuit                        |         2 |
| snowflake                                  |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| obfs3 websocket, websocket                 |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

