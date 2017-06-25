---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-06-25 16:00 UTC**

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
| [snaptorg at gmail , com &gt;&gt; bitcoin:1DmvqGnoexBSzSF](endtoend-correlation-groups#snaptorgatgmailcom--bitcoin1dmvqgnoexbszsf)       | 0.27        | 0.15       | 5         | 4               | 2017-05-03     | 1                           |
| [yscoder@foxmail.com](endtoend-correlation-groups#yscoderfoxmailcom)                                                                     | 0.12        | 0.03       | 4         | 2               | 2017-06-08     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-btc---14w) | 0.11        | 0.67       | 12        | 2               | 2016-04-01     | 4                           |
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.08        | 0.13       | 4         | 4               | 2017-04-13     | 1                           |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](endtoend-correlation-groups#tornoisebridgenet-admintornoisebridgenet)            | 0.04        | 3.83       | 9         | 3               | 2017-05-21     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)     | 0.03        | 0.08       | 4         | 4               | 2017-05-25     | 3                           |
| [Abuse Department &lt;abuse AT hartvoorinternetvrijhei](endtoend-correlation-groups#abuse-department-abuse-at-hartvoorinternetvrijhei)   | 0.02        | 1.21       | 2         | 2               | 2015-09-06     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           | 0.02        | 0.35       | 3         | 3               | 2016-08-08     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                     | 0.01        | 0.27       | 3         | 2               | 2016-08-28     | 1                           |
| **Total**                                                                                                                                | **0.70**    | **6.72**   | **46**    |                 |                |                             |

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
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)   |      5.98 |         7 | 2014-04-09   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |      5.83 |         9 | 2014-02-13   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                         |      3.64 |        25 | 2016-01-25   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:65F9944338C684109EB975D0EC7489B30E191E87)    |      3.46 |         4 | 2014-11-21   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://atlas.torproject.org/#search/family:8175A86D8896CEA37FDC67311F9BDC1DDCBE8136) |      2.91 |         4 | 2017-05-20   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:162F7E752504C49A656FF1E9669E0B9572CE4870)                              |      2.43 |         7 | 2015-08-27   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:8E6EDA78D8E3ABA88D877C3E37D6D4F0938C7B9F) |      2.24 |         6 | 2014-04-08   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C90CA3B7FE01A146B8268D56977DC4A2C024B9EA)                                 |      2.02 |         6 | 2016-04-02   |
| [sirmatt ksu edu 0x94FBBB0A](https://atlas.torproject.org/#search/family:95880E08A375C62D570B885554CCCFBCCB362660)                            |      1.83 |         4 | 2016-11-02   |
| [tor-relay-admin robgjansen com](https://atlas.torproject.org/#search/family:4B1E3276137AD12DCCEBE354EA11C1E47F804F67)                        |      1.82 |         3 | 2015-12-11   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.49 |         3 | 2015-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |       1.24 |        35 | 2014-12-23   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |       0.97 |         7 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |       0.92 |        20 | 2015-05-16   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:72B2B12A3F60408BDBC98C6DF53988D3A0B3F0EE) |       0.85 |         5 | 2016-01-03   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |       0.82 |        10 | 2014-04-10   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:1D3174338A1131A53E098443E76E1103CDED00DC) |       0.79 |         6 | 2016-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |       0.66 |         5 | 2014-04-22   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:9C8A123081EFBE022EF795630F447839DDFDDDEC)                      |       0.65 |         6 | 2016-03-10   |
| [see https://www.artikel5ev.de/torcontact/](https://atlas.torproject.org/#search/family:035D2E216B065B961E404BD172336050E5AF4EEA)             |       0.6  |        11 | 2016-09-05   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |            1.758 |      5.83 |       0.79 |        15 | 2014-02-13   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)   |            1.257 |      5.98 |       0    |         7 | 2014-04-09   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |            0.998 |      0    |       0.66 |         7 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.994 |      0    |       1.49 |         3 | 2015-04-22   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                         |            0.914 |      3.64 |       0.21 |        31 | 2016-01-25   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |            0.863 |      0    |       1.24 |        40 | 2014-12-23   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |            0.736 |      0.4  |       0.97 |        10 | 2016-08-10   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:65F9944338C684109EB975D0EC7489B30E191E87)    |            0.729 |      3.46 |       0    |         4 | 2014-11-21   |
| [sirmatt ksu edu 0x94FBBB0A](https://atlas.torproject.org/#search/family:95880E08A375C62D570B885554CCCFBCCB362660)                            |            0.626 |      1.83 |       0.21 |        11 | 2015-06-01   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |            0.616 |      0    |       0.92 |        20 | 2015-05-16   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.2.9         |             48.3 |     43.83 |      50.17 |      3030 |
| 0.3.0         |             20.4 |     28.64 |      18.24 |      1009 |
| 0.2.5         |              9.3 |      8.4  |       8.88 |      1038 |
| 0.2.7         |              7.3 |      5.27 |       7.46 |       835 |
| 0.2.8         |              6.5 |      6.17 |       6.98 |       404 |
| 0.2.4         |              3.1 |      2.45 |       3.26 |       614 |
| 0.2.6         |              3.1 |      1.28 |       3.95 |       229 |
| 0.3.1         |              1.3 |      2.71 |       1.02 |        66 |
| 0.3.2         |              0.2 |      1.21 |       0    |         3 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.7 |      91.5 |       92.4 |      6631 |
| BSD     |              6.7 |       7.9 |        7   |       358 |
| Windows |              0.3 |       0.5 |        0.1 |       206 |
| SunOS   |              0.1 |       0   |        0.1 |         4 |
| Darwin  |              0   |       0   |        0   |        13 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            17.93 |      17.15 |       14.67 |     25.51 |       607 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     28.74 |            122 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1904 |
| None                                       |       633 |
| obfs3, obfs4, scramblesuit                 |       473 |
| obfs3, obfs4                               |        88 |
| fte, obfs3, obfs4, scramblesuit            |        48 |
| obfs3                                      |        28 |
| scramblesuit                               |        23 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3                               |        12 |
| obfs3, scramblesuit                        |        11 |
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

