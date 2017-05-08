---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data from: **2017-05-08 22:00 UTC**

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
| [abuse@to-surf-and-protect.net](endtoend-correlation-groups#abuseto-surf-and-protectnet)                                                 |        0.25 |       2.95 |        22 |               9 | 2017-04-27     |                           1 |
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  |        0.18 |       0.06 |         5 |               5 | 2017-04-13     |                           1 |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-btc---14w) |        0.1  |       0.49 |        13 |               2 | 2016-04-01     |                           4 |
| [aTorRelay@gmail.com](endtoend-correlation-groups#atorrelaygmailcom)                                                                     |        0.09 |       0.13 |         9 |               6 | 2017-03-21     |                           1 |
| [tor@schlarman.org - 15icgtSewYphZqN1tr9H22sbaVkQiU](endtoend-correlation-groups#torschlarmanorg---15icgtsewyphzqn1tr9h22sbavkqiu)       |        0.06 |       0.17 |         2 |               2 | 2017-04-30     |                           1 |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             |        0.03 |       0.27 |         2 |               2 | 2017-02-16     |                           1 |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           |        0.03 |       0.62 |         3 |               3 | 2016-08-08     |                           1 |
| [George Shuklin &lt;george.shuklin@gmail.com&gt;](endtoend-correlation-groups#george-shuklin-georgeshuklingmailcom)                      |        0.03 |       0.02 |         2 |               2 | 2016-07-21     |                           1 |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](endtoend-correlation-groups#tornoisebridgenet-admintornoisebridgenet)            |        0.01 |       0.87 |         5 |               2 | 2015-05-20     |                           1 |

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
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://compass.torproject.org/#?top=-1&family=EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)      |      4.82 |         7 | 2014-04-09   |
| [abuse@to-surf-and-protect.net](https://compass.torproject.org/#?top=-1&family=C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                            |      3.28 |        18 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://compass.torproject.org/#?top=-1&family=EC15DB62D9101481F364DE52EB8313C838BDDC29)    |      2.43 |        31 | 2016-08-22   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://compass.torproject.org/#?top=-1&family=8E6EDA78D8E3ABA88D877C3E37D6D4F0938C7B9F)    |      2.21 |         6 | 2014-04-08   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://compass.torproject.org/#?top=-1&family=65F9944338C684109EB975D0EC7489B30E191E87)       |      2.18 |         4 | 2014-11-21   |
| [3DC5B80B](https://atlas.torproject.org/#details/3DC5B80B0FBB7F88B709CB4C388D9CE8D21EF3DC)                                                          |      1.93 |         1 | 2017-04-22   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://compass.torproject.org/#?top=-1&family=2B44FD1742D26E4F28D4CACF1F0CF8A686270E45)     |      1.86 |        20 | 2014-05-19   |
| [abuse aT nectodoT--onion](https://compass.torproject.org/#?top=-1&family=162F7E752504C49A656FF1E9669E0B9572CE4870)                                 |      1.84 |         7 | 2015-08-27   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://compass.torproject.org/#?top=-1&family=38A42B8D7C0E6346F4A4821617740AEE86EA885B) |      1.78 |         3 | 2014-11-04   |
| [&lt;zwiebeln at online de&gt; please donate BTC 1K38x9xq](https://compass.torproject.org/#?top=-1&family=53018DB58301743267F057340C51C3151135F13F) |      1.78 |        34 | 2016-09-16   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                               |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://compass.torproject.org/#?top=-1&family=8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |       1.49 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://compass.torproject.org/#?top=-1&family=F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |       1.17 |        40 | 2014-12-23   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://compass.torproject.org/#?top=-1&family=1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |       1.13 |         7 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://compass.torproject.org/#?top=-1&family=CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |       0.99 |        18 | 2015-05-16   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://compass.torproject.org/#?top=-1&family=B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       0.94 |         3 | 2015-04-22   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://compass.torproject.org/#?top=-1&family=EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |       0.83 |        10 | 2014-04-10   |
| [tor at fiberoverethernet dot com](https://compass.torproject.org/#?top=-1&family=9C8A123081EFBE022EF795630F447839DDFDDDEC)                      |       0.74 |         6 | 2016-03-10   |
| [45A00F0A](https://compass.torproject.org/#?top=-1&family=45A00F0A6574ADA2B9EA3948590113E7DAA30AAB)                                              |       0.7  |         8 | 2016-07-26   |
| [Hello, I am a Tor node My nickname: https://youtu](https://compass.torproject.org/#?top=-1&family=0ED06F12AF64D5027422169B61D1AC5366C6FFE9)     |       0.66 |        17 | 2014-11-17   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://compass.torproject.org/#?top=-1&family=72B2B12A3F60408BDBC98C6DF53988D3A0B3F0EE) |       0.65 |         5 | 2016-01-03   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                               |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://compass.torproject.org/#?top=-1&family=EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)   |            1.163 |      4.82 |       0    |         7 | 2014-04-09   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://compass.torproject.org/#?top=-1&family=8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |            0.975 |      0    |       1.49 |         7 | 2014-04-22   |
| [abuse@to-surf-and-protect.net](https://compass.torproject.org/#?top=-1&family=C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                         |            0.958 |      3.28 |       0.25 |        24 | 2016-01-25   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://compass.torproject.org/#?top=-1&family=1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |            0.804 |      0.25 |       1.13 |        11 | 2016-08-10   |
| [monitor0penmailbox0rg](https://compass.torproject.org/#?top=-1&family=F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |            0.769 |      0    |       1.17 |        40 | 2014-12-23   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://compass.torproject.org/#?top=-1&family=CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |            0.651 |      0    |       0.99 |        19 | 2015-05-16   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://compass.torproject.org/#?top=-1&family=B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.616 |      0    |       0.94 |         3 | 2015-04-22   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://compass.torproject.org/#?top=-1&family=EC15DB62D9101481F364DE52EB8313C838BDDC29) |            0.587 |      2.43 |       0    |        31 | 2016-08-22   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://compass.torproject.org/#?top=-1&family=EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |            0.546 |      0    |       0.83 |        10 | 2014-04-10   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://compass.torproject.org/#?top=-1&family=8E6EDA78D8E3ABA88D877C3E37D6D4F0938C7B9F) |            0.533 |      2.21 |       0    |         6 | 2014-04-08   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.2.9         |             54.2 |     53.89 |      55.07 |      3104 |
| 0.3.0         |             12   |     21.87 |       9.28 |       568 |
| 0.2.5         |              8.9 |      4.96 |       9.85 |      1133 |
| 0.2.7         |              7.8 |      6.58 |       7.13 |       882 |
| 0.2.8         |              7.5 |      5.72 |       8.34 |       556 |
| 0.2.6         |              5.1 |      1.94 |       6.59 |       360 |
| 0.2.4         |              3.5 |      2.65 |       3.52 |       650 |
| 0.3.1         |              0.6 |      2.36 |       0.17 |        20 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93.7 |      95.1 |       92.8 |      6701 |
| BSD     |              5.8 |       4.5 |        6.8 |       366 |
| Windows |              0.2 |       0.3 |        0.1 |       173 |
| SunOS   |              0.1 |       0   |        0.2 |         6 |
| Darwin  |              0   |       0   |        0   |        14 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.27 |      17.72 |       14.96 |     24.36 |       614 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     25.83 |            119 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      2128 |
| None                                       |       623 |
| obfs3, obfs4, scramblesuit                 |       459 |
| fte, obfs3, obfs4, scramblesuit            |       298 |
| obfs3, obfs4                               |        96 |
| scramblesuit                               |        29 |
| obfs3                                      |        28 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3                               |        13 |
| obfs3, scramblesuit                        |        11 |
| obfs2, obfs3, obfs4                        |         8 |
| fte, obfs3, obfs4                          |         6 |
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

