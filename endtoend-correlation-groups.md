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


## ContactInfo: aTorRelay@gmail.com (9) {#atorrelaygmailcom}

| Nickname                                                                                     | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Pichincha](https://atlas.torproject.org/#details/68F175CCABE727AA2D2309BCD8789499CEE36ED7)  | 2016-05-24   | Yes         |                     8 |
| [Cotopaxi](https://atlas.torproject.org/#details/4623A9EC53BFD83155929E56D6F7B55B5E718C24)   | 2016-05-24   | Yes         |                     8 |
| [Tungurahua](https://atlas.torproject.org/#details/7CB15FA5CD985B9BBD6AC386C62C206A1F391C23) | 2016-10-02   | Yes         |                     8 |
| [Cayambe](https://atlas.torproject.org/#details/EA147A10B261A03B863B428A8EB45513038E6793)    | 2016-10-02   | Yes         |                     8 |
| [Cuicocha](https://atlas.torproject.org/#details/1447CB81A31B3701F7D5CB82E84B0AF2436189E0)   | 2017-03-21   | No          |                     1 |
| [Illiniza](https://atlas.torproject.org/#details/1A253681CBC0836C71AA7D6D0FC9B01D6B38045F)   | 2017-03-21   | No          |                     1 |
| [Sangay](https://atlas.torproject.org/#details/329EA46CC86E9DF8CDA3F06F3B403D8D89772D47)     | 2016-11-16   | No          |                     8 |
| [Antisana](https://atlas.torproject.org/#details/4FDD4AFD8653DE16EE2DFCD7012570DA953CDF4C)   | 2016-11-19   | No          |                     8 |
| [Atacazo](https://atlas.torproject.org/#details/83E6F0C19588C5601741FB55D007C2374ED66FF3)    | 2017-03-21   | No          |                     1 |
| [inky](https://atlas.torproject.org/#details/C8200264E43F7920B543F8CDAE055E6EECAD658E)       | 2015-11-15   | No          |                     8 |
| [Chimborazo](https://atlas.torproject.org/#details/E81EF60A73B3809F8964F73766B01BAA0A171E20) | 2016-05-23   | No          |                     8 |

## ContactInfo: $ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA (4) {#contactgpgfingerprint-contactname-conta}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [hacktheplanet](https://atlas.torproject.org/#details/503B81114811247C0D2D1317A929E5100370FB2D)  | 2017-04-01   | Yes         |                     1 |
| [PieceOfShitSrv](https://atlas.torproject.org/#details/8D13A1B5F11E79DCD3B2868215251769C8076AA1) | 2017-03-05   | Yes         |                     1 |
| [hacktheplanet](https://atlas.torproject.org/#details/043199D2C41E640430B77388B80D442D379BD8E2)  | 2017-04-13   | Yes         |                     1 |
| [celerity](https://atlas.torproject.org/#details/07DE0162672BA711A396D7056E053C1748B566DB)       | 2017-02-09   | No          |                     1 |
| [hacktheplanet](https://atlas.torproject.org/#details/288C8093654549E816930635C9D7D5F360A3D5B2)  | 2017-05-16   | No          |                     1 |
| [yougotrelay](https://atlas.torproject.org/#details/75F5826C4DA47146F9D2665BBB10859494DA9E94)    | 2017-03-03   | No          |                     1 |
| [darknumbat](https://atlas.torproject.org/#details/EE5B1908BC169F219EE9F74637D396D43EC1B58D)     | 2016-12-25   | No          |                     1 |

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

## ContactInfo: snaptorg at gmail , com &gt;&gt; bitcoin:1DmvqGnoexBSzSF (5) {#snaptorgatgmailcom--bitcoin1dmvqgnoexbszsf}

| Nickname                                                                                        | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [SnapTorZie](https://atlas.torproject.org/#details/A019AF72731C2731CA90C01B2C5F279289B5E177)    | 2017-05-03   | Yes         |                     1 |
| [SnapTorSTRAS](https://atlas.torproject.org/#details/04738935F40F06E03312097C7411EEC67EB99E93)  | 2016-11-26   | Yes         |                     4 |
| [SnapTorCAN](https://atlas.torproject.org/#details/B39AD54B73A70DA68F6FC26CD0A874DE762B7825)    | 2016-11-12   | Yes         |                     4 |
| [SnapTorUSA](https://atlas.torproject.org/#details/48B93C88B90608913C1D7FD9378DBB970BF994EC)    | 2017-03-12   | Yes         |                     4 |
| [SnapTorExitUS](https://atlas.torproject.org/#details/B164C656D44C1936E6D5E79183E3C7F341C663CD) | 2017-03-12   | No          |                     4 |

## ContactInfo: echo gbe@tbbqsryybj.vg rot13 (2) {#echo-gbetbbqsryybjvg--rot13}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [GoodfellowTorRelay](https://atlas.torproject.org/#details/138ED47EE2156E6492FDE0B61338D973C9717F32)  | 2017-01-23   | Yes         |                     1 |
| [GoodfellowTorRelay2](https://atlas.torproject.org/#details/B313688DAF1E90788F5296D416C58FB42CA418E9) | 2017-05-14   | No          |                     1 |

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

## ContactInfo: tor.noisebridge.net &lt;admin@tor.noisebridge.net&gt; (5) {#tornoisebridgenet-admintornoisebridgenet}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [noisebridge01a](https://atlas.torproject.org/#details/1A835E3663068222F28F7C5AF3216F4B27B50B57) | 2015-05-20   | Yes         |                     1 |
| [noiseexit01b](https://atlas.torproject.org/#details/3591E0E966309AD335BE62FF694E8A898F97A6C9)   | 2014-04-16   | No          |                     4 |
| [noiseexit01d](https://atlas.torproject.org/#details/C6F6B70AD9115C65B618B0AF3FD10B0432626CA9)   | 2014-04-16   | No          |                     4 |
| [noiseexit01c](https://atlas.torproject.org/#details/D42EE35F9B62769E782DEA2FC6358ABFAFE7DB66)   | 2014-04-16   | No          |                     4 |
| [noiseexit01a](https://atlas.torproject.org/#details/E93F05C9A7112544A2F132CBB7F6701877140F2A)   | 2014-04-16   | No          |                     4 |


## Fingerprint List of Guard-only Relays in E2E Groups

42ED91DD3768F6A2A194D094A7432CBE8DA004B1,B39AD54B73A70DA68F6FC26CD0A874DE762B7825,20198F4E1A0E23F32C6265DF749BA003DDAF79B1,48B93C88B90608913C1D7FD9378DBB970BF994EC,503B81114811247C0D2D1317A929E5100370FB2D,C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7,CB4EBE9C475A60A5F2CDA92C83CE093BD945D940,DFC5F4F0FFCBA62EC816536D46B184E0A1DDE29F,1A835E3663068222F28F7C5AF3216F4B27B50B57,1B9FACF25E17D26E307EA7CFA7D455B144B032E5,7CB15FA5CD985B9BBD6AC386C62C206A1F391C23,138ED47EE2156E6492FDE0B61338D973C9717F32,A019AF72731C2731CA90C01B2C5F279289B5E177,043199D2C41E640430B77388B80D442D379BD8E2,8D13A1B5F11E79DCD3B2868215251769C8076AA1,4623A9EC53BFD83155929E56D6F7B55B5E718C24,EA147A10B261A03B863B428A8EB45513038E6793,68F175CCABE727AA2D2309BCD8789499CEE36ED7,04738935F40F06E03312097C7411EEC67EB99E93