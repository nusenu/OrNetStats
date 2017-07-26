---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

For each operator the list of running relays is shown (relays are linked to [Atlas](https://atlas.torproject.org)).
Operators and relays are sorted from more relevant to less relevant. More relevant in terms of guard probability.
Guardonly relays have the guard flag but not the exit flag.
Since exits are less common than guards their guard probability is usually 0% even when they have the guard flag.
The number next to the contactinfo shows the number of relays running with the given ContactInfo (excluding middle-only relays).
Middle-only relays (no guard and exit flag) are excluded to reduce the size of this list.

At the end of this page you can find a comma separated list of fingerprints of all guard-only relays on this page.

## If your relay is listed here
Please configure [MyFamily](https://www.torproject.org/docs/tor-manual.html.en#MyFamily) in your torrc configuration files.
This page should help you with debugging your MyFamily configuration. The number in the last column should equal to the number of
relays you operate (for every relay).

Once MyFamily is fixed the relays will automatically disappear from this page (within ~1-2 days).
If you need help with the MyFamily configuration you can reach out to the
[tor-relays mailing list](https://lists.torproject.org/cgi-bin/mailman/listinfo/tor-relays).
You can also use tools that handle MyFamily automatically (I maintain an ansible role - 
[relayor](https://medium.com/@nusenu/deploying-tor-relays-with-ansible-6612593fa34d))
If someone else is using your contactInfo please send an email to bad-relays AT lists DOT torproject DOT org.


## ContactInfo: see https://www.artikel5ev.de/torcontact/ (13) {#see-httpswwwartikel5evdetorcontact}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [dc6jgk8](https://atlas.torproject.org/#details/1B06E7B8B4DAAED1895A73FFDB1B3E24FFBCA0CA)             | 2016-11-06   | Yes         |                    20 |
| [dc6jgk7](https://atlas.torproject.org/#details/F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A)             | 2016-11-04   | Yes         |                    20 |
| [dc6jgk12](https://atlas.torproject.org/#details/A853BA9862837B5FC8E4FF784829DB3BE6F53A75)            | 2016-11-13   | Yes         |                    20 |
| [dc6jgk11](https://atlas.torproject.org/#details/7B700C0C207EBD0002E00F499BE265519AC3C25A)            | 2016-11-11   | Yes         |                    20 |
| [dc6jgk5](https://atlas.torproject.org/#details/846B3EAAF0C07FF72FC79AEBB11FA3ADC58F240F)             | 2016-09-05   | Yes         |                    20 |
| [dc6jgk9](https://atlas.torproject.org/#details/78BC2254D3B31CD865F7682633AA438212132532)             | 2016-11-11   | Yes         |                    20 |
| [dc6jgk10](https://atlas.torproject.org/#details/D86D10F1ADFCB8C58A521E165837D3A90C699418)            | 2016-11-11   | Yes         |                    20 |
| [dc6jgk6](https://atlas.torproject.org/#details/A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13)             | 2016-10-06   | Yes         |                    20 |
| [utzer2](https://atlas.torproject.org/#details/035D2E216B065B961E404BD172336050E5AF4EEA)              | 2017-03-02   | Yes         |                    20 |
| [noiwillnotfixfamily](https://atlas.torproject.org/#details/4DAD2D02EC7F3D278AF20B119652BC3CC4988D6A) | 2017-04-27   | Yes         |                     1 |
| [artikel5ev1](https://atlas.torproject.org/#details/0BC8BA32CC3CB0F598E0C92778F7C0946DFBCE91)         | 2016-10-19   | No          |                    20 |
| [artikel5ev3](https://atlas.torproject.org/#details/7458E9E8AA636DE53F383575E41AA4A6227376D9)         | 2016-11-07   | No          |                    20 |
| [artikel5ev2](https://atlas.torproject.org/#details/DC2191663DD4BAECB34F949CCAC3FDA004CE5BCE)         | 2016-10-29   | No          |                    20 |

## ContactInfo: George Shuklin &lt;george.shuklin@gmail.com&gt; (2) {#george-shuklin-georgeshuklingmailcom}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NSA42](https://atlas.torproject.org/#details/20198F4E1A0E23F32C6265DF749BA003DDAF79B1)       | 2016-02-15   | Yes         |                     1 |
| [freeBogatov](https://atlas.torproject.org/#details/CB6FF27F3A474F6A67D20683C9C97DC275F2658F) | 2016-07-21   | No          |                     1 |

## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv (6) {#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay2](https://atlas.torproject.org/#details/D5B8C38539C509380767D4DE20DE84CF84EE8299)      | 2016-09-05   | Yes         |                     3 |
| [NeelTorRelay1](https://atlas.torproject.org/#details/A20840A16CB658024B0D3A0E3F19A9C0E34C843F)      | 2017-01-17   | Yes         |                     4 |
| [NeelTorExitUSWest](https://atlas.torproject.org/#details/0D8211D34F29F51D690303E319766E1B7C28BADB)  | 2017-05-25   | No          |                     3 |
| [NeelTorExitCZ](https://atlas.torproject.org/#details/1602E42D1DE3C7B3EF042F357F906DE55FA6C7C6)      | 2016-08-10   | No          |                     4 |
| [NeelTorExitUA](https://atlas.torproject.org/#details/976652C0FF243539B1A966F2C27F00C3724545C0)      | 2017-07-23   | No          |                     1 |
| [NeelTorExitUSMwest](https://atlas.torproject.org/#details/FF3A6898F1348224E6ABA8B8E98F15770E5DD362) | 2017-07-14   | No          |                     1 |

## ContactInfo: Abuse Department &lt;abuse AT hartvoorinternetvrijhei (2) {#abuse-department-abuse-at-hartvoorinternetvrijhei}

| Nickname                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [hviv103](https://atlas.torproject.org/#details/D12D357D91DD3B79E2AD9FDB160F9A4558147E05) | 2015-09-06   | Yes         |                     1 |
| [hviv104](https://atlas.torproject.org/#details/81B75D534F91BFB7C57AB67DA10BCEF622582AE8) | 2014-04-09   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://atlas.torproject.org/#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://atlas.torproject.org/#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://atlas.torproject.org/#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt; (5) {#tornoisebridgenet-admintornoisebridgenet}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [noisebridge01a](https://atlas.torproject.org/#details/1A835E3663068222F28F7C5AF3216F4B27B50B57) | 2015-05-20   | Yes         |                     1 |
| [noiseexit03d](https://atlas.torproject.org/#details/02A627FA195809A3ABE031B7864CCA7A310F1D44)   | 2017-05-21   | No          |                     4 |
| [noiseexit03c](https://atlas.torproject.org/#details/7016E939A2DD6EF2FB66A33F1DD45357458B737F)   | 2017-05-21   | No          |                     4 |
| [noiseexit03a](https://atlas.torproject.org/#details/8175A86D8896CEA37FDC67311F9BDC1DDCBE8136)   | 2017-05-20   | No          |                     4 |
| [noiseexit03b](https://atlas.torproject.org/#details/D4010FAD096CFB59278015F711776D8CCB2735EC)   | 2017-05-21   | No          |                     4 |

## ContactInfo: visualbasic033@gmail.com (3) {#visualbasic033gmailcom}

| Nickname                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [doutreval](https://atlas.torproject.org/#details/CB4EBE9C475A60A5F2CDA92C83CE093BD945D940) | 2015-12-04   | Yes         |                     1 |
| [dlavolos](https://atlas.torproject.org/#details/6E41F9BC3FE626D1897865CE9A9335D09A8DA5FE)  | 2016-03-07   | No          |                     1 |
| [sowinetz](https://atlas.torproject.org/#details/A041B285B228241C3185483EEF42F0BC96D40BFB)  | 2016-08-08   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

D12D357D91DD3B79E2AD9FDB160F9A4558147E05,1A835E3663068222F28F7C5AF3216F4B27B50B57,1B06E7B8B4DAAED1895A73FFDB1B3E24FFBCA0CA,D86D10F1ADFCB8C58A521E165837D3A90C699418,B4CA5FDB58A06914689BA23ED2C5FED79CFB3950,F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A,20198F4E1A0E23F32C6265DF749BA003DDAF79B1,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13,035D2E216B065B961E404BD172336050E5AF4EEA,A853BA9862837B5FC8E4FF784829DB3BE6F53A75,D5B8C38539C509380767D4DE20DE84CF84EE8299,A20840A16CB658024B0D3A0E3F19A9C0E34C843F,846B3EAAF0C07FF72FC79AEBB11FA3ADC58F240F,78BC2254D3B31CD865F7682633AA438212132532,7B700C0C207EBD0002E00F499BE265519AC3C25A,CB4EBE9C475A60A5F2CDA92C83CE093BD945D940,4DAD2D02EC7F3D278AF20B119652BC3CC4988D6A