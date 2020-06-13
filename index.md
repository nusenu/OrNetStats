---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2020-06-13 08:00 UTC**

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
| [abuse-contact@to-surf-and-protect.net](endtoend-correlation-groups#abuse-contactto-surf-and-protectnet) | 1.12        | 20.28      | 138       | 4               | 2020-03-27     | 1                           |
| [tomas.vanagas@knf.vu.lt tor-relay.co](endtoend-correlation-groups#tomasvanagasknfvult-tor-relayco)      | 0.03        | 0.06       | 2         | 2               | 2020-04-28     | 1                           |
| **Total**                                                                                                | **1.15**    | **20.34**  | **140**   |                 |                |                             |

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
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                    |     20.59 |       131 | 2016-01-25   |
| [abusetor1234@protonmail.com](https://metrics.torproject.org/rs.html#search/family:167C0B275C82A4DD39316454C5FAEFB3E449EB3B)                              |      7.4  |        32 | 2020-05-22   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                        |      5.45 |        32 | 2018-03-21   |
| [stayhomeusetor@protonmail.ch](https://metrics.torproject.org/rs.html#search/family:0187FF31A3872C81C0297C5C704E9812BCE3AB68)                             |      5.05 |        35 | 2020-05-28   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)        |      3.76 |        18 | 2018-03-01   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887)    |      3.5  |        90 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE)    |      3.48 |        17 | 2016-12-23   |
| [fbirelays@protonmail.com](https://metrics.torproject.org/rs.html#search/family:060595712ABB1E34DBD2061E6C13AC0062BE30DE)                                 |      3.02 |        12 | 2020-05-04   |
| [MichaelLyons12345@hotmail.com](https://metrics.torproject.org/rs.html#search/family:012AA2D05CBE808AC8D235409BEEFB81B3828FA6)                            |      2.45 |        34 | 2020-05-25   |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w](https://metrics.torproject.org/rs.html#search/family:0011BD2485AD45D984EC4159C88FC066E5E3300E) |      1.9  |        19 | 2013-06-11   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                                        |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                      |       1.37 |        14 | 2018-10-05   |
| [Bauruine &lt;torcontact aatt tuxli.ch&gt; - 1CVkdZfRGWXE](https://metrics.torproject.org/rs.html#search/family:021047C51A57254D263DDB8B9277CA1C286D600E) |       0.92 |        11 | 2014-04-09   |
| [0ED0EA32](https://metrics.torproject.org/rs.html#search/family:0ED0EA324C931CF41CB5272BFB1D015B3D5772A9)                                                 |       0.82 |         5 | 2017-10-24   |
| [BMTY90VKYRQPUJZOTH @ Safe-mail.net](https://metrics.torproject.org/rs.html#search/family:14E72D4DA10B66353E583F26EE04AC0D563EA7EF)                       |       0.72 |        28 | 2019-02-23   |
| [63540827](https://metrics.torproject.org/rs.html#search/family:63540827C4832D214984EA47B7A68C593F9F862F)                                                 |       0.72 |         2 | 2018-12-12   |
| [torrpi1405@gmail.com](https://metrics.torproject.org/rs.html#search/family:1323D34C2FA4AE0EC4EEA9853F3464693EF428E7)                                     |       0.71 |        23 | 2018-08-28   |
| [24F97F98](https://metrics.torproject.org/rs.html#search/family:24F97F98C45E4754655BE66799049763DAEE99CE)                                                 |       0.65 |         4 | 2018-08-17   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://metrics.torproject.org/rs.html#search/family:6DFEB41C04CCE846871338E85DD5ACF5CFB6C1DD)                      |       0.63 |         3 | 2015-04-22   |
| [Peter Gerber &lt;tor@arbitrary.ch&gt;](https://metrics.torproject.org/rs.html#search/family:3F43D0584A2613C9DB631382FF486DC6B95EA1C8)                    |       0.6  |         8 | 2019-01-20   |
| [Kevin Hicks &lt;admin@fissionrelays.net&gt;](https://metrics.torproject.org/rs.html#search/family:0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)              |       0.55 |        11 | 2018-01-07   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                                     |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse-contact@to-surf-and-protect.net](https://metrics.torproject.org/rs.html#search/family:01FDC8E92D3280847D856DA1F9BFC2B4CD2C2EE8)                 |            6.861 |     20.59 |       0.47 |       135 | 2016-01-25   |
| [abusetor1234@protonmail.com](https://metrics.torproject.org/rs.html#search/family:167C0B275C82A4DD39316454C5FAEFB3E449EB3B)                           |            2.367 |      7.4  |       0    |        32 | 2020-05-22   |
| [F3 Netze &lt;abuse@f3netze.de&gt;](https://metrics.torproject.org/rs.html#search/family:06EC2C1669E5A811D9640E07CED5786DA50C5737)                     |            1.744 |      5.45 |       0    |        32 | 2018-03-21   |
| [stayhomeusetor@protonmail.ch](https://metrics.torproject.org/rs.html#search/family:0187FF31A3872C81C0297C5C704E9812BCE3AB68)                          |            1.616 |      5.05 |       0    |        35 | 2020-05-28   |
| [Foundation for Applied Privacy email:tor appliedp](https://metrics.torproject.org/rs.html#search/family:06804E6383EE94E83C9453F39B1E524C272D6D84)     |            1.258 |      3.76 |       0.09 |        21 | 2017-06-13   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://metrics.torproject.org/rs.html#search/family:0077BCBA7244DB3E6A5ED2746E86170066684887) |            1.121 |      3.5  |       0    |        90 | 2016-08-22   |
| [https://www.torservers.net/donate.html &lt;support .A](https://metrics.torproject.org/rs.html#search/family:0E5522CB4F79E36C0BB263BABC861CFC686929AE) |            1.115 |      3.48 |       0    |        17 | 2016-12-23   |
| [fbirelays@protonmail.com](https://metrics.torproject.org/rs.html#search/family:060595712ABB1E34DBD2061E6C13AC0062BE30DE)                              |            0.967 |      3.02 |       0    |        12 | 2020-05-04   |
| [&lt;tor AT afo MINUS tm DOT org&gt;](https://metrics.torproject.org/rs.html#search/family:0512FE6BE9CCA0ED133152E64010B2FBA141EB10)                   |            0.806 |      0    |       1.37 |        14 | 2018-10-05   |
| [MichaelLyons12345@hotmail.com](https://metrics.torproject.org/rs.html#search/family:012AA2D05CBE808AC8D235409BEEFB81B3828FA6)                         |            0.785 |      2.45 |       0    |        34 | 2020-05-25   |

**[Show more](maincwfamilies)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                        |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                        |            17.52 |      16.06 |     23.22 |       600 |
| Hetzner Online GmbH            |            15.82 |      23.7  |      0.42 |       389 |
| Online S.a.s.                  |             7.6  |      10.8  |      2.58 |       249 |
| Joshua Peter McQuistan         |             6.83 |       0.33 |     20.59 |       135 |
| netcup GmbH                    |             2.43 |       2.8  |      0.57 |       126 |
| F3 Netze e.V.                  |             1.74 |       0    |      5.45 |        32 |
| myLoc managed IT AG            |             1.57 |       2.06 |      0.94 |        44 |
| FranTech Solutions             |             1.45 |       0.59 |      3.2  |       123 |
| Contabo GmbH                   |             1.23 |       1.87 |      0.28 |        84 |
| Foundation for Applied Privacy |             1.2  |       0    |      3.76 |        18 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.4.3         |             42.7 |     41.53 |      44.06 |      2437 |
| 0.4.2         |             37   |     53.28 |      28.36 |      2278 |
| 0.3.5         |             13.3 |      3.62 |      17.44 |      1120 |
| 0.4.1         |              5.8 |      1.41 |       8.53 |       338 |
| 0.4.4         |              0.9 |      0.15 |       1.52 |        35 |
| 0.4.5         |              0   |      0    |       0.06 |         8 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             5.89 |        8.6 |      1.41 |       346 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             93   |      92.8 |       92.8 |      5670 |
| BSD     |              6.7 |       7   |        6.9 |       462 |
| Windows |              0.1 |       0   |        0.1 |        40 |
| Darwin  |              0   |       0   |        0   |         8 |
| SunOS   |              0   |       0   |        0   |         3 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|             35.9 |      31.05 |       29.85 |     47.49 |      1485 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     48.55 |            532 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |       744 |
| None                                       |       468 |
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
| meek, meek, obfs4                          |         1 |
| meek, obfs3, obfs4                         |         1 |
| obfs2, obfs3, obfs4, scramblesuit          |         1 |
| obfs3, scramblesuit                        |         1 |
| obfs4, scramblesuit                        |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://metrics.torproject.org/onionoo.html)
* [CollecTor](https://metrics.torproject.org/collector.html)

