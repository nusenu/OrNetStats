---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-05-20 18:00 UTC**

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
| [aTorRelay@gmail.com](endtoend-correlation-groups#atorrelaygmailcom)                                                                     | 0.28        | 0.15       | 9         | 6               | 2017-03-21     | 1                           |
| [snaptorg at gmail , com &gt;&gt; bitcoin:1DmvqGnoexBSzSF](endtoend-correlation-groups#snaptorgatgmailcom--bitcoin1dmvqgnoexbszsf)       | 0.16        | 0.16       | 5         | 4               | 2017-05-03     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-btc---14w) | 0.15        | 0.59       | 13        | 2               | 2016-04-01     | 4                           |
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.06        | 0.13       | 4         | 4               | 2017-04-13     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.05        | 0.2        | 2         | 2               | 2017-02-16     | 1                           |
| [George Shuklin &lt;george.shuklin@gmail.com&gt;](endtoend-correlation-groups#george-shuklin-georgeshuklingmailcom)                      | 0.04        | 0.01       | 2         | 2               | 2016-07-21     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           | 0.03        | 0.4        | 3         | 3               | 2016-08-08     | 1                           |
| [torman@memeware.net](endtoend-correlation-groups#tormanmemewarenet)                                                                     | 0.02        | 0.09       | 2         | 2               | 2017-05-11     | 1                           |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](endtoend-correlation-groups#tornoisebridgenet-admintornoisebridgenet)            | 0.01        | 0.51       | 5         | 2               | 2015-05-20     | 1                           |
| **Total**                                                                                                                                | **0.80**    | **2.24**   | **45**    |                 |                |                             |

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
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)      |      5.39 |         7 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                            |      4.32 |        24 | 2016-01-25   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:2B44FD1742D26E4F28D4CACF1F0CF8A686270E45)     |      3.44 |        20 | 2014-05-19   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:EC15DB62D9101481F364DE52EB8313C838BDDC29)    |      2.9  |        40 | 2016-08-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:65F9944338C684109EB975D0EC7489B30E191E87)       |      2.74 |         4 | 2014-11-21   |
| [29C92C85](https://atlas.torproject.org/#details/29C92C854E0F6652A77F3A8B231D6932993969E8)                                                       |      2.29 |         1 | 2017-04-10   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:8E6EDA78D8E3ABA88D877C3E37D6D4F0938C7B9F)    |      2.14 |         6 | 2014-04-08   |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](https://atlas.torproject.org/#search/family:53018DB58301743267F057340C51C3151135F13F) |      1.83 |        34 | 2016-09-16   |
| [sirmatt ksu edu 0x94FBBB0A](https://atlas.torproject.org/#search/family:95880E08A375C62D570B885554CCCFBCCB362660)                               |      1.75 |         4 | 2016-11-02   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:162F7E752504C49A656FF1E9669E0B9572CE4870)                                 |      1.74 |         7 | 2015-08-27   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |       1.47 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |       1.38 |        40 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.32 |         3 | 2015-04-22   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |       1.06 |         7 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |       0.97 |        19 | 2015-05-16   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:72B2B12A3F60408BDBC98C6DF53988D3A0B3F0EE) |       0.92 |         5 | 2016-01-03   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |       0.83 |        10 | 2014-04-10   |
| [45A00F0A](https://atlas.torproject.org/#search/family:45A00F0A6574ADA2B9EA3948590113E7DAA30AAB)                                              |       0.69 |         8 | 2016-07-26   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:9C8A123081EFBE022EF795630F447839DDFDDDEC)                      |       0.67 |         6 | 2016-03-10   |
| [Hello, I am a Tor node My nickname: https://youtu](https://atlas.torproject.org/#search/family:0ED06F12AF64D5027422169B61D1AC5366C6FFE9)     |       0.64 |        17 | 2014-11-17   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)   |            1.208 |      5.39 |       0    |         7 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                         |            1.198 |      4.32 |       0.34 |        30 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |            0.988 |      0    |       1.47 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |            0.931 |      0    |       1.38 |        40 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.886 |      0    |       1.32 |         3 | 2015-04-22   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |            0.79  |      0.31 |       1.06 |        11 | 2016-08-10   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:2B44FD1742D26E4F28D4CACF1F0CF8A686270E45)  |            0.772 |      3.44 |       0    |        20 | 2014-05-19   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |            0.655 |      0    |       0.97 |        19 | 2015-05-16   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:EC15DB62D9101481F364DE52EB8313C838BDDC29) |            0.65  |      2.9  |       0    |        40 | 2016-08-22   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:72B2B12A3F60408BDBC98C6DF53988D3A0B3F0EE) |            0.62  |      0    |       0.92 |         5 | 2016-01-03   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.2.9         |             48.9 |     43.63 |      50.57 |      2980 |
| 0.3.0         |             16.9 |     27.92 |      14.17 |       805 |
| 0.2.5         |              9.9 |      6.59 |      10.62 |      1100 |
| 0.2.7         |              7.9 |      7.13 |       7.26 |       890 |
| 0.2.8         |              7.3 |      6.52 |       8.12 |       507 |
| 0.2.6         |              4.7 |      1.98 |       5.95 |       333 |
| 0.2.4         |              3.6 |      4.18 |       3.24 |       647 |
| 0.3.1         |              0.4 |      2.01 |       0.04 |        21 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93.3 |      93.9 |       92.9 |      6669 |
| BSD     |              6.1 |       5.5 |        6.7 |       383 |
| Windows |              0.2 |       0.4 |        0   |       197 |
| SunOS   |              0.1 |       0   |        0.2 |         4 |
| Darwin  |              0   |       0   |        0   |        13 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.74 |      17.99 |       15.27 |     26.03 |       635 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     27.55 |            116 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      2179 |
| None                                       |       635 |
| obfs3, obfs4, scramblesuit                 |       460 |
| fte, obfs3, obfs4, scramblesuit            |       298 |
| obfs3, obfs4                               |        98 |
| obfs3                                      |        29 |
| scramblesuit                               |        29 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3                               |        13 |
| obfs3, scramblesuit                        |        10 |
| obfs2, obfs3, obfs4                        |         8 |
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

