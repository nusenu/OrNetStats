---
layout: default
---


# OrNetStats

OrNetStats shows you statistics about the Tor network.

Tor network data as of: **2017-10-06 17:00 UTC**

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
| [$ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA](endtoend-correlation-groups#contactgpgfingerprint-contactname-conta)                  | 0.11        | 0.15       | 4         | 3               | 2017-09-24     | 1                           |
| [Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB](endtoend-correlation-groups#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb) | 0.1         | 0.7        | 13        | 2               | 2016-04-01     | 4                           |
| [Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv](endtoend-correlation-groups#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv)     | 0.08        | 0.33       | 4         | 4               | 2017-08-28     | 1                           |
| [AnonyMaid Team &lt;info@anonymaid.net&gt;](endtoend-correlation-groups#anonymaid-team-infoanonymaidnet)                                 | 0.06        | 0.06       | 4         | 4               | 2017-10-01     | 1                           |
| [VSIF Support &lt;support AT vsif dot ca&gt;](endtoend-correlation-groups#vsif-support-support-at-vsif-dot-ca)                           | 0.04        | 0.4        | 5         | 2               | 2017-06-23     | 1                           |
| [Digineo GmbH &lt;tor AT digineo dot de&gt;](endtoend-correlation-groups#digineo-gmbh-tor-at-digineo-dot-de)                             | 0.03        | 0.02       | 2         | 2               | 2017-02-16     | 1                           |
| [visualbasic033@gmail.com](endtoend-correlation-groups#visualbasic033gmailcom)                                                           | 0.03        | 0.94       | 3         | 3               | 2016-08-08     | 1                           |
| **Total**                                                                                                                                | **0.45**    | **2.60**   | **35**    |                 |                |                             |

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
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                            |      7.71 |        21 | 2016-01-25   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9)    |      3.75 |        50 | 2016-08-22   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:DAB96CEA61CC039A803217035293FAB32645FDDA)      |      3.38 |         3 | 2014-04-09   |
| [Privacy Republic &lt;abuse-team at PrivacyRepublic](https://atlas.torproject.org/#search/family:5CECC5C30ACC4B3DE462792323967087CC53D947)       |      2.92 |         4 | 2014-11-21   |
| [0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno](https://atlas.torproject.org/#search/family:C656B41AEFB40A141967EBF49D6E69603C9B4A11)    |      2.45 |         5 | 2014-04-08   |
| [apx &lt;kenan@sly.mn&gt; - 114x2PzqXhfPjQUMVqkcpi8DZN9du](https://atlas.torproject.org/#search/family:51377C496818552E263583A44C796DF3FB0BC71B) |      2.17 |         3 | 2014-11-04   |
| [abuse@blockone.cz](https://atlas.torproject.org/#details/7A5A9DF2FAE2EDDD4EB3BBF2C489BF296F1B2144)                                              |      2.14 |         1 | 2017-07-20   |
| [tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt;](https://atlas.torproject.org/#search/family:7016E939A2DD6EF2FB66A33F1DD45357458B737F)    |      2.02 |         8 | 2014-04-16   |
| [tor@ipredator.se - 1Q3mjKbZwZFEigC8edUZ8ywX4QD7kxF](https://atlas.torproject.org/#details/BC630CBBB518BE7E9F4E09712AB0269E9DC7D626)             |      1.99 |         1 | 2014-04-19   |
| [tor-relays@coldhak.ca](https://atlas.torproject.org/#search/family:C0192FF43E777250084175F4E59AC1BA2290CE38)                                    |      1.96 |         6 | 2016-04-02   |

**[Show more](allexitfamilies)**

### Top 10 Guard Families

| Contact or Fingerprint (truncated)                                                                                                            |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------:|----------:|:-------------|
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |       1.36 |        26 | 2014-12-23   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |       1.29 |         6 | 2014-04-22   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |       1.22 |         3 | 2015-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |       1.18 |        19 | 2015-05-16   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |       1.03 |         7 | 2016-08-10   |
| [CDA994EF](https://atlas.torproject.org/#search/family:CDA994EF01449CDD2E9410709563A3FA3B92ED41)                                              |       1.01 |         8 | 2016-07-26   |
| [Thomas Steen Rasmussen / Tykling &lt;thomas@gibfest.d](https://atlas.torproject.org/#search/family:3A901D1D97500D021E9BDD2A06BE5A846051CD0F) |       0.9  |         7 | 2016-01-03   |
| [info AT omuravpn.com](https://atlas.torproject.org/#search/family:94C0F99BA44AA4A6767C71333B8A66DBD1BC08C7)                                  |       0.7  |         5 | 2017-01-05   |
| [noc@cymru.com](https://atlas.torproject.org/#search/family:896FCE19CB53A73A21DC874977C06B28FC9A8BBA)                                         |       0.62 |         6 | 2011-11-29   |
| [tor terjan net](https://atlas.torproject.org/#search/family:B411027C926A9BFFCF7DA91E3CAF1856A321EFFD)                                        |       0.61 |        10 | 2015-03-05   |

**[Show more](allguardfamilies)**

### Top 10 Relay Families by Consensus Weight

| Contact or Fingerprint (truncated)                                                                                                            |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays | First Seen   |
|:----------------------------------------------------------------------------------------------------------------------------------------------|-----------------:|----------:|-----------:|----------:|:-------------|
| [abuse@to-surf-and-protect.net](https://atlas.torproject.org/#search/family:644DECC5A1879C0FE23DE927DD7049F58BBDF349)                         |            1.958 |      7.71 |       0.57 |        29 | 2016-01-25   |
| [monitor0penmailbox0rg](https://atlas.torproject.org/#search/family:DCD30B90BA3A792DA75DC54A327EF353FB84C38E)                                 |            0.939 |      0    |       1.36 |        28 | 2014-12-23   |
| [https://www.torservers.net/donate.html &lt;support .A](https://atlas.torproject.org/#search/family:F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A) |            0.915 |      1.64 |       0    |         9 | 2014-02-13   |
| [tor at 0x3d dot lu - 1x3dG3utS7FDrTtJutnR3zuCo4Z8f](https://atlas.torproject.org/#search/family:3711E80B5B04494C971FB0459D4209AB7F2EA799)    |            0.873 |      0    |       1.29 |         7 | 2014-04-22   |
| [Felix &lt;zwiebel ta quantentunnel tod de&gt;](https://atlas.torproject.org/#search/family:1AE039EE0B11DB79E4B4B29CBA9F752864A0259E)         |            0.81  |      0    |       1.18 |        22 | 2015-05-16   |
| [Gijs Rijnders tor AT ip-eend DOT nl](https://atlas.torproject.org/#search/family:B204DE75B37064EF6A4C6BAF955C5724578D0B32)                   |            0.783 |      0    |       1.22 |         3 | 2015-04-22   |
| [John L. Ricketts, PhD &lt;john AT quintex dot com&gt;](https://atlas.torproject.org/#search/family:54A4820B46E65509BF3E2B892E66930A41759DE9) |            0.776 |      3.75 |       0    |        50 | 2016-08-22   |
| [https://onionpop.github.io/ gmail is teor2345](https://atlas.torproject.org/#search/family:1A4488A367D89D0EFDA88116059FEBCACF0F508A)         |            0.71  |      0.25 |       1.03 |         8 | 2016-08-10   |
| [sirmatt ksu edu 0x94FBBB0A](https://atlas.torproject.org/#search/family:68CECB9ECDF5EFE8FF23C25B926D756FB346FD92)                            |            0.701 |      1.86 |       0.46 |        10 | 2015-06-01   |
| [0x02225522 Frenn vun der Enn FVDE &lt;info AT enn D](https://atlas.torproject.org/#search/family:DAB96CEA61CC039A803217035293FAB32645FDDA)   |            0.699 |      3.38 |       0    |         3 | 2014-04-09   |

**[Show more](maincwfamilies)**

## Top 10 Countries by CW Fraction

| Country                                                           |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:------------------------------------------------------------------|-----------------:|-----------:|----------:|----------:|
| [France](https://atlas.torproject.org/#search/country:fr)         |            22.06 |      25.63 |     19.54 |       912 |
| [Germany](https://atlas.torproject.org/#search/country:de)        |            19.44 |      21.83 |      6.79 |      1326 |
| [United States](https://atlas.torproject.org/#search/country:us)  |            13.66 |      11.4  |     19.22 |      1203 |
| [Netherlands](https://atlas.torproject.org/#search/country:nl)    |            10.95 |      10.36 |     14.63 |       512 |
| [Canada](https://atlas.torproject.org/#search/country:ca)         |             5.28 |       5.04 |      7.24 |       283 |
| [Sweden](https://atlas.torproject.org/#search/country:se)         |             3.48 |       3.1  |      2.97 |       190 |
| [United Kingdom](https://atlas.torproject.org/#search/country:gb) |             3.3  |       2.77 |      3.8  |       258 |
| [Romania](https://atlas.torproject.org/#search/country:ro)        |             2.3  |       1.46 |      5.81 |        87 |
| [Switzerland](https://atlas.torproject.org/#search/country:ch)    |             2.2  |       2.45 |      1.97 |       143 |
| [Russia](https://atlas.torproject.org/#search/country:ru)         |             2.06 |       1.99 |      1.25 |       329 |

**[Show more](countriesbycw)**

## Top 10 Autonomous System Names by CW Fraction

| AS Name                  |   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|:-------------------------|-----------------:|-----------:|----------:|----------:|
| OVH SAS                  |            16.01 |      18.17 |     13.81 |       589 |
| Online S.a.s.            |            12.49 |      14.71 |     12.58 |       430 |
| Hetzner Online GmbH      |             7.33 |       9    |      0.56 |       316 |
| Digital Ocean, Inc.      |             6.15 |       7.5  |      1.73 |       362 |
| Host Europe GmbH         |             2.12 |       3.03 |      0    |        48 |
| myLoc managed IT AG      |             1.61 |       1.39 |      1    |        38 |
| SURFnet bv               |             1.43 |       1.94 |      0.92 |        11 |
| Linode, LLC              |             1.08 |       0.54 |      0.72 |       221 |
| ITL Company              |             1.04 |       1.42 |      0.28 |        46 |
| Hurricane Electric, Inc. |             0.98 |       0.4  |      3.48 |        13 |

**[Show more](asnameshare)**

## Tor Version Distribution (Relays)

### Major Versions

| Tor Version   |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------------|-----------------:|----------:|-----------:|----------:|
| 0.3.0         |             34.8 |     35.53 |      36.06 |      1823 |
| 0.3.1         |             29.2 |     38.38 |      27.16 |      1476 |
| 0.2.9         |             16.6 |     11.3  |      17.76 |      1372 |
| 0.2.5         |              7.1 |      7.03 |       7.03 |       783 |
| 0.2.7         |              3.6 |      0.39 |       4    |       506 |
| 0.3.2         |              3.3 |      5.39 |       2.16 |       109 |
| 0.2.8         |              2.2 |      0.79 |       2.91 |       161 |
| 0.2.4         |              1.9 |      0.45 |       1.89 |       427 |
| 0.2.6         |              0.8 |      0.7  |       0.99 |        76 |

A version-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/versions.html)

[Complete list of Tor Versions](torversions)

## End-of-Life Relays Share

The following table shows how many relays run a tor version that is no longer supported.

|   CW Fraction(%) |   Guard(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|----------:|----------:|
|             6.55 |       6.88 |      1.55 |      1009 |

**[Show all relays running unsupported tor releases](eolrelays)**

## OS Distribution (Relays)

| OS      |   CW Fraction(%) |   Exit(%) |   Guard(%) |   #Relays |
|:--------|-----------------:|----------:|-----------:|----------:|
| Linux   |             92.9 |      91.2 |       92.9 |      6198 |
| BSD     |              6.6 |       8.6 |        6.7 |       322 |
| Windows |              0.1 |       0   |        0   |       173 |
| SunOS   |              0   |       0   |        0.1 |         4 |
| Darwin  |              0   |       0   |        0.1 |        13 |

A OS-distribution-over-time graph (by relay count) can be found on the [Torproject Metrics page](https://metrics.torproject.org/platforms.html)

## IPv6 Relay Stats

### How many relays are IPv6 ready?

|   CW Fraction(%) |   Guard(%) |   Middle(%) |   Exit(%) |   #Relays |
|-----------------:|-----------:|------------:|----------:|----------:|
|            17.77 |      17.15 |       15.65 |        23 |       567 |

### What portion of exit relays allows IPv6 exiting?

|   Exit(%) |   #Exit Relays |
|----------:|---------------:|
|     26.82 |            128 |

## Bridge Stats

### Bridge Transports Distribution

| Supported Transports                       |   Bridges |
|:-------------------------------------------|----------:|
| obfs4                                      |      1426 |
| None                                       |       690 |
| obfs3, obfs4, scramblesuit                 |       248 |
| obfs3, obfs4                               |        71 |
| obfs3                                      |        23 |
| fte, obfs3, obfs4, scramblesuit, websocket |        20 |
| obfs2, obfs3, obfs4                        |        10 |
| obfs2, obfs3                               |         9 |
| obfs3, scramblesuit                        |         8 |
| fte, obfs3, obfs4, scramblesuit            |         7 |
| meek                                       |         5 |
| fte, obfs3, obfs4                          |         4 |
| obfs2, obfs3, obfs4, scramblesuit          |         3 |
| obfs4, scramblesuit                        |         2 |
| scramblesuit                               |         2 |
| fte, meek, meek, obfs3, scramblesuit       |         1 |
| fte, obfs3                                 |         1 |
| snowflake                                  |         1 |
| websocket                                  |         1 |

## Data Source

OrNetStats uses public data provided by The Tor Project:
* [Onionoo](https://onionoo.torproject.org)
* [CollecTor](https://collector.torproject.org/)

