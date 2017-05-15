---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-05-15 03:00 UTC**

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
| [aTorRelay@gmail.com](endtoend-correlation-groups#atorrelaygmailcom)                                                                     | 0.19        | 0.14       | 9         | 6               | 2017-03-21     | 1                           |
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.16        | 0.12       | 4         | 4               | 2017-04-13     | 1                           |
| [snaptorg at gmail , com &gt;&gt; bitcoin:1DmvqGnoexBSzSF](endtoend-correlation-groups#snaptorgatgmailcom--bitcoin1dmvqgnoexbszsf)       | 0.16        | 0.13       | 5         | 4               | 2017-05-03     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-btc---14w) | 0.1         | 0.58       | 13        | 2               | 2016-04-01     | 4                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.04        | 0.23       | 2         | 2               | 2017-02-16     | 1                           |
| [George Shuklin &lt;george.shuklin@gmail.com&gt;](endtoend-correlation-groups#george-shuklin-georgeshuklingmailcom)                      | 0.02        | 0.01       | 2         | 2               | 2016-07-21     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           | 0.02        | 0.5        | 3         | 3               | 2016-08-08     | 1                           |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](endtoend-correlation-groups#tornoisebridgenet-admintornoisebridgenet)            | 0.01        | 0.88       | 5         | 2               | 2015-05-20     | 1                           |
| [torman@memeware.net](endtoend-correlation-groups#tormanmemewarenet)                                                                     | 0.01        | 0.07       | 2         | 2               | 2017-05-11     | 1                           |
|                                                                                                                                          | **0.71**    | **2.66**   | **45**    |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).

## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                                  |   Exit(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://compass.torproject.org/#?top=-1&family=C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                            |      4.85 |        25 | 2016-01-25   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://compass.torproject.org/#?top=-1&family=2B44FD1742D26E4F28D4CACF1F0CF8A686270E45)     |      2.96 |        19 | 2014-05-19   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://compass.torproject.org/#?top=-1&family=65F9944338C684109EB975D0EC7489B30E191E87)       |      2.5  |         4 | 2014-11-21   |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](https://compass.torproject.org/#?top=-1&family=53018DB58301743267F057340C51C3151135F13F) |      2.27 |        34 | 2016-09-16   |
| [abuse aT nectodoT--onion](https://compass.torproject.org/#?top=-1&family=162F7E752504C49A656FF1E9669E0B9572CE4870)                                 |      2.19 |         7 | 2015-08-27   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://compass.torproject.org/#?top=-1&family=8E6EDA78D8E3ABA88D877C3E37D6D4F0938C7B9F)    |      2.12 |         6 | 2014-04-08   |
| [3DC5B80B](https://atlas.torproject.org/#details/3DC5B80B0FBB7F88B709CB4C388D9CE8D21EF3DC)                                                          |      1.81 |         1 | 2017-04-22   |
| [tor-relay-admin robgjansen com](https://compass.torproject.org/#?top=-1&family=4B1E3276137AD12DCCEBE354EA11C1E47F804F67)                           |      1.58 |         4 | 2015-12-11   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://compass.torproject.org/#?top=-1&family=38A42B8D7C0E6346F4A4821617740AEE86EA885B) |      1.57 |         3 | 2014-11-04   |
| [sirmatt ksu edu 0x94FBBB0A](https://compass.torproject.org/#?top=-1&family=95880E08A375C62D570B885554CCCFBCCB362660)                               |      1.57 |         4 | 2016-11-02   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://compass.torproject.org/#?top=-1&family=8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |       1.51 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://compass.torproject.org/#?top=-1&family=F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |       1.28 |        40 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://compass.torproject.org/#?top=-1&family=B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.09 |         3 | 2015-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://compass.torproject.org/#?top=-1&family=CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |       1.05 |        19 | 2015-05-16   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://compass.torproject.org/#?top=-1&family=1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |       0.99 |         7 | 2016-08-10   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://compass.torproject.org/#?top=-1&family=EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |       0.79 |        10 | 2014-04-10   |
| [45A00F0A](https://compass.torproject.org/#?top=-1&family=45A00F0A6574ADA2B9EA3948590113E7DAA30AAB)                                              |       0.78 |         8 | 2016-07-26   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://compass.torproject.org/#?top=-1&family=72B2B12A3F60408BDBC98C6DF53988D3A0B3F0EE) |       0.77 |         5 | 2016-01-03   |
| [tor at fiberoverethernet dot com](https://compass.torproject.org/#?top=-1&family=9C8A123081EFBE022EF795630F447839DDFDDDEC)                      |       0.76 |         6 | 2016-03-10   |
| [Hello, I am a Tor node My nickname: https://youtu](https://compass.torproject.org/#?top=-1&family=0ED06F12AF64D5027422169B61D1AC5366C6FFE9)     |       0.63 |        17 | 2014-11-17   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                  |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://compass.torproject.org/#?top=-1&family=C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                            |            1.287 |      4.85 |       0.32 |        31 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://compass.torproject.org/#?top=-1&family=8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)       |            1.012 |      0    |       1.51 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://compass.torproject.org/#?top=-1&family=F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                    |            0.853 |      0    |       1.28 |        40 | 2014-12-23   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://compass.torproject.org/#?top=-1&family=1A4488A367D89D0EFDA88116059FEBCACF0F508A)           |            0.737 |      0.33 |       0.99 |        11 | 2016-08-10   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://compass.torproject.org/#?top=-1&family=B204DE75B37064EF6A4C6BAF955C5724578D0B32)                      |            0.729 |      0    |       1.09 |         3 | 2015-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://compass.torproject.org/#?top=-1&family=CE47F0356D86CF0A1A2008D97623216D560FB0A8)            |            0.702 |      0    |       1.05 |        19 | 2015-05-16   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://compass.torproject.org/#?top=-1&family=2B44FD1742D26E4F28D4CACF1F0CF8A686270E45)     |            0.652 |      2.96 |       0    |        19 | 2014-05-19   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://compass.torproject.org/#?top=-1&family=65F9944338C684109EB975D0EC7489B30E191E87)       |            0.552 |      2.5  |       0    |         4 | 2014-11-21   |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](https://compass.torproject.org/#?top=-1&family=53018DB58301743267F057340C51C3151135F13F) |            0.549 |      2.27 |       0.07 |        36 | 2016-08-28   |
| [see https://www.artikel5ev.de/torcontact/](https://compass.torproject.org/#?top=-1&family=035D2E216B065B961E404BD172336050E5AF4EEA)                |            0.545 |      0.67 |       0.57 |        21 | 2014-04-08   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.2.9         |             52   |     47.33 |      54.01 |      2997 |
| 0.3.0         |             13.6 |     24.87 |      10.83 |       653 |
| 0.2.5         |              9   |      5.31 |       9.99 |      1121 |
| 0.2.7         |              8   |      7.58 |       6.77 |       862 |
| 0.2.8         |              7.7 |      7.1  |       8.15 |       525 |
| 0.2.6         |              5.3 |      2.14 |       6.86 |       349 |
| 0.2.4         |              3.5 |      3.39 |       3.22 |       590 |
| 0.3.1         |              0.6 |      2.24 |       0.14 |        21 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93.3 |      94.9 |       92.7 |      6560 |
| BSD     |              6.2 |       4.5 |        6.9 |       396 |
| Windows |              0.2 |       0.4 |        0.1 |       144 |
| SunOS   |              0.1 |       0   |        0.1 |         5 |
| Darwin  |              0   |       0   |        0   |        12 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            17.94 |      17.83 |       15.27 |     22.86 |       642 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     24.32 |            112 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      2168 |
| None                                       |       631 |
| obfs3, obfs4, scramblesuit                 |       460 |
| fte, obfs3, obfs4, scramblesuit            |       298 |
| obfs3, obfs4                               |        99 |
| obfs3                                      |        29 |
| scramblesuit                               |        29 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3                               |        13 |
| obfs3, scramblesuit                        |        11 |
| obfs2, obfs3, obfs4                        |         8 |
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

