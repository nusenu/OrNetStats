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

Once MyFamily is fixed the relays will automatically disappear from this page (within a ~week).
If you need help with the MyFamily configuration you can reach out to the
[tor-relays mailing list](https://lists.torproject.org/cgi-bin/mailman/listinfo/tor-relays).
You can also use tools that handle MyFamily automatically (I maintain an ansible role - 
[relayor](https://medium.com/@nusenu/deploying-tor-relays-with-ansible-6612593fa34d))
If someone else is using your contactInfo please send an email to bad-relays AT lists DOT torproject DOT org.


## ContactInfo: see https://www.artikel5ev.de/torcontact/ (14) {#see-httpswwwartikel5evdetorcontact}

| Nickname                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [dc6jgk8](https://atlas.torproject.org/#details/1B06E7B8B4DAAED1895A73FFDB1B3E24FFBCA0CA)      | 2016-11-06   | Yes         |                    21 |
| [dc6jgk11](https://atlas.torproject.org/#details/7B700C0C207EBD0002E00F499BE265519AC3C25A)     | 2016-11-11   | Yes         |                    21 |
| [dc6jgk12](https://atlas.torproject.org/#details/A853BA9862837B5FC8E4FF784829DB3BE6F53A75)     | 2016-11-13   | Yes         |                    21 |
| [Artikel5ev6](https://atlas.torproject.org/#details/4DD902046E7155BBE79C34EE6D53BF7408B98CE4)  | 2017-03-05   | Yes         |                    21 |
| [dc6jgk9](https://atlas.torproject.org/#details/78BC2254D3B31CD865F7682633AA438212132532)      | 2016-11-11   | Yes         |                    21 |
| [dc6jgk5](https://atlas.torproject.org/#details/846B3EAAF0C07FF72FC79AEBB11FA3ADC58F240F)      | 2016-09-05   | Yes         |                    21 |
| [dc6jgk7](https://atlas.torproject.org/#details/F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A)      | 2016-11-04   | Yes         |                    21 |
| [dc6jgk6](https://atlas.torproject.org/#details/A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13)      | 2016-10-06   | Yes         |                    21 |
| [dc6jgk10](https://atlas.torproject.org/#details/D86D10F1ADFCB8C58A521E165837D3A90C699418)     | 2016-11-11   | Yes         |                    21 |
| [dc6jgk15TEST](https://atlas.torproject.org/#details/4DAD2D02EC7F3D278AF20B119652BC3CC4988D6A) | 2017-04-27   | Yes         |                     1 |
| [utzer2](https://atlas.torproject.org/#details/035D2E216B065B961E404BD172336050E5AF4EEA)       | 2017-03-02   | Yes         |                    21 |
| [artikel5ev1](https://atlas.torproject.org/#details/0BC8BA32CC3CB0F598E0C92778F7C0946DFBCE91)  | 2016-10-19   | No          |                    21 |
| [tweinbrenner](https://atlas.torproject.org/#details/340C8447003B79B4EF30617F983BDEA5EF1E254F) | 2017-03-03   | No          |                    21 |
| [dc6jgk1](https://atlas.torproject.org/#details/486740353B905AA4731F82C0B4CC25821A62C6E3)      | 2014-06-09   | No          |                    21 |
| [artikel5ev3](https://atlas.torproject.org/#details/7458E9E8AA636DE53F383575E41AA4A6227376D9)  | 2016-11-07   | No          |                    21 |
| [dc6jgk4](https://atlas.torproject.org/#details/868A253C330F40FBE435D9320849397F85823E86)      | 2014-08-04   | No          |                    21 |
| [h3rmi](https://atlas.torproject.org/#details/A690C6AA8102C027D297AF3401BFE16918CCF7A6)        | 2016-07-22   | No          |                    21 |
| [utzer1](https://atlas.torproject.org/#details/B4CA5FDB58A06914689BA23ED2C5FED79CFB3950)       | 2017-03-01   | No          |                    21 |
| [dc6jgk3](https://atlas.torproject.org/#details/B5E0F84850C6948839F8BBB4E7E5B5A8F490EA4F)      | 2014-05-17   | No          |                    21 |
| [artikel5ev2](https://atlas.torproject.org/#details/DC2191663DD4BAECB34F949CCAC3FDA004CE5BCE)  | 2016-10-29   | No          |                    21 |
| [dc6jgk2](https://atlas.torproject.org/#details/E754AA9939DE56E388390930B302142FA319085F)      | 2014-04-11   | No          |                    21 |

## ContactInfo: aTorRelay@gmail.com (9) {#atorrelaygmailcom}

| Nickname                                                                                     | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Cayambe](https://atlas.torproject.org/#details/EA147A10B261A03B863B428A8EB45513038E6793)    | 2016-10-02   | Yes         |                     6 |
| [Tungurahua](https://atlas.torproject.org/#details/7CB15FA5CD985B9BBD6AC386C62C206A1F391C23) | 2016-10-02   | Yes         |                     6 |
| [Pichincha](https://atlas.torproject.org/#details/68F175CCABE727AA2D2309BCD8789499CEE36ED7)  | 2016-05-24   | Yes         |                     6 |
| [Cotopaxi](https://atlas.torproject.org/#details/4623A9EC53BFD83155929E56D6F7B55B5E718C24)   | 2016-05-24   | Yes         |                     6 |
| [Cuicocha](https://atlas.torproject.org/#details/1447CB81A31B3701F7D5CB82E84B0AF2436189E0)   | 2017-03-21   | No          |                     1 |
| [Illiniza](https://atlas.torproject.org/#details/1A253681CBC0836C71AA7D6D0FC9B01D6B38045F)   | 2017-03-21   | No          |                     1 |
| [Sangay](https://atlas.torproject.org/#details/329EA46CC86E9DF8CDA3F06F3B403D8D89772D47)     | 2016-11-16   | No          |                     6 |
| [Antisana](https://atlas.torproject.org/#details/4FDD4AFD8653DE16EE2DFCD7012570DA953CDF4C)   | 2016-11-19   | No          |                     6 |
| [Atacazo](https://atlas.torproject.org/#details/83E6F0C19588C5601741FB55D007C2374ED66FF3)    | 2017-03-21   | No          |                     1 |

## ContactInfo: $ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA (5) {#contactgpgfingerprint-contactname-conta}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [hacktheplanet](https://atlas.torproject.org/#details/503B81114811247C0D2D1317A929E5100370FB2D)  | 2017-04-01   | Yes         |                     1 |
| [PieceOfShitSrv](https://atlas.torproject.org/#details/8D13A1B5F11E79DCD3B2868215251769C8076AA1) | 2017-03-05   | Yes         |                     1 |
| [hacktheplanet](https://atlas.torproject.org/#details/043199D2C41E640430B77388B80D442D379BD8E2)  | 2017-04-13   | Yes         |                     1 |
| [darknumbat](https://atlas.torproject.org/#details/EE5B1908BC169F219EE9F74637D396D43EC1B58D)     | 2016-12-25   | Yes         |                     1 |
| [celerity](https://atlas.torproject.org/#details/07DE0162672BA711A396D7056E053C1748B566DB)       | 2017-02-09   | No          |                     1 |
| [yougotrelay](https://atlas.torproject.org/#details/75F5826C4DA47146F9D2665BBB10859494DA9E94)    | 2017-03-03   | No          |                     1 |
| [hacktheplanet](https://atlas.torproject.org/#details/CC6510EFBD46295322803A1ED6A13B0E43A43D0C)  | 2017-05-11   | No          |                     1 |

## ContactInfo: Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w (13) {#nicholas-merrill-nick-at-calyx-dot-com-btc---14w}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CalyxInstitute07](https://atlas.torproject.org/#details/1B9FACF25E17D26E307EA7CFA7D455B144B032E5) | 2013-11-05   | Yes         |                    12 |
| [CalyxInstitute10](https://atlas.torproject.org/#details/42ED91DD3768F6A2A194D094A7432CBE8DA004B1) | 2016-04-01   | Yes         |                     4 |
| [CalyxInstitute14](https://atlas.torproject.org/#details/0011BD2485AD45D984EC4159C88FC066E5E3300E) | 2014-12-23   | No          |                    13 |
| [CalyxInstitute08](https://atlas.torproject.org/#details/0B5E5E70FFEA9C7F9FFD13B8E16916A608F3E9EB) | 2013-11-12   | No          |                    12 |
| [CalyxInstitute15](https://atlas.torproject.org/#details/47E49319DD67784F1E65B5793371BE467365979E) | 2015-08-21   | No          |                    12 |
| [CalyxInstitute04](https://atlas.torproject.org/#details/501B3DBF250B094A05CA5DBC424AD4C3D46721A2) | 2013-07-08   | No          |                    12 |
| [CalyxInstitute11](https://atlas.torproject.org/#details/6C143720FFF8469EF6A5C5B4066366340CF6C0D1) | 2014-11-24   | No          |                    13 |
| [CalyxInstitute06](https://atlas.torproject.org/#details/6F4E9FD00D4251D98BE96FB1AA546FE34676A95B) | 2013-11-23   | No          |                    12 |
| [CalyxInstitute09](https://atlas.torproject.org/#details/7761DDC7EB1BE26D4155F74A15F12C32A36FE0F2) | 2013-11-19   | No          |                    12 |
| [CalyxInstitute13](https://atlas.torproject.org/#details/A7C7EB2A0DFB2E3FFFC12B7756707433DD550F9E) | 2014-12-20   | No          |                    13 |
| [CalyxInstitute12](https://atlas.torproject.org/#details/B34CC9056250847D1980F08285B01CF0B718C0B6) | 2014-12-16   | No          |                    12 |
| [CalyxInstitute01](https://atlas.torproject.org/#details/E4D1F25DFBE484208866BA4A1A958B73127CB0AD) | 2013-06-11   | No          |                    12 |

## ContactInfo: snaptorg at gmail , com &gt;&gt; bitcoin:1DmvqGnoexBSzSF (4) {#snaptorgatgmailcom--bitcoin1dmvqgnoexbszsf}

| Nickname                                                                                        | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [SnapTorSTRAS](https://atlas.torproject.org/#details/04738935F40F06E03312097C7411EEC67EB99E93)  | 2016-11-26   | Yes         |                     4 |
| [SnapTorZie](https://atlas.torproject.org/#details/A019AF72731C2731CA90C01B2C5F279289B5E177)    | 2017-05-03   | Yes         |                     1 |
| [SnapTorUSA](https://atlas.torproject.org/#details/48B93C88B90608913C1D7FD9378DBB970BF994EC)    | 2017-03-12   | Yes         |                     4 |
| [SnapTorExitUS](https://atlas.torproject.org/#details/B164C656D44C1936E6D5E79183E3C7F341C663CD) | 2017-03-12   | No          |                     4 |
| [SnapTorCAN](https://atlas.torproject.org/#details/B39AD54B73A70DA68F6FC26CD0A874DE762B7825)    | 2016-11-12   | No          |                     4 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://atlas.torproject.org/#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://atlas.torproject.org/#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |

## ContactInfo: George Shuklin &lt;george.shuklin@gmail.com&gt; (2) {#george-shuklin-georgeshuklingmailcom}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NSA42](https://atlas.torproject.org/#details/20198F4E1A0E23F32C6265DF749BA003DDAF79B1)       | 2016-02-15   | Yes         |                     1 |
| [freeBogatov](https://atlas.torproject.org/#details/CB6FF27F3A474F6A67D20683C9C97DC275F2658F) | 2016-07-21   | No          |                     1 |

## ContactInfo: tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt; (5) {#tornoisebridgenet-admintornoisebridgenet}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [noisebridge01a](https://atlas.torproject.org/#details/1A835E3663068222F28F7C5AF3216F4B27B50B57) | 2015-05-20   | Yes         |                     1 |
| [noiseexit01b](https://atlas.torproject.org/#details/3591E0E966309AD335BE62FF694E8A898F97A6C9)   | 2014-04-16   | No          |                     4 |
| [noiseexit01d](https://atlas.torproject.org/#details/C6F6B70AD9115C65B618B0AF3FD10B0432626CA9)   | 2014-04-16   | No          |                     4 |
| [noiseexit01c](https://atlas.torproject.org/#details/D42EE35F9B62769E782DEA2FC6358ABFAFE7DB66)   | 2014-04-16   | No          |                     4 |
| [noiseexit01a](https://atlas.torproject.org/#details/E93F05C9A7112544A2F132CBB7F6701877140F2A)   | 2014-04-16   | No          |                     4 |

## ContactInfo: torman@memeware.net (2) {#tormanmemewarenet}

| Nickname                                                                                     | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [deeppacket](https://atlas.torproject.org/#details/DFC5F4F0FFCBA62EC816536D46B184E0A1DDE29F) | 2017-04-27   | Yes         |                     1 |
| [thotpatrol](https://atlas.torproject.org/#details/FD7DC7A6FC2890B18085E964879D8D078622D288) | 2017-05-11   | No          |                     1 |

## ContactInfo: visualbasic033@gmail.com (3) {#visualbasic033gmailcom}

| Nickname                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [doutreval](https://atlas.torproject.org/#details/CB4EBE9C475A60A5F2CDA92C83CE093BD945D940) | 2015-12-04   | Yes         |                     1 |
| [dlavolos](https://atlas.torproject.org/#details/6E41F9BC3FE626D1897865CE9A9335D09A8DA5FE)  | 2016-03-07   | No          |                     1 |
| [sowinetz](https://atlas.torproject.org/#details/A041B285B228241C3185483EEF42F0BC96D40BFB)  | 2016-08-08   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

42ED91DD3768F6A2A194D094A7432CBE8DA004B1,EE5B1908BC169F219EE9F74637D396D43EC1B58D,20198F4E1A0E23F32C6265DF749BA003DDAF79B1,48B93C88B90608913C1D7FD9378DBB970BF994EC,035D2E216B065B961E404BD172336050E5AF4EEA,A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13,503B81114811247C0D2D1317A929E5100370FB2D,A853BA9862837B5FC8E4FF784829DB3BE6F53A75,78BC2254D3B31CD865F7682633AA438212132532,7B700C0C207EBD0002E00F499BE265519AC3C25A,C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7,4DD902046E7155BBE79C34EE6D53BF7408B98CE4,CB4EBE9C475A60A5F2CDA92C83CE093BD945D940,DFC5F4F0FFCBA62EC816536D46B184E0A1DDE29F,1A835E3663068222F28F7C5AF3216F4B27B50B57,1B9FACF25E17D26E307EA7CFA7D455B144B032E5,1B06E7B8B4DAAED1895A73FFDB1B3E24FFBCA0CA,7CB15FA5CD985B9BBD6AC386C62C206A1F391C23,846B3EAAF0C07FF72FC79AEBB11FA3ADC58F240F,4DAD2D02EC7F3D278AF20B119652BC3CC4988D6A,A019AF72731C2731CA90C01B2C5F279289B5E177,D86D10F1ADFCB8C58A521E165837D3A90C699418,043199D2C41E640430B77388B80D442D379BD8E2,8D13A1B5F11E79DCD3B2868215251769C8076AA1,4623A9EC53BFD83155929E56D6F7B55B5E718C24