---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-05-28 07:00 UTC**

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

| Contact                                                                                                                              | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:-------------------------------------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [snaptorg at gmail , com &gt;&gt; bitcoin:1DmvqGnoexBSzSF](endtoend-correlation-groups#snaptorgatgmailcom--bitcoin1dmvqgnoexbszsf)   | 0.15        | 0.15       | 5         | 4               | 2017-05-03     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                         | 0.05        | 0.21       | 2         | 2               | 2017-02-16     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv) | 0.04        | 0.02       | 4         | 4               | 2017-05-25     | 3                           |
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)              | 0.03        | 0.19       | 4         | 4               | 2017-04-13     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                       | 0.03        | 0.32       | 3         | 3               | 2016-08-08     | 1                           |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](endtoend-correlation-groups#tornoisebridgenet-admintornoisebridgenet)        | 0.01        | 1.0        | 9         | 3               | 2017-05-21     | 1                           |
| **Total**                                                                                                                            | **0.31**    | **1.89**   | **27**    |                 |                |                             |

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
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)   |      7.06 |         7 | 2014-04-09   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:EC15DB62D9101481F364DE52EB8313C838BDDC29) |      3.37 |        40 | 2016-08-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:65F9944338C684109EB975D0EC7489B30E191E87)    |      3.32 |         4 | 2014-11-21   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                         |      3.28 |        23 | 2016-01-25   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:1F0D2A44C56F42816DED2022EFD631878C29905B)  |      2.58 |        15 | 2014-05-19   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:8E6EDA78D8E3ABA88D877C3E37D6D4F0938C7B9F) |      2.5  |         6 | 2014-04-08   |
| [sirmatt ksu edu 0x94FBBB0A](https://atlas.torproject.org/#search/family:95880E08A375C62D570B885554CCCFBCCB362660)                            |      2.38 |         4 | 2016-11-02   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:162F7E752504C49A656FF1E9669E0B9572CE4870)                              |      2.26 |         7 | 2015-08-27   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)          |      2.11 |         1 | 2014-04-19   |
| [tor-relay-admin robgjansen com](https://atlas.torproject.org/#search/family:4B1E3276137AD12DCCEBE354EA11C1E47F804F67)                        |      1.98 |         4 | 2015-12-11   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |       1.66 |         7 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.43 |         3 | 2015-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |       1.41 |        40 | 2014-12-23   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |       0.97 |         7 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:CE47F0356D86CF0A1A2008D97623216D560FB0A8)         |       0.89 |        19 | 2015-05-16   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:72B2B12A3F60408BDBC98C6DF53988D3A0B3F0EE) |       0.77 |         5 | 2016-01-03   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:EE5F897C752D46BCFF531641B853FC6BC78DD4A7)                  |       0.76 |        10 | 2014-04-10   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:9C8A123081EFBE022EF795630F447839DDFDDDEC)                      |       0.68 |         7 | 2016-03-10   |
| [45A00F0A](https://atlas.torproject.org/#search/family:45A00F0A6574ADA2B9EA3948590113E7DAA30AAB)                                              |       0.65 |         8 | 2016-07-26   |
| [0x43C4819E Chip Marshall &lt;chip@2bithacker.net&gt;](https://atlas.torproject.org/#search/family:C3F631DE3EC41854168600AE1AE5728A2EA55CBC)  |       0.58 |        10 | 2016-12-23   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:EC116BCB80565A408CE67F8EC3FE3B0B02C3A065)   |            1.693 |      7.06 |       0    |         7 | 2014-04-09   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:8EBB8D1CF48FE2AB95C451DA8F10DB6235F40F8A)    |            1.071 |      0    |       1.66 |         7 | 2014-04-22   |
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:C08DE49658E5B3CFC6F2A952B453C4B608C9A16A)                         |            0.952 |      3.28 |       0.25 |        29 | 2016-01-25   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.921 |      0    |       1.43 |         3 | 2015-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:F349C1663CCF02F6EB479E4D925DE4F3D7F46713)                                 |            0.908 |      0    |       1.41 |        40 | 2014-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:EC15DB62D9101481F364DE52EB8313C838BDDC29) |            0.809 |      3.37 |       0    |        40 | 2016-08-22   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:65F9944338C684109EB975D0EC7489B30E191E87)    |            0.797 |      3.32 |       0    |         4 | 2014-11-21   |
| [sirmatt ksu edu 0x94FBBB0A](https://atlas.torproject.org/#search/family:95880E08A375C62D570B885554CCCFBCCB362660)                            |            0.747 |      2.38 |       0.27 |         9 | 2016-10-02   |
| [gmail is teor2345 http://tor-relays.net PGP C8](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)        |            0.689 |      0.25 |       0.97 |        11 | 2016-08-10   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:1F0D2A44C56F42816DED2022EFD631878C29905B)  |            0.619 |      2.58 |       0    |        15 | 2014-05-19   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.2.9         |             48   |     44.96 |      50.31 |      2894 |
| 0.3.0         |             17.6 |     25.08 |      15.19 |       774 |
| 0.2.5         |              9.4 |      7.85 |       9.64 |      1115 |
| 0.2.7         |              8   |      7.4  |       6.98 |       870 |
| 0.2.8         |              7.6 |      7.09 |       8.03 |       488 |
| 0.2.6         |              4.7 |      1.74 |       6.16 |       336 |
| 0.2.4         |              3.6 |      3.76 |       3.41 |       610 |
| 0.3.1         |              0.7 |      2.08 |       0.24 |        32 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93.6 |      93.3 |       93.3 |      6585 |
| BSD     |              5.9 |       6.1 |        6.3 |       351 |
| Windows |              0.3 |       0.5 |        0.1 |       164 |
| Darwin  |              0   |       0   |        0   |        12 |
| SunOS   |              0   |       0   |        0   |         5 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            18.88 |       17.9 |       17.38 |     22.83 |       613 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     25.19 |            113 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      2134 |
| None                                       |       633 |
| obfs3, obfs4, scramblesuit                 |       461 |
| fte, obfs3, obfs4, scramblesuit            |       298 |
| obfs3, obfs4                               |       102 |
| obfs3                                      |        29 |
| scramblesuit                               |        29 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs2, obfs3                               |        12 |
| obfs3, scramblesuit                        |        11 |
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

