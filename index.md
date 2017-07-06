---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-07-06 16:00 UTC**

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
| [see https://www.artikel5ev.de/torcontact/](endtoend-correlation-groups#see-httpswwwartikel5evdetorcontact)                            | 0.5         | 0.32       | 13        | 9               | 2017-04-27     | 1                           |
| [torrelays A-T cyb3rwr3ck D-O-T net](endtoend-correlation-groups#torrelays-a-t-cyb3rwr3ck-d-o-t-net)                                   | 0.09        | 0.01       | 3         | 2               | 2017-06-15     | 1                           |
| [yscoder@foxmail.com](endtoend-correlation-groups#yscoderfoxmailcom)                                                                   | 0.08        | 0.04       | 3         | 2               | 2017-06-08     | 1                           |
| [George Shuklin &lt;george.shuklin@gmail.com&gt;](endtoend-correlation-groups#george-shuklin-georgeshuklingmailcom)                    | 0.05        | 0.02       | 2         | 2               | 2016-07-21     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)   | 0.04        | 0.08       | 4         | 4               | 2017-05-25     | 3                           |
| [Abuse Department &lt;abuse AT hartvoorinternetvrijhei](endtoend-correlation-groups#abuse-department-abuse-at-hartvoorinternetvrijhei) | 0.03        | 1.56       | 2         | 2               | 2015-09-06     | 1                           |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](endtoend-correlation-groups#tornoisebridgenet-admintornoisebridgenet)          | 0.03        | 2.11       | 5         | 2               | 2017-05-21     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                         | 0.03        | 0.5        | 3         | 3               | 2016-08-08     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                   | 0.01        | 0.23       | 3         | 2               | 2016-08-28     | 1                           |
| [https://freebogatov.org](endtoend-correlation-groups#httpsfreebogatovorg)                                                             | 0.01        | 0.01       | 2         | 2               | 2017-05-09     | 1                           |
| **Total**                                                                                                                              | **0.87**    | **4.88**   | **40**    |                 |                |                             |

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
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |      6.61 |         9 | 2014-02-13   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                         |      4.59 |        26 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)   |      4.13 |         7 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:65F9944338C684109EB975D0EC7489B30E191E87)    |      3.08 |         4 | 2014-11-21   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:2B44FD1742D26E4F28D4CACF1F0CF8A686270E45)  |      2.89 |        20 | 2014-05-19   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:8E6EDA78D8E3ABA88D877C3E37D6D4F0938C7B9F) |      2.43 |         6 | 2014-04-08   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:162F7E752504C49A656FF1E9669E0B9572CE4870)                              |      2.28 |         7 | 2015-08-27   |
| [29C92C85](https://atlas.torproject.org/#details/29C92C854E0F6652A77F3A8B231D6932993969E8)                                                    |      2.16 |         1 | 2017-04-10   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://atlas.torproject.org/#search/family:8175A86D8896CEA37FDC67311F9BDC1DDCBE8136) |      2.11 |         4 | 2017-05-20   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C90CA3B7FE01A146B8268D56977DC4A2C024B9EA)                                 |      1.99 |         6 | 2016-04-02   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |       1.86 |         7 | 2014-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |       1.72 |        37 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.49 |         3 | 2015-04-22   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |       1.33 |         7 | 2016-08-10   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |       1.24 |         6 | 2016-12-23   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |       1.1  |        21 | 2015-05-16   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:9C8A123081EFBE022EF795630F447839DDFDDDEC)                      |       0.89 |         6 | 2016-03-10   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |       0.73 |        10 | 2014-04-10   |
| [nibbler &lt;nibbler dash tor dash mail at geekbox.inf](https://atlas.torproject.org/#details/9BF04559224F0F1C3C953D641F1744AF0192543A)       |       0.68 |         1 | 2013-09-19   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:72B2B12A3F60408BDBC98C6DF53988D3A0B3F0EE) |       0.68 |         5 | 2016-01-03   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |            2.3   |      6.61 |       1.24 |        15 | 2014-02-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |            1.199 |      0    |       1.86 |         7 | 2014-04-22   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                         |            1.183 |      4.59 |       0.2  |        32 | 2016-01-25   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |            1.129 |      0    |       1.72 |        40 | 2014-12-23   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.964 |      0    |       1.49 |         3 | 2015-04-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)   |            0.951 |      4.13 |       0    |         7 | 2014-04-09   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |            0.93  |      0.29 |       1.33 |        10 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |            0.722 |      0    |       1.1  |        22 | 2015-05-16   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:65F9944338C684109EB975D0EC7489B30E191E87)    |            0.699 |      3.08 |       0    |         4 | 2014-11-21   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:2B44FD1742D26E4F28D4CACF1F0CF8A686270E45)  |            0.659 |      2.89 |       0    |        20 | 2014-05-19   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.2.9         |             41.9 |     35.69 |      43.99 |      2597 |
| 0.3.0         |             29.5 |     36.05 |      29.1  |      1547 |
| 0.2.5         |              9   |      9.65 |       8.46 |      1022 |
| 0.2.7         |              6.9 |      3.99 |       6.86 |       825 |
| 0.2.8         |              5.8 |      5.36 |       5.98 |       352 |
| 0.2.4         |              3   |      3.59 |       2.7  |       594 |
| 0.3.1         |              2.3 |      2.89 |       2.31 |       104 |
| 0.2.6         |              0.7 |      0.41 |       0.74 |        97 |
| 0.3.2         |              0.7 |      3.29 |       0.04 |        11 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93.6 |      94.2 |       92.9 |      6587 |
| BSD     |              6.2 |       6.6 |        6.7 |       349 |
| Windows |              0.1 |       0   |        0.1 |       179 |
| Darwin  |              0   |       0   |        0.1 |        12 |
| SunOS   |              0   |       0   |        0.1 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.53 |      18.78 |       15.83 |     22.75 |       605 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     26.29 |            131 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1812 |
| None                                       |       640 |
| obfs3, obfs4, scramblesuit                 |       476 |
| obfs3, obfs4                               |        86 |
| fte, obfs3, obfs4, scramblesuit            |        48 |
| obfs3                                      |        24 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| scramblesuit                               |        19 |
| obfs2, obfs3                               |        12 |
| obfs3, scramblesuit                        |        10 |
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

