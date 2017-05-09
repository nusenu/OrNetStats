---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-05-09 22:00 UTC**

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

| Contact                                                                                                                                  |   Guard (%) |   Exit (%) |   #Relays |   /16 Netblocks | Newest Relay   |   Eff. Family Members (min) |
|:-----------------------------------------------------------------------------------------------------------------------------------------|------------:|-----------:|----------:|----------------:|:---------------|----------------------------:|
| [abuse@to-surf-and-protect.net](endtoend-correlation-groups#abuseto-surf-and-protectnet)                                                 |        0.24 |       3.15 |        22 |               9 | 2017-04-27     |                           1 |
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  |        0.19 |       0.08 |         5 |               5 | 2017-04-13     |                           1 |
| [aTorRelay@gmail.com](endtoend-correlation-groups#atorrelaygmailcom)                                                                     |        0.13 |       0.14 |         9 |               6 | 2017-03-21     |                           1 |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-btc---14w) |        0.13 |       0.54 |        13 |               2 | 2016-04-01     |                           4 |
| [tor@schlarman.org - 15icgtSewYphZqN1tr9H22sbaVkQiU](endtoend-correlation-groups#torschlarmanorg---15icgtsewyphzqn1tr9h22sbavkqiu)       |        0.09 |       0.15 |         2 |               2 | 2017-04-30     |                           1 |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             |        0.03 |       0.3  |         2 |               2 | 2017-02-16     |                           1 |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           |        0.02 |       0.5  |         3 |               3 | 2016-08-08     |                           1 |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](endtoend-correlation-groups#tornoisebridgenet-admintornoisebridgenet)            |        0.01 |       0.97 |         5 |               2 | 2015-05-20     |                           1 |

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
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://compass.torproject.org/#?top=-1&family=EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)      |      5.14 |         7 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://compass.torproject.org/#?top=-1&family=C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                            |      3.43 |        18 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://compass.torproject.org/#?top=-1&family=EC15DB62D9101481F364DE52EB8313C838BDDC29)    |      2.62 |        31 | 2016-08-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://compass.torproject.org/#?top=-1&family=65F9944338C684109EB975D0EC7489B30E191E87)       |      2.24 |         4 | 2014-11-21   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://compass.torproject.org/#?top=-1&family=8E6EDA78D8E3ABA88D877C3E37D6D4F0938C7B9F)    |      2.24 |         6 | 2014-04-08   |
| [abuse aT nectodoT--onion](https://compass.torproject.org/#?top=-1&family=162F7E752504C49A656FF1E9669E0B9572CE4870)                                 |      2.15 |         7 | 2015-08-27   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://compass.torproject.org/#?top=-1&family=2B44FD1742D26E4F28D4CACF1F0CF8A686270E45)     |      1.92 |        20 | 2014-05-19   |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](https://compass.torproject.org/#?top=-1&family=53018DB58301743267F057340C51C3151135F13F) |      1.85 |        34 | 2016-09-16   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://compass.torproject.org/#?top=-1&family=38A42B8D7C0E6346F4A4821617740AEE86EA885B) |      1.68 |         3 | 2014-11-04   |
| [6E5A0949](https://atlas.torproject.org/#details/6E5A09493DF5E23579B94D16FBA8ADCC75833144)                                                          |      1.56 |         1 | 2017-04-27   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://compass.torproject.org/#?top=-1&family=8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |       1.41 |         7 | 2014-04-22   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://compass.torproject.org/#?top=-1&family=1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |       1.18 |         7 | 2016-08-10   |
| [monitor0penmailbox0rg](https://compass.torproject.org/#?top=-1&family=F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |       1.18 |        40 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://compass.torproject.org/#?top=-1&family=B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.01 |         3 | 2015-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://compass.torproject.org/#?top=-1&family=CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |       0.97 |        18 | 2015-05-16   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://compass.torproject.org/#?top=-1&family=EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |       0.84 |        10 | 2014-04-10   |
| [tor at fiberoverethernet dot com](https://compass.torproject.org/#?top=-1&family=9C8A123081EFBE022EF795630F447839DDFDDDEC)                      |       0.74 |         6 | 2016-03-10   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://compass.torproject.org/#?top=-1&family=72B2B12A3F60408BDBC98C6DF53988D3A0B3F0EE) |       0.67 |         5 | 2016-01-03   |
| [45A00F0A](https://compass.torproject.org/#?top=-1&family=45A00F0A6574ADA2B9EA3948590113E7DAA30AAB)                                              |       0.67 |         8 | 2016-07-26   |
| [Hello, I am a Tor node My nickname: https://youtu](https://compass.torproject.org/#?top=-1&family=0ED06F12AF64D5027422169B61D1AC5366C6FFE9)     |       0.66 |        17 | 2014-11-17   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                               |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://compass.torproject.org/#?top=-1&family=EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)   |            1.231 |      5.14 |       0    |         7 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://compass.torproject.org/#?top=-1&family=C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                         |            0.983 |      3.43 |       0.24 |        24 | 2016-01-25   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://compass.torproject.org/#?top=-1&family=8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |            0.931 |      0    |       1.41 |         7 | 2014-04-22   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://compass.torproject.org/#?top=-1&family=1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |            0.842 |      0.25 |       1.18 |        11 | 2016-08-10   |
| [monitor0penmailbox0rg](https://compass.torproject.org/#?top=-1&family=F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |            0.777 |      0    |       1.18 |        40 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://compass.torproject.org/#?top=-1&family=B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.664 |      0    |       1.01 |         3 | 2015-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://compass.torproject.org/#?top=-1&family=CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |            0.644 |      0    |       0.97 |        19 | 2015-05-16   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://compass.torproject.org/#?top=-1&family=EC15DB62D9101481F364DE52EB8313C838BDDC29) |            0.627 |      2.62 |       0    |        31 | 2016-08-22   |
| [sirmatt ksu edu 0x94FBBB0A](https://compass.torproject.org/#?top=-1&family=95880E08A375C62D570B885554CCCFBCCB362660)                            |            0.599 |      1.35 |       0.41 |         9 | 2016-10-02   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://compass.torproject.org/#?top=-1&family=EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |            0.555 |      0    |       0.84 |        10 | 2014-04-10   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.2.9         |             53.8 |     53.18 |      54.71 |      3096 |
| 0.3.0         |             12.4 |     22.38 |       9.81 |       588 |
| 0.2.5         |              8.8 |      4.38 |       9.83 |      1136 |
| 0.2.7         |              7.8 |      6.76 |       7.17 |       865 |
| 0.2.8         |              7.5 |      6.14 |       8.25 |       546 |
| 0.2.6         |              5.1 |      2.06 |       6.63 |       357 |
| 0.2.4         |              3.5 |      2.74 |       3.41 |       634 |
| 0.3.1         |              0.6 |      2.31 |       0.14 |        22 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93.5 |      94.8 |       92.6 |      6677 |
| BSD     |              6   |       4.7 |        7   |       370 |
| Windows |              0.2 |       0.3 |        0.1 |       163 |
| SunOS   |              0.1 |       0   |        0.1 |         5 |
| Darwin  |              0   |       0   |        0   |        15 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.52 |      17.75 |       15.25 |     24.92 |       610 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     26.36 |            121 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      2118 |
| None                                       |       624 |
| obfs3, obfs4, scramblesuit                 |       459 |
| fte, obfs3, obfs4, scramblesuit            |       298 |
| obfs3, obfs4                               |        98 |
| scramblesuit                               |        29 |
| obfs3                                      |        29 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3                               |        14 |
| obfs3, scramblesuit                        |        11 |
| obfs2, obfs3, obfs4                        |         8 |
| fte, obfs3, obfs4                          |         4 |
| meek                                       |         4 |
| snowflake                                  |         2 |
| obfs4, scramblesuit                        |         2 |
| obfs2, obfs3, obfs4, scramblesuit          |         2 |
| fte, obfs3                                 |         1 |
| obfs3 websocket, websocket                 |         1 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

