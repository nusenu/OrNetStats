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


## ContactInfo: https://www.torservers.net/donate.html &lt;support .A (13) {#httpswwwtorserversnetdonatehtml-support-a}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [iVPN](https://atlas.torproject.org/#details/A2534EF23390CAE079B1586F0FDF9CE11F556062)           | 2016-12-30   | Yes         |                     1 |
| [criticalmass](https://atlas.torproject.org/#details/1D3174338A1131A53E098443E76E1103CDED00DC)   | 2016-12-30   | Yes         |                     1 |
| [HSLtor](https://atlas.torproject.org/#details/E43A346CB81DDF364B6FF68235AFADBA0E8692B8)         | 2017-01-22   | Yes         |                     1 |
| [dorrisdeebrown](https://atlas.torproject.org/#details/FDAED15C98CFE7A416E5676F614254F78406105C) | 2016-12-23   | Yes         |                     1 |
| [edwardsnowden1](https://atlas.torproject.org/#details/0818DAE0E2DDF795AEDEAC60B15E71901084F281) | 2016-11-15   | No          |                     1 |
| [hessel0](https://atlas.torproject.org/#details/14F92FF956105932E9DEC5B82A7778A0B1BD9A52)        | 2016-09-02   | No          |                     1 |
| [andregorz0](https://atlas.torproject.org/#details/23038A7F2845EBA2234ECD6651BD4A7762F51B18)     | 2016-11-15   | No          |                     1 |
| [hessel1](https://atlas.torproject.org/#details/4888770464F0E900EFEF1BA181EA873D13F7713C)        | 2016-09-02   | No          |                     1 |
| [amazonas](https://atlas.torproject.org/#details/4E021F36F95EDD4F93F824020E3C5BFEA7B595CC)       | 2014-02-13   | No          |                     3 |
| [hessel2](https://atlas.torproject.org/#details/5EB8D862E70981B8690DEDEF546789E26AB2BD24)        | 2016-09-02   | No          |                     1 |
| [politkovskaja](https://atlas.torproject.org/#details/64D500C4D7F989ECD74B42ABB068818EF95525F3)  | 2014-02-13   | No          |                     3 |
| [edwardsnowden2](https://atlas.torproject.org/#details/ABF7FBF389C9A747938B639B20E80620B460B2A9) | 2016-11-15   | No          |                     1 |
| [freeBogatov](https://atlas.torproject.org/#details/F657ACB301CBAB4283F9CEC6D82ABE2FA62A398A)    | 2014-02-13   | No          |                     3 |

## ContactInfo: see https://www.artikel5ev.de/torcontact/ (15) {#see-httpswwwartikel5evdetorcontact}

| Nickname                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [dc6jgk11](https://atlas.torproject.org/#details/7B700C0C207EBD0002E00F499BE265519AC3C25A)     | 2016-11-11   | Yes         |                    21 |
| [dc6jgk12](https://atlas.torproject.org/#details/A853BA9862837B5FC8E4FF784829DB3BE6F53A75)     | 2016-11-13   | Yes         |                    21 |
| [dc6jgk6](https://atlas.torproject.org/#details/A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13)      | 2016-10-06   | Yes         |                    21 |
| [dc6jgk8](https://atlas.torproject.org/#details/1B06E7B8B4DAAED1895A73FFDB1B3E24FFBCA0CA)      | 2016-11-06   | Yes         |                    21 |
| [dc6jgk15TEST](https://atlas.torproject.org/#details/4DAD2D02EC7F3D278AF20B119652BC3CC4988D6A) | 2017-04-27   | Yes         |                     1 |
| [utzer1](https://atlas.torproject.org/#details/B4CA5FDB58A06914689BA23ED2C5FED79CFB3950)       | 2017-03-01   | Yes         |                    21 |
| [dc6jgk7](https://atlas.torproject.org/#details/F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A)      | 2016-11-04   | Yes         |                    21 |
| [Artikel5ev6](https://atlas.torproject.org/#details/4DD902046E7155BBE79C34EE6D53BF7408B98CE4)  | 2017-03-05   | Yes         |                    21 |
| [dc6jgk9](https://atlas.torproject.org/#details/78BC2254D3B31CD865F7682633AA438212132532)      | 2016-11-11   | Yes         |                    21 |
| [utzer2](https://atlas.torproject.org/#details/035D2E216B065B961E404BD172336050E5AF4EEA)       | 2017-03-02   | Yes         |                    21 |
| [dc6jgk5](https://atlas.torproject.org/#details/846B3EAAF0C07FF72FC79AEBB11FA3ADC58F240F)      | 2016-09-05   | Yes         |                    21 |
| [dc6jgk10](https://atlas.torproject.org/#details/D86D10F1ADFCB8C58A521E165837D3A90C699418)     | 2016-11-11   | Yes         |                    21 |
| [artikel5ev1](https://atlas.torproject.org/#details/0BC8BA32CC3CB0F598E0C92778F7C0946DFBCE91)  | 2016-10-19   | No          |                    21 |
| [artikel5ev3](https://atlas.torproject.org/#details/7458E9E8AA636DE53F383575E41AA4A6227376D9)  | 2016-11-07   | No          |                    21 |
| [artikel5ev2](https://atlas.torproject.org/#details/DC2191663DD4BAECB34F949CCAC3FDA004CE5BCE)  | 2016-10-29   | No          |                    21 |

## ContactInfo: snaptorg at gmail , com &gt;&gt; bitcoin:1DmvqGnoexBSzSF (5) {#snaptorgatgmailcom--bitcoin1dmvqgnoexbszsf}

| Nickname                                                                                        | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [SnapTorZie](https://atlas.torproject.org/#details/A019AF72731C2731CA90C01B2C5F279289B5E177)    | 2017-05-03   | Yes         |                     1 |
| [SnapTorCAN](https://atlas.torproject.org/#details/B39AD54B73A70DA68F6FC26CD0A874DE762B7825)    | 2016-11-12   | Yes         |                     4 |
| [SnapTorSTRAS](https://atlas.torproject.org/#details/04738935F40F06E03312097C7411EEC67EB99E93)  | 2016-11-26   | Yes         |                     4 |
| [SnapTorUSA](https://atlas.torproject.org/#details/48B93C88B90608913C1D7FD9378DBB970BF994EC)    | 2017-03-12   | Yes         |                     4 |
| [SnapTorExitUS](https://atlas.torproject.org/#details/B164C656D44C1936E6D5E79183E3C7F341C663CD) | 2017-03-12   | No          |                     4 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://atlas.torproject.org/#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://atlas.torproject.org/#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://atlas.torproject.org/#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://atlas.torproject.org/#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://atlas.torproject.org/#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: visualbasic033@gmail.com (3) {#visualbasic033gmailcom}

| Nickname                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [doutreval](https://atlas.torproject.org/#details/CB4EBE9C475A60A5F2CDA92C83CE093BD945D940) | 2015-12-04   | Yes         |                     1 |
| [dlavolos](https://atlas.torproject.org/#details/6E41F9BC3FE626D1897865CE9A9335D09A8DA5FE)  | 2016-03-07   | No          |                     1 |
| [sowinetz](https://atlas.torproject.org/#details/A041B285B228241C3185483EEF42F0BC96D40BFB)  | 2016-08-08   | No          |                     1 |

## ContactInfo: tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt; (9) {#tornoisebridgenet-admintornoisebridgenet}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [noisebridge01a](https://atlas.torproject.org/#details/1A835E3663068222F28F7C5AF3216F4B27B50B57) | 2015-05-20   | Yes         |                     1 |
| [noiseexit03d](https://atlas.torproject.org/#details/02A627FA195809A3ABE031B7864CCA7A310F1D44)   | 2017-05-21   | No          |                     4 |
| [noiseexit01b](https://atlas.torproject.org/#details/3591E0E966309AD335BE62FF694E8A898F97A6C9)   | 2014-04-16   | No          |                     4 |
| [noiseexit03c](https://atlas.torproject.org/#details/7016E939A2DD6EF2FB66A33F1DD45357458B737F)   | 2017-05-21   | No          |                     4 |
| [noiseexit03a](https://atlas.torproject.org/#details/8175A86D8896CEA37FDC67311F9BDC1DDCBE8136)   | 2017-05-20   | No          |                     4 |
| [noiseexit01d](https://atlas.torproject.org/#details/C6F6B70AD9115C65B618B0AF3FD10B0432626CA9)   | 2014-04-16   | No          |                     4 |
| [noiseexit03b](https://atlas.torproject.org/#details/D4010FAD096CFB59278015F711776D8CCB2735EC)   | 2017-05-21   | No          |                     4 |
| [noiseexit01c](https://atlas.torproject.org/#details/D42EE35F9B62769E782DEA2FC6358ABFAFE7DB66)   | 2014-04-16   | No          |                     4 |
| [noiseexit01a](https://atlas.torproject.org/#details/E93F05C9A7112544A2F132CBB7F6701877140F2A)   | 2014-04-16   | No          |                     4 |

## ContactInfo: Abuse Department &lt;abuse AT hartvoorinternetvrijhei (2) {#abuse-department-abuse-at-hartvoorinternetvrijhei}

| Nickname                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [hviv103](https://atlas.torproject.org/#details/D12D357D91DD3B79E2AD9FDB160F9A4558147E05) | 2015-09-06   | Yes         |                     1 |
| [hviv104](https://atlas.torproject.org/#details/81B75D534F91BFB7C57AB67DA10BCEF622582AE8) | 2014-04-09   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

B39AD54B73A70DA68F6FC26CD0A874DE762B7825,48B93C88B90608913C1D7FD9378DBB970BF994EC,035D2E216B065B961E404BD172336050E5AF4EEA,A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13,A853BA9862837B5FC8E4FF784829DB3BE6F53A75,1D3174338A1131A53E098443E76E1103CDED00DC,78BC2254D3B31CD865F7682633AA438212132532,7B700C0C207EBD0002E00F499BE265519AC3C25A,A2534EF23390CAE079B1586F0FDF9CE11F556062,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,E43A346CB81DDF364B6FF68235AFADBA0E8692B8,C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7,4DD902046E7155BBE79C34EE6D53BF7408B98CE4,CB4EBE9C475A60A5F2CDA92C83CE093BD945D940,1A835E3663068222F28F7C5AF3216F4B27B50B57,D12D357D91DD3B79E2AD9FDB160F9A4558147E05,FDAED15C98CFE7A416E5676F614254F78406105C,1B06E7B8B4DAAED1895A73FFDB1B3E24FFBCA0CA,846B3EAAF0C07FF72FC79AEBB11FA3ADC58F240F,4DAD2D02EC7F3D278AF20B119652BC3CC4988D6A,A019AF72731C2731CA90C01B2C5F279289B5E177,D86D10F1ADFCB8C58A521E165837D3A90C699418,B4CA5FDB58A06914689BA23ED2C5FED79CFB3950,04738935F40F06E03312097C7411EEC67EB99E93,F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A