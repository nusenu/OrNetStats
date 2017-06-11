---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-06-11 21:00 UTC**

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

| Contact                                                                                                                                | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:---------------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [see https://www.artikel5ev.de/torcontact/](endtoend-correlation-groups#see-httpswwwartikel5evdetorcontact)                            | 0.75        | 0.25       | 15        | 11              | 2017-04-27     | 1                           |
| [https://www.torservers.net/donate.html &lt;support .A](endtoend-correlation-groups#httpswwwtorserversnetdonatehtml-support-a)         | 0.46        | 5.15       | 13        | 3               | 2017-01-22     | 1                           |
| [snaptorg at gmail , com &gt;&gt; bitcoin:1DmvqGnoexBSzSF](endtoend-correlation-groups#snaptorgatgmailcom--bitcoin1dmvqgnoexbszsf)     | 0.23        | 0.19       | 5         | 4               | 2017-05-03     | 1                           |
| [yscoder@foxmail.com](endtoend-correlation-groups#yscoderfoxmailcom)                                                                   | 0.08        | 0.02       | 4         | 2               | 2017-06-08     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)   | 0.07        | 0.1        | 4         | 4               | 2017-05-25     | 3                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                           | 0.04        | 0.29       | 2         | 2               | 2017-02-16     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                         | 0.03        | 0.41       | 2         | 2               | 2016-08-08     | 1                           |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](endtoend-correlation-groups#tornoisebridgenet-admintornoisebridgenet)          | 0.02        | 3.13       | 9         | 3               | 2017-05-21     | 1                           |
| [Abuse Department &lt;abuse AT hartvoorinternetvrijhei](endtoend-correlation-groups#abuse-department-abuse-at-hartvoorinternetvrijhei) | 0.01        | 1.2        | 2         | 2               | 2015-09-06     | 1                           |
| **Total**                                                                                                                              | **1.69**    | **10.74**  | **56**    |                 |                |                             |

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
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)      |      6.31 |         7 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                            |      3.44 |        23 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:EC15DB62D9101481F364DE52EB8313C838BDDC29)    |      3.25 |        21 | 2016-08-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:65F9944338C684109EB975D0EC7489B30E191E87)       |      3.14 |         4 | 2014-11-21   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:8E6EDA78D8E3ABA88D877C3E37D6D4F0938C7B9F)    |      2.47 |         6 | 2014-04-08   |
| [29C92C85](https://atlas.torproject.org/#details/29C92C854E0F6652A77F3A8B231D6932993969E8)                                                       |      2.44 |         1 | 2017-04-10   |
| [Admin &lt;admin AT xshells DOT net&gt;](https://atlas.torproject.org/#details/E8E71987BCB8C24DBDF1C3BB0BF3B6C76550A108)                         |      2.39 |         1 | 2016-09-14   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://atlas.torproject.org/#search/family:8175A86D8896CEA37FDC67311F9BDC1DDCBE8136)    |      2.37 |         4 | 2017-05-20   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C90CA3B7FE01A146B8268D56977DC4A2C024B9EA)                                    |      2.24 |         6 | 2016-04-02   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:38A42B8D7C0E6346F4A4821617740AEE86EA885B) |      2.11 |         3 | 2014-11-04   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |       1.5  |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |       1.33 |        39 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.12 |         3 | 2015-04-22   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |       0.98 |         7 | 2016-08-10   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |       0.94 |        10 | 2014-04-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |       0.89 |        20 | 2015-05-16   |
| [see https://www.artikel5ev.de/torcontact/](https://atlas.torproject.org/#search/family:035D2E216B065B961E404BD172336050E5AF4EEA)             |       0.74 |        11 | 2016-09-05   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:9C8A123081EFBE022EF795630F447839DDFDDDEC)                      |       0.73 |         7 | 2016-03-10   |
| [45A00F0A](https://atlas.torproject.org/#search/family:45A00F0A6574ADA2B9EA3948590113E7DAA30AAB)                                              |       0.72 |         7 | 2016-07-26   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:72B2B12A3F60408BDBC98C6DF53988D3A0B3F0EE) |       0.58 |         5 | 2016-01-03   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)   |            1.452 |      6.31 |       0    |         7 | 2014-04-09   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |            0.983 |      0    |       1.5  |         7 | 2014-04-22   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                         |            0.941 |      3.44 |       0.22 |        29 | 2016-01-25   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |            0.878 |      0    |       1.33 |        40 | 2014-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:EC15DB62D9101481F364DE52EB8313C838BDDC29) |            0.749 |      3.25 |       0    |        21 | 2016-08-22   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |            0.741 |      0.42 |       0.98 |        11 | 2016-08-10   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.738 |      0    |       1.12 |         3 | 2015-04-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:65F9944338C684109EB975D0EC7489B30E191E87)    |            0.723 |      3.14 |       0    |         4 | 2014-11-21   |
| [see https://www.artikel5ev.de/torcontact/](https://atlas.torproject.org/#search/family:035D2E216B065B961E404BD172336050E5AF4EEA)             |            0.67  |      0.72 |       0.74 |        21 | 2014-04-08   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |            0.616 |      0    |       0.94 |        10 | 2014-04-10   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.2.9         |             48   |     47.9  |      48.14 |      2933 |
| 0.3.0         |             18.6 |     23.09 |      17.4  |       900 |
| 0.2.5         |             10.1 |      9.95 |       9.94 |      1088 |
| 0.2.7         |              7.6 |      6.97 |       7.41 |       849 |
| 0.2.8         |              7   |      6.17 |       7.47 |       438 |
| 0.2.6         |              4.6 |      1.65 |       6.15 |       325 |
| 0.2.4         |              2.5 |      1.22 |       2.83 |       596 |
| 0.3.1         |              1.1 |      3.01 |       0.61 |        50 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93.4 |      93.7 |       93   |      6623 |
| BSD     |              6   |       5.8 |        6.5 |       345 |
| Windows |              0.2 |       0.3 |        0.1 |       176 |
| Darwin  |              0   |       0   |        0   |        13 |
| SunOS   |              0   |       0   |        0.1 |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.62 |      17.88 |       14.77 |     26.32 |       606 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     26.11 |            119 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      2002 |
| None                                       |       657 |
| obfs3, obfs4, scramblesuit                 |       462 |
| fte, obfs3, obfs4, scramblesuit            |       298 |
| obfs3, obfs4                               |       107 |
| scramblesuit                               |        29 |
| obfs3                                      |        27 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3                               |        12 |
| obfs3, scramblesuit                        |        12 |
| obfs2, obfs3, obfs4                        |         7 |
| fte, obfs3, obfs4                          |         5 |
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

