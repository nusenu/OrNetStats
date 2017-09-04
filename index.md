---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-09-04 17:00 UTC**

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
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.12        | 0.14       | 4         | 3               | 2017-08-14     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb) | 0.08        | 0.66       | 13        | 2               | 2016-04-01     | 4                           |
| [George Shuklin &lt;george.shuklin@gmail.com&gt;](endtoend-correlation-groups#george-shuklin-georgeshuklingmailcom)                      | 0.04        | 0.01       | 2         | 2               | 2016-07-21     | 1                           |
| [Syncaddict &lt;tor-node-operations@syncaddict.net&gt;](endtoend-correlation-groups#syncaddict-tor-node-operationssyncaddictnet)         | 0.03        | 0.01       | 2         | 2               | 2017-08-09     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           | 0.03        | 0.44       | 3         | 3               | 2016-08-08     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                           | 0.02        | 0.43       | 5         | 2               | 2017-06-23     | 1                           |
| [&lt;hostmaster at denetron dot com&gt;](endtoend-correlation-groups#hostmaster-at-denetron-dot-com)                                     | 0.01        | 0.38       | 3         | 2               | 2016-08-28     | 1                           |
| [Brandon Kuschel &lt;kusch023 AT nospam UMN dot edu.](endtoend-correlation-groups#brandon-kuschel-kusch023-at-nospam-umn-dot-edu)        | 0.01        | 0.03       | 2         | 2               | 2016-10-26     | 1                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)     | 0.01        | 0.35       | 3         | 3               | 2017-08-23     | 1                           |
| **Total**                                                                                                                                | **0.35**    | **2.45**   | **37**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      5.97 |        20 | 2016-01-25   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      3.09 |         4 | 2014-11-21   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      2.81 |         5 | 2014-04-09   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:9BA84E8C90083676F86C7427C8D105925F13716C)    |      2.61 |         6 | 2014-04-08   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.35 |         3 | 2014-11-04   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.35 |         1 | 2014-04-19   |
| [29C92C85](https://atlas.torproject.org/#details/29C92C854E0F6652A77F3A8B231D6932993969E8)                                                       |      2.27 |         1 | 2017-04-10   |
| [abuse aT nectodoT--onion](https://atlas.torproject.org/#search/family:B2AFC9DB441202EEFEC8592456311759698A6927)                                 |      2.05 |         7 | 2015-08-27   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                    |      1.98 |         6 | 2016-04-02   |
| [Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt;](https://atlas.torproject.org/#search/family:3EAAAB35932610411E24FA4317603CB5780B80BC)     |      1.95 |        18 | 2014-05-19   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       1.37 |        21 | 2015-05-16   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.32 |         6 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.31 |         3 | 2015-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |       1.15 |        24 | 2014-12-23   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       1.01 |         7 | 2016-08-10   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:8672E8A01B4D3FA4C0BBE21C740D4506302EA487)                      |       0.96 |         6 | 2016-03-10   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)    |       0.81 |         5 | 2016-12-23   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       0.79 |         7 | 2016-01-03   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |       0.69 |         8 | 2016-07-26   |
| [noc@cymru.com](https://atlas.torproject.org/#search/family:896FCE19CB53A73A21DC874977C06B28FC9A8BBA)                                         |       0.63 |         6 | 2011-11-29   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.487 |      5.97 |       0.4  |        28 | 2016-01-25   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |            0.933 |      1.93 |       0.81 |         8 | 2014-02-13   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.915 |      0    |       1.37 |        22 | 2015-05-16   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.868 |      0    |       1.32 |         6 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.867 |      0    |       1.31 |         3 | 2015-04-22   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.791 |      0    |       1.15 |        26 | 2014-12-23   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.756 |      0.42 |       1.01 |         8 | 2016-08-10   |
| [tor at fiberoverethernet dot com](https://atlas.torproject.org/#search/family:8672E8A01B4D3FA4C0BBE21C740D4506302EA487)                      |            0.641 |      0    |       0.96 |         8 | 2016-03-10   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)    |            0.633 |      3.09 |       0    |         4 | 2014-11-21   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            0.575 |      2.81 |       0    |         5 | 2014-04-09   |

**[Show more](maincwfamilies)**


## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.0         |             51.3 |     55.5  |      49.83 |      2917 |
| 0.2.9         |             21.2 |     13.12 |      24.44 |      1452 |
| 0.2.5         |              8.7 |     11.32 |       7.33 |       866 |
| 0.3.1         |              5.8 |     10.18 |       5.14 |       210 |
| 0.2.7         |              5.3 |      2.55 |       5.59 |       671 |
| 0.2.8         |              3.4 |      1.6  |       4.39 |       229 |
| 0.2.4         |              2.4 |      2.22 |       2.09 |       531 |
| 0.2.6         |              0.9 |      0.53 |       1.09 |        80 |
| 0.3.2         |              0.6 |      2.93 |       0.06 |        16 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             8.69 |       8.78 |      5.31 |      1282 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93.2 |      90.8 |       93.8 |      6413 |
| BSD     |              6.3 |       8.9 |        5.9 |       336 |
| Windows |              0.2 |       0.1 |        0.1 |       195 |
| Darwin  |              0   |       0   |        0   |        13 |
| SunOS   |              0   |       0   |        0.1 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            17.48 |      16.82 |        15.6 |     22.38 |       580 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|      27.7 |            135 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      7081 |
| None                                       |       703 |
| obfs3, obfs4, scramblesuit                 |       250 |
| obfs3, obfs4                               |        70 |
| obfs3                                      |        22 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| obfs2, obfs3                               |         9 |
| obfs2, obfs3, obfs4                        |         9 |
| obfs3, scramblesuit                        |         9 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| meek                                       |         5 |
| fte, obfs3, obfs4                          |         4 |
| obfs2, obfs3, obfs4, scramblesuit          |         3 |
| obfs4, scramblesuit                        |         2 |
| scramblesuit                               |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| fte, obfs4, websocket                      |         1 |
| obfs3 websocket, websocket                 |         1 |
| snowflake                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

