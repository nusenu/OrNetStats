---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2017-10-10 20:00 UTC**

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


## ContactInfo: $ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA (4) {#contactgpgfingerprint-contactname-conta}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [netnognrelay](https://atlas.torproject.org/#details/57436E58262FCB32263108C23631DC6C7064A17F)   | 2017-07-16   | Yes         |                     1 |
| [PieceOfShitSrv](https://atlas.torproject.org/#details/8D13A1B5F11E79DCD3B2868215251769C8076AA1) | 2017-03-05   | Yes         |                     1 |
| [justhelpingout](https://atlas.torproject.org/#details/16273E9FFDF2B5EF64EE187AB1A71D6C6287F02C) | 2017-08-14   | Yes         |                     1 |
| [hacktheplanet](https://atlas.torproject.org/#details/FF48FFC2C35AEDAF87EBE2B20A0EC14579D9C0FC)  | 2017-09-24   | No          |                     1 |

## ContactInfo: Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB (13) {#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb}

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
| [CalyxInstitute03](https://atlas.torproject.org/#details/84D361B736A8CD1E8818D0FC186892E91AB76881) | 2013-06-23   | No          |                    12 |
| [CalyxInstitute13](https://atlas.torproject.org/#details/A7C7EB2A0DFB2E3FFFC12B7756707433DD550F9E) | 2014-12-20   | No          |                    13 |
| [CalyxInstitute12](https://atlas.torproject.org/#details/B34CC9056250847D1980F08285B01CF0B718C0B6) | 2014-12-16   | No          |                    12 |
| [CalyxInstitute01](https://atlas.torproject.org/#details/E4D1F25DFBE484208866BA4A1A958B73127CB0AD) | 2013-06-11   | No          |                    12 |

## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv (3) {#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay2](https://atlas.torproject.org/#details/D5B8C38539C509380767D4DE20DE84CF84EE8299)      | 2016-09-05   | Yes         |                     1 |
| [NeelTorExitUSWest](https://atlas.torproject.org/#details/0D8211D34F29F51D690303E319766E1B7C28BADB)  | 2017-05-25   | No          |                     1 |
| [NeelTorExitUSMdwst](https://atlas.torproject.org/#details/46583FB9E1E914D26D05F8073A740857DBCDFE70) | 2017-08-23   | No          |                     1 |

## ContactInfo: AnonyMaid Team &lt;info@anonymaid.net&gt; (4) {#anonymaid-team-infoanonymaidnet}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [DutchDroid](https://atlas.torproject.org/#details/BF5068641A54A9433CA612BDFF7F098B72EB9762)  | 2017-08-09   | Yes         |                     1 |
| [DutchMaid04](https://atlas.torproject.org/#details/44182447E5E9F2997754CE53FFB4881942B5B3C6) | 2017-10-01   | No          |                     1 |
| [DutchMaid03](https://atlas.torproject.org/#details/7FAB8FED1A821455902BEA3388A6DA5BF6F78198) | 2017-10-01   | No          |                     1 |
| [DutchMaid02](https://atlas.torproject.org/#details/F0AAF9279CF541144C374D4D60CDCFA45CDB86E3) | 2017-07-05   | No          |                     1 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://atlas.torproject.org/#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://atlas.torproject.org/#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |

## ContactInfo: emerson tor@emersonveenstra.net bitcoin:126gyYcBji (5) {#emerson-toremersonveenstranet-bitcoin126gyycbji}

| Nickname                                                                                     | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [emvnrelay1](https://atlas.torproject.org/#details/C20681C998369024A91C6692100A1080E1FCCC28) | 2017-09-30   | Yes         |                     5 |
| [emvnrelay2](https://atlas.torproject.org/#details/056CF262BCC6E4AE8FFB22790DAB8D34C519CC1B) | 2017-10-02   | Yes         |                     5 |
| [emvnexit3](https://atlas.torproject.org/#details/24337497701FD761A5E7FB7A4E5DC72D5421045F)  | 2017-10-04   | No          |                     1 |
| [nodvexit2](https://atlas.torproject.org/#details/4B007F4B6DF506278BB2CE54F08767728551867A)  | 2017-10-02   | No          |                     5 |
| [emvnexit1](https://atlas.torproject.org/#details/7E42EB420668BBE44DA9974B4F81B527A220CAEE)  | 2017-10-02   | No          |                     5 |

## ContactInfo: VSIF Support &lt;support AT vsif dot ca&gt; (5) {#vsif-support-support-at-vsif-dot-ca}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [VSIFweb](https://atlas.torproject.org/#details/78378DDD015C4E1C9242A5EC41158AF1E24CF43E)        | 2017-06-23   | Yes         |                     1 |
| [VSIFviking1](https://atlas.torproject.org/#details/1DEB985E3EEC0E7E0F6A887B417065E63522C5E2)    | 2017-06-15   | No          |                     4 |
| [VSIFenterprise](https://atlas.torproject.org/#details/59AE2B55941324B24354ADAAF971FC2C9F836963) | 2017-06-15   | No          |                     4 |
| [VSIFsalyut4](https://atlas.torproject.org/#details/D2461A903A754DEA625827AB333A2ECD06CE2E43)    | 2017-06-09   | No          |                     4 |
| [VSIFskylab](https://atlas.torproject.org/#details/F13B97699EF7328A6289E5C2540560903CBC79A8)     | 2017-06-04   | No          |                     4 |

## ContactInfo: visualbasic033@gmail.com (3) {#visualbasic033gmailcom}

| Nickname                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [doutreval](https://atlas.torproject.org/#details/CB4EBE9C475A60A5F2CDA92C83CE093BD945D940) | 2015-12-04   | Yes         |                     1 |
| [dlavolos](https://atlas.torproject.org/#details/6E41F9BC3FE626D1897865CE9A9335D09A8DA5FE)  | 2016-03-07   | No          |                     1 |
| [sowinetz](https://atlas.torproject.org/#details/A041B285B228241C3185483EEF42F0BC96D40BFB)  | 2016-08-08   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

C20681C998369024A91C6692100A1080E1FCCC28,C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7,78378DDD015C4E1C9242A5EC41158AF1E24CF43E,57436E58262FCB32263108C23631DC6C7064A17F,BF5068641A54A9433CA612BDFF7F098B72EB9762,056CF262BCC6E4AE8FFB22790DAB8D34C519CC1B,16273E9FFDF2B5EF64EE187AB1A71D6C6287F02C,D5B8C38539C509380767D4DE20DE84CF84EE8299,8D13A1B5F11E79DCD3B2868215251769C8076AA1,CB4EBE9C475A60A5F2CDA92C83CE093BD945D940