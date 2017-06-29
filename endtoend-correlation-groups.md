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
| [dc6jgk7](https://atlas.torproject.org/#details/F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A)             | 2016-11-04   | Yes         |                    21 |
| [dc6jgk8](https://atlas.torproject.org/#details/1B06E7B8B4DAAED1895A73FFDB1B3E24FFBCA0CA)             | 2016-11-06   | Yes         |                    21 |
| [dc6jgk5](https://atlas.torproject.org/#details/846B3EAAF0C07FF72FC79AEBB11FA3ADC58F240F)             | 2016-09-05   | Yes         |                    21 |
| [dc6jgk9](https://atlas.torproject.org/#details/78BC2254D3B31CD865F7682633AA438212132532)             | 2016-11-11   | Yes         |                    21 |
| [dc6jgk6](https://atlas.torproject.org/#details/A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13)             | 2016-10-06   | Yes         |                    21 |
| [utzer1](https://atlas.torproject.org/#details/B4CA5FDB58A06914689BA23ED2C5FED79CFB3950)              | 2017-03-01   | Yes         |                    21 |
| [dc6jgk12](https://atlas.torproject.org/#details/A853BA9862837B5FC8E4FF784829DB3BE6F53A75)            | 2016-11-13   | Yes         |                    21 |
| [dc6jgk10](https://atlas.torproject.org/#details/D86D10F1ADFCB8C58A521E165837D3A90C699418)            | 2016-11-11   | Yes         |                    21 |
| [noiwillnotfixfamily](https://atlas.torproject.org/#details/4DAD2D02EC7F3D278AF20B119652BC3CC4988D6A) | 2017-04-27   | Yes         |                     1 |
| [utzer2](https://atlas.torproject.org/#details/035D2E216B065B961E404BD172336050E5AF4EEA)              | 2017-03-02   | Yes         |                    21 |
| [artikel5ev1](https://atlas.torproject.org/#details/0BC8BA32CC3CB0F598E0C92778F7C0946DFBCE91)         | 2016-10-19   | No          |                    21 |
| [artikel5ev3](https://atlas.torproject.org/#details/7458E9E8AA636DE53F383575E41AA4A6227376D9)         | 2016-11-07   | No          |                    21 |
| [artikel5ev2](https://atlas.torproject.org/#details/DC2191663DD4BAECB34F949CCAC3FDA004CE5BCE)         | 2016-10-29   | No          |                    21 |

## ContactInfo: snaptorg at gmail , com &gt;&gt; bitcoin:1DmvqGnoexBSzSF (5) {#snaptorgatgmailcom--bitcoin1dmvqgnoexbszsf}

| Nickname                                                                                        | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [SnapTorSTRAS](https://atlas.torproject.org/#details/04738935F40F06E03312097C7411EEC67EB99E93)  | 2016-11-26   | Yes         |                     4 |
| [SnapTorZie](https://atlas.torproject.org/#details/A019AF72731C2731CA90C01B2C5F279289B5E177)    | 2017-05-03   | Yes         |                     1 |
| [SnapTorUSA](https://atlas.torproject.org/#details/48B93C88B90608913C1D7FD9378DBB970BF994EC)    | 2017-03-12   | Yes         |                     4 |
| [SnapTorCAN](https://atlas.torproject.org/#details/B39AD54B73A70DA68F6FC26CD0A874DE762B7825)    | 2016-11-12   | Yes         |                     4 |
| [SnapTorExitUS](https://atlas.torproject.org/#details/B164C656D44C1936E6D5E79183E3C7F341C663CD) | 2017-03-12   | No          |                     4 |

## ContactInfo: Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w (12) {#nicholas-merrill-nick-at-calyx-dot-com-btc---14w}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CalyxInstitute07](https://atlas.torproject.org/#details/1B9FACF25E17D26E307EA7CFA7D455B144B032E5) | 2013-11-05   | Yes         |                    11 |
| [CalyxInstitute10](https://atlas.torproject.org/#details/42ED91DD3768F6A2A194D094A7432CBE8DA004B1) | 2016-04-01   | Yes         |                     4 |
| [CalyxInstitute14](https://atlas.torproject.org/#details/0011BD2485AD45D984EC4159C88FC066E5E3300E) | 2014-12-23   | No          |                    12 |
| [CalyxInstitute08](https://atlas.torproject.org/#details/0B5E5E70FFEA9C7F9FFD13B8E16916A608F3E9EB) | 2013-11-12   | No          |                    11 |
| [CalyxInstitute15](https://atlas.torproject.org/#details/47E49319DD67784F1E65B5793371BE467365979E) | 2015-08-21   | No          |                    11 |
| [CalyxInstitute04](https://atlas.torproject.org/#details/501B3DBF250B094A05CA5DBC424AD4C3D46721A2) | 2013-07-08   | No          |                    11 |
| [CalyxInstitute11](https://atlas.torproject.org/#details/6C143720FFF8469EF6A5C5B4066366340CF6C0D1) | 2014-11-24   | No          |                    12 |
| [CalyxInstitute06](https://atlas.torproject.org/#details/6F4E9FD00D4251D98BE96FB1AA546FE34676A95B) | 2013-11-23   | No          |                    11 |
| [CalyxInstitute09](https://atlas.torproject.org/#details/7761DDC7EB1BE26D4155F74A15F12C32A36FE0F2) | 2013-11-19   | No          |                    11 |
| [CalyxInstitute13](https://atlas.torproject.org/#details/A7C7EB2A0DFB2E3FFFC12B7756707433DD550F9E) | 2014-12-20   | No          |                    12 |
| [CalyxInstitute12](https://atlas.torproject.org/#details/B34CC9056250847D1980F08285B01CF0B718C0B6) | 2014-12-16   | No          |                    11 |
| [CalyxInstitute01](https://atlas.torproject.org/#details/E4D1F25DFBE484208866BA4A1A958B73127CB0AD) | 2013-06-11   | No          |                    11 |

## ContactInfo: yscoder@foxmail.com (4) {#yscoderfoxmailcom}

| Nickname                                                                                          | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [keepongoingYes](https://atlas.torproject.org/#details/71D1213DE3F8982ED8653DB116702404054BAC62)  | 2017-05-31   | Yes         |                     1 |
| [keepongoing](https://atlas.torproject.org/#details/D844412187933013C9D36F32AC279D72945F0BD0)     | 2017-05-31   | Yes         |                     1 |
| [xietongguanguan](https://atlas.torproject.org/#details/1D5DD271A465B227B35526FA0A82658BDDF9680E) | 2017-06-08   | No          |                     1 |
| [xietongguan](https://atlas.torproject.org/#details/C567E7F2CC9335ECED038FE564A64974B9E2BC88)     | 2017-06-08   | No          |                     1 |

## ContactInfo: Abuse Department &lt;abuse AT hartvoorinternetvrijhei (2) {#abuse-department-abuse-at-hartvoorinternetvrijhei}

| Nickname                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [hviv103](https://atlas.torproject.org/#details/D12D357D91DD3B79E2AD9FDB160F9A4558147E05) | 2015-09-06   | Yes         |                     1 |
| [hviv104](https://atlas.torproject.org/#details/81B75D534F91BFB7C57AB67DA10BCEF622582AE8) | 2014-04-09   | No          |                     1 |

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

42ED91DD3768F6A2A194D094A7432CBE8DA004B1,B39AD54B73A70DA68F6FC26CD0A874DE762B7825,71D1213DE3F8982ED8653DB116702404054BAC62,48B93C88B90608913C1D7FD9378DBB970BF994EC,035D2E216B065B961E404BD172336050E5AF4EEA,A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13,A853BA9862837B5FC8E4FF784829DB3BE6F53A75,78BC2254D3B31CD865F7682633AA438212132532,CB4EBE9C475A60A5F2CDA92C83CE093BD945D940,1A835E3663068222F28F7C5AF3216F4B27B50B57,D844412187933013C9D36F32AC279D72945F0BD0,D12D357D91DD3B79E2AD9FDB160F9A4558147E05,1B9FACF25E17D26E307EA7CFA7D455B144B032E5,1B06E7B8B4DAAED1895A73FFDB1B3E24FFBCA0CA,846B3EAAF0C07FF72FC79AEBB11FA3ADC58F240F,4DAD2D02EC7F3D278AF20B119652BC3CC4988D6A,A019AF72731C2731CA90C01B2C5F279289B5E177,D86D10F1ADFCB8C58A521E165837D3A90C699418,B4CA5FDB58A06914689BA23ED2C5FED79CFB3950,04738935F40F06E03312097C7411EEC67EB99E93,F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A