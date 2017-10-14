---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-10-14 09:00 UTC**

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
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb) | 0.09        | 0.77       | 13        | 2               | 2016-04-01     | 4                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)     | 0.06        | 0.35       | 3         | 3               | 2017-08-23     | 1                           |
| [torrelays A-T cyb3rwr3ck D-O-T net](endtoend-correlation-groups#torrelays-a-t-cyb3rwr3ck-d-o-t-net)                                     | 0.06        | 0.01       | 2         | 2               | 2017-06-15     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                                 | 0.05        | 0.03       | 4         | 4               | 2017-10-01     | 1                           |
| [emerson tor@emersonveenstra.net bitcoin:126gyYcBji](endtoend-correlation-groups#emerson-toremersonveenstranet-bitcoin126gyycbji)        | 0.04        | 0.44       | 4         | 4               | 2017-10-04     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           | 0.04        | 0.12       | 2         | 2               | 2016-03-07     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                           | 0.04        | 0.69       | 5         | 2               | 2017-06-23     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.03        | 0.28       | 2         | 2               | 2017-02-16     | 1                           |
| **Total**                                                                                                                                | **0.41**    | **2.69**   | **35**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      6.29 |        21 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)      |      5.29 |         6 | 2014-04-09   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9)    |      3.95 |        50 | 2016-08-22   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.58 |         3 | 2014-11-04   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      2.49 |         4 | 2014-11-21   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:C656B41AEFB40A141967EBF49D6E69603C9B4A11)    |      2.3  |         5 | 2014-04-08   |
| [abuse@blockone.cz](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)                                              |      2.29 |         1 | 2017-07-20   |
| [Exit by Reporters without Borders via https://www.](https://atlas.torproject.org/#search/family:A2DB293FFC5A76A718863BF1AEDBC8DFB1CB1097)       |      2.09 |         6 | 2016-12-23   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://atlas.torproject.org/#search/family:7016E939A2DD6EF2FB66A33F1DD45357458B737F)    |      2.07 |         8 | 2014-04-16   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      2.03 |         1 | 2014-04-19   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |       1.37 |         8 | 2016-07-26   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |       1.31 |        26 | 2014-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.05 |         6 | 2014-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       1    |         7 | 2016-08-10   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       1    |        19 | 2015-05-16   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       0.91 |         7 | 2016-01-03   |
| [info AT omuravpn.com](https://atlas.torproject.org/#search/family:94C0F99BA44AA4A6767C71333B8A66DBD1BC08C7)                                  |       0.81 |         9 | 2017-01-05   |
| [GTor &lt;contact AT gtor DOT org&gt;](https://atlas.torproject.org/#search/family:8C7106C880FE8AA1319DD71B59623FCB8914C9F1)                  |       0.72 |        10 | 2014-04-10   |
| [11882BD0](https://atlas.torproject.org/#search/family:11882BD0A5A587FEE13465244EA8BCD4C7E03510)                                              |       0.66 |         6 | 2016-07-26   |
| [noc@cymru.com](https://atlas.torproject.org/#search/family:896FCE19CB53A73A21DC874977C06B28FC9A8BBA)                                         |       0.56 |         5 | 2011-11-29   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.521 |      6.29 |       0.41 |        29 | 2016-01-25   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:C793AB88565DDD3C9E4C6F15CCB9D8C7EF964CE9)   |            1.05  |      5.29 |       0    |         6 | 2014-04-09   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.951 |      0    |       1.31 |        28 | 2014-12-23   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |            0.9   |      0    |       1.37 |         8 | 2016-07-26   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9) |            0.785 |      3.95 |       0    |        50 | 2016-08-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.757 |      0    |       0.31 |         3 | 2015-04-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.731 |      0.37 |       1    |         8 | 2016-08-10   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.729 |      0    |       1.05 |         7 | 2014-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.698 |      0    |       1    |        22 | 2015-05-16   |
| [sirmatt ksu edu 0x94FBBB0A](https://atlas.torproject.org/#search/family:68CECB9ECDF5EFE8FF23C25B926D756FB346FD92)                            |            0.663 |      2.02 |       0.37 |        10 | 2015-06-01   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            23.06 |      26.56 |     18.61 |       901 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            19.51 |      22.34 |      5.85 |      1321 |
| [United States](https://atlas.torproject.org/#search/country:us)  |            13.65 |      11.63 |     19.27 |      1169 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            10.59 |       9.49 |     13.66 |       495 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             5.22 |       4.97 |      6.81 |       272 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             3.13 |       2.94 |      3.46 |       254 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.12 |       2.84 |      4.44 |       189 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.43 |       2.62 |      2.17 |       142 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.27 |       1.42 |      6.33 |        86 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             1.87 |       1.65 |      1.03 |       304 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                  |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                  |            15.99 |      18.42 |     11.38 |       583 |
| Online S.a.s.            |            13.38 |      15.73 |     12.11 |       425 |
| Hetzner Online GmbH      |             7.43 |       9.32 |      0.67 |       312 |
| Digital Ocean, Inc.      |             6.02 |       7.2  |      1.63 |       386 |
| Host Europe GmbH         |             2.25 |       3.22 |      0    |        46 |
| myLoc managed IT AG      |             1.51 |       1.66 |      0.17 |        53 |
| SURFnet bv               |             1.47 |       1.05 |      1.17 |        11 |
| Linode, LLC              |             0.99 |       0.48 |      0.5  |       210 |
| ITL Company              |             0.96 |       1.18 |      0.08 |        48 |
| Hurricane Electric, Inc. |             0.95 |       0.38 |      3.48 |        13 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.0         |             31.6 |     29.09 |      34.29 |      1512 |
| 0.3.1         |             31   |     40.06 |      28.5  |      1698 |
| 0.2.9         |             16.6 |     11.01 |      17.26 |      1362 |
| 0.2.5         |              7.4 |      7.16 |       6.97 |       808 |
| 0.3.2         |              4.7 |     10.3  |       3.63 |       149 |
| 0.2.7         |              3.7 |      0.3  |       4.06 |       481 |
| 0.2.8         |              2   |      0.84 |       2.44 |       147 |
| 0.2.4         |              1.9 |      0.65 |       2.01 |       387 |
| 0.2.6         |              0.6 |      0.54 |       0.78 |        67 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             6.44 |       6.86 |       1.5 |       935 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.8 |      90.7 |       93   |      6136 |
| BSD     |              6.6 |       9.2 |        6.5 |       305 |
| Windows |              0.2 |       0   |        0   |       143 |
| Darwin  |              0.1 |       0   |        0.1 |        12 |
| SunOS   |              0.1 |       0   |        0.1 |         4 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### What cw fraction / guard/middle/exit probability has an IPv6 ORPort?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            17.94 |      16.85 |       15.15 |     25.78 |       567 |

### What exit probability allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     29.21 |            129 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1314 |
| None                                       |       707 |
| obfs3, obfs4, scramblesuit                 |       247 |
| obfs3, obfs4                               |        62 |
| fte, obfs3, obfs4, scramblesuit, websocket |        22 |
| obfs3                                      |        22 |
| obfs2, obfs3, obfs4                        |        10 |
| obfs2, obfs3                               |         9 |
| obfs3, scramblesuit                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         6 |
| meek                                       |         5 |
| fte, obfs3, obfs4                          |         4 |
| obfs2, obfs3, obfs4, scramblesuit          |         3 |
| obfs4, scramblesuit                        |         2 |
| scramblesuit                               |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

