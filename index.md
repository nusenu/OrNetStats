---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-06-08 18:00 UTC**

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

| Contact                                                                                                  | Guard (%)   | Exit (%)   | #Relays   | /16 Netblocks   | Newest Relay   | Eff. Family Members (min)   |
|:---------------------------------------------------------------------------------------------------------|:------------|:-----------|:----------|:----------------|:---------------|:----------------------------|
| [abuse-contact@to-surf-and-protect.net](endtoend-correlation-groups#abuse-contactto-surf-and-protectnet) | 1.07        | 20.56      | 138       | 4               | 2020-03-27     | 1                           |
| [tomas.vanagas@knf.vu.lt tor-relay.co](endtoend-correlation-groups#tomasvanagasknfvult-tor-relayco)      | 0.03        | 0.07       | 2         | 2               | 2020-04-28     | 1                           |
| **Total**                                                                                                | **1.10**    | **20.63**  | **140**   |                 |                |                             |

For a detailed list of (known) relays in end-to-end correlation position see **[this page](endtoend-correlation-groups)**.

**NOTE:** There are many more relays with
[MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) configuration issues but most operate exit or guard relays
exclusively or within a single /16 network block. Such operators can not become the first **and** last hop of your tor circuits,
but they might be able to reveal your guard relay (when they act as the middle and exit relay in a single circuit).


## Biggest Relay Families on the Tor Network

Relays are aggregated based on effective families. Effective families are relays with a mutually configured [MyFamily setting](https://www.torproject.org/docs/tor-manual.html.en). Single relays (without family) are also considered but not aggregated. The first column usually shows the contact information, or if no contact information was provided, the first 8 characters of the relay fingerprint.

### Top 10 Exit Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Exit(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     20.91 |       131 | 2016-01-25   |
| [abusetor1234@protonmail.com](https://metrics.torproject.org/rs.html#search/family:167C0B275C82A4DD39316454C5FAEFB3E449EB3B)                              |      6.33 |        32 | 2020-05-22   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |      5.32 |        32 | 2018-03-21   |
| [stayhomeusetor@protonmail.ch](https://metrics.torproject.org/rs.html#search/family:0187FF31A3872C81C0297C5C704E9812BCE3AB68)                             |      3.92 |        35 | 2020-05-28   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      3.92 |        18 | 2018-03-01   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.84 |        17 | 2016-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      3.76 |       100 | 2016-08-22   |
| [fbirelays@protonmail.com](https://metrics.torproject.org/rs.html#search/family:060595712ABB1E34DBD2061E6C13AC0062BE30DE)                                 |      2.89 |        12 | 2020-05-04   |
| [MichaelLyons12345@hotmail.com](https://metrics.torproject.org/rs.html#search/family:012AA2D05CBE808AC8D235409BEEFB81B3828FA6)                            |      2.11 |        34 | 2020-05-25   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      1.98 |        19 | 2013-06-11   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |       1.42 |        14 | 2018-10-05   |
| [abuse@for-privacy.net](https://metrics.torproject.org/rs.html#search/family:18671DE5092C67883BFB2450C3267B92618BEC66)                                    |       0.82 |        10 | 2019-03-16   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)              |       0.78 |        15 | 2018-01-07   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:04D9CEA8D778ABA130B014F758C2BCADD31DA05E)                       |       0.75 |        30 | 2019-02-23   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                                 |       0.73 |         5 | 2017-10-24   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://metrics.torproject.org/rs.html#search/family:13557448AD1632BF080757C2FF7769BB23DF1DF3) |       0.7  |         8 | 2014-04-09   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                                 |       0.69 |         4 | 2018-08-17   |
| [63540827](https://metrics.torproject.org/rs.html#search/family:63540827C4832D214984EA47B7A68C593F9F862F)                                                 |       0.68 |         2 | 2018-12-12   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:1323D34C2FA4AE0EC4EEA9853F3464693EF428E7)                                     |       0.67 |        22 | 2018-08-28   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                      |       0.63 |         3 | 2015-04-22   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                 |            6.916 |     20.91 |       0.5  |       135 | 2016-01-25   |
| [abusetor1234@protonmail.com](https://metrics.torproject.org/rs.html#search/family:167C0B275C82A4DD39316454C5FAEFB3E449EB3B)                           |            2.004 |      6.33 |       0    |        32 | 2020-05-22   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                     |            1.684 |      5.32 |       0    |        32 | 2018-03-21   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.299 |      3.92 |       0.09 |        21 | 2017-06-13   |
| [stayhomeusetor@protonmail.ch](https://metrics.torproject.org/rs.html#search/family:0187FF31A3872C81C0297C5C704E9812BCE3AB68)                          |            1.242 |      3.92 |       0    |        35 | 2020-05-28   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |            1.216 |      3.84 |       0    |        17 | 2016-12-23   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |            1.191 |      3.76 |       0    |       100 | 2016-08-22   |
| [fbirelays@protonmail.com](https://metrics.torproject.org/rs.html#search/family:060595712ABB1E34DBD2061E6C13AC0062BE30DE)                              |            0.917 |      2.89 |       0    |        12 | 2020-05-04   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.826 |      0    |       1.42 |        14 | 2018-10-05   |
| [MichaelLyons12345@hotmail.com](https://metrics.torproject.org/rs.html#search/family:012AA2D05CBE808AC8D235409BEEFB81B3828FA6)                         |            0.67  |      2.11 |       0    |        34 | 2020-05-25   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                        |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                        |            16.16 |      15.84 |     20.37 |       595 |
| Hetzner Online GmbH            |            15.75 |      23.53 |      0.43 |       397 |
| Online S.a.s.                  |             7.38 |      10.71 |      2.58 |       250 |
| Joshua Peter McQuistan         |             6.95 |       0.38 |     20.91 |       136 |
| netcup GmbH                    |             2.33 |       2.64 |      0.59 |       123 |
| myLoc managed IT AG            |             1.68 |       2.34 |      0.92 |        42 |
| F3 Netze e.V.                  |             1.68 |       0    |      5.32 |        32 |
| FranTech Solutions             |             1.31 |       0.68 |      2.78 |       123 |
| Foundation for Applied Privacy |             1.24 |       0    |      3.92 |        18 |
| Contabo GmbH                   |             1.19 |       1.9  |      0.25 |        84 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.3         |             40.9 |     41.24 |      42.68 |      2326 |
| 0.4.2         |             39   |     53.33 |      29.42 |      2434 |
| 0.3.5         |             13.1 |      3.82 |      17.7  |      1147 |
| 0.4.1         |              5.8 |      1.43 |       8.52 |       351 |
| 0.4.4         |              1   |      0.16 |       1.65 |        43 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.81 |       8.52 |      1.43 |       351 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93   |      92.5 |       92.9 |      5761 |
| BSD     |              6.7 |       7.3 |        6.8 |       454 |
| Windows |              0.1 |       0   |        0.1 |        47 |
| SunOS   |              0   |       0   |        0   |         3 |
| Darwin  |              0   |       0   |        0   |         7 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            35.75 |      31.07 |       28.72 |     48.39 |      1482 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     49.38 |            537 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       746 |
| None                                       |       461 |
| obfs3, obfs4                               |        78 |
| fte, obfs3, obfs4, scramblesuit, websocket |        21 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| meek                                       |         5 |
| obfs3, obfs4, scramblesuit                 |         4 |
| obfs2, obfs3, obfs4                        |         3 |
| obfs3                                      |         2 |
| fte, obfs2, obfs3, obfs4, scramblesuit     |         1 |
| fte, obfs3, obfs4                          |         1 |
| fte, obfs3, scramblesuit                   |         1 |
| fte, obfs4                                 |         1 |
| meek, meek                                 |         1 |
| meek, obfs3, obfs4                         |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs3, scramblesuit                        |         1 |
| obfs4, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

