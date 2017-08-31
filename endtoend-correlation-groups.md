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


## ContactInfo: see https://www.artikel5ev.de/torcontact/ (12) {#see-httpswwwartikel5evdetorcontact}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [dc6jgk6](https://atlas.torproject.org/#details/A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13)             | 2016-10-06   | Yes         |                    21 |
| [dc6jgk7](https://atlas.torproject.org/#details/F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A)             | 2016-11-04   | Yes         |                    21 |
| [dc6jgk10](https://atlas.torproject.org/#details/D86D10F1ADFCB8C58A521E165837D3A90C699418)            | 2016-11-11   | Yes         |                    21 |
| [dc6jgk9](https://atlas.torproject.org/#details/78BC2254D3B31CD865F7682633AA438212132532)             | 2016-11-11   | Yes         |                    21 |
| [dc6jgk8](https://atlas.torproject.org/#details/1B06E7B8B4DAAED1895A73FFDB1B3E24FFBCA0CA)             | 2016-11-06   | Yes         |                    21 |
| [dc6jgk11](https://atlas.torproject.org/#details/7B700C0C207EBD0002E00F499BE265519AC3C25A)            | 2016-11-11   | Yes         |                    21 |
| [utzer1](https://atlas.torproject.org/#details/B4CA5FDB58A06914689BA23ED2C5FED79CFB3950)              | 2017-03-01   | Yes         |                    21 |
| [dc6jgk12](https://atlas.torproject.org/#details/A853BA9862837B5FC8E4FF784829DB3BE6F53A75)            | 2016-11-13   | Yes         |                    21 |
| [noiwillnotfixfamily](https://atlas.torproject.org/#details/4DAD2D02EC7F3D278AF20B119652BC3CC4988D6A) | 2017-04-27   | Yes         |                     1 |
| [artikel5ev1](https://atlas.torproject.org/#details/0BC8BA32CC3CB0F598E0C92778F7C0946DFBCE91)         | 2016-10-19   | No          |                    21 |
| [artikel5ev3](https://atlas.torproject.org/#details/7458E9E8AA636DE53F383575E41AA4A6227376D9)         | 2016-11-07   | No          |                    21 |
| [artikel5ev2](https://atlas.torproject.org/#details/DC2191663DD4BAECB34F949CCAC3FDA004CE5BCE)         | 2016-10-29   | No          |                    21 |

## ContactInfo: $ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA (4) {#contactgpgfingerprint-contactname-conta}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [netnognrelay](https://atlas.torproject.org/#details/57436E58262FCB32263108C23631DC6C7064A17F)   | 2017-07-16   | Yes         |                     1 |
| [justhelpingout](https://atlas.torproject.org/#details/16273E9FFDF2B5EF64EE187AB1A71D6C6287F02C) | 2017-08-14   | Yes         |                     1 |
| [PieceOfShitSrv](https://atlas.torproject.org/#details/8D13A1B5F11E79DCD3B2868215251769C8076AA1) | 2017-03-05   | Yes         |                     1 |
| [hacktheplanet](https://atlas.torproject.org/#details/F484276FC3BFE743AEFDA937E25C26518D1226BE)  | 2017-08-13   | No          |                     1 |

## ContactInfo: Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB (13) {#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CalyxInstitute03](https://atlas.torproject.org/#details/84D361B736A8CD1E8818D0FC186892E91AB76881) | 2013-06-23   | No          |                    13 |

## ContactInfo: George Shuklin &lt;george.shuklin@gmail.com&gt; (2) {#george-shuklin-georgeshuklingmailcom}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NSA42](https://atlas.torproject.org/#details/20198F4E1A0E23F32C6265DF749BA003DDAF79B1)       | 2016-02-15   | Yes         |                     1 |
| [freeBogatov](https://atlas.torproject.org/#details/CB6FF27F3A474F6A67D20683C9C97DC275F2658F) | 2016-07-21   | No          |                     1 |

## ContactInfo: tor at h0sted dot net tor-relay.co (5) {#torath0steddotnet-tor-relayco}

| Nickname                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [UK2h0stedt0r](https://atlas.torproject.org/#details/4603E997819AC615035369A9DC947FF0CF049D30) | 2017-06-10   | Yes         |                     4 |
| [UK1h0stedt0r](https://atlas.torproject.org/#details/0EEA0B924A7481EC0497304C2BEBD76E731B464C) | 2017-06-09   | No          |                     4 |
| [FR1h0stedt0r](https://atlas.torproject.org/#details/3C84885900080E74ED475A0B904ADCF9C5116887) | 2017-06-30   | No          |                     5 |
| [AU1h0stedt0r](https://atlas.torproject.org/#details/5608145DCDBBFDF4D566C90DC72220298F723CFA) | 2017-06-12   | No          |                     2 |
| [UK4h0stedt0r](https://atlas.torproject.org/#details/BAC503E941F649EDD25FB61066DD08D0635922F9) | 2017-07-21   | No          |                     4 |

## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv (3) {#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay2](https://atlas.torproject.org/#details/D5B8C38539C509380767D4DE20DE84CF84EE8299)      | 2016-09-05   | Yes         |                     2 |
| [NeelTorExitUSWest](https://atlas.torproject.org/#details/0D8211D34F29F51D690303E319766E1B7C28BADB)  | 2017-05-25   | No          |                     2 |
| [NeelTorExitUSMdwst](https://atlas.torproject.org/#details/46583FB9E1E914D26D05F8073A740857DBCDFE70) | 2017-08-23   | No          |                     1 |

## ContactInfo: Brandon Kuschel &lt;kusch023 AT nospam UMN dot edu. (2) {#brandon-kuschel-kusch023-at-nospam-umn-dot-edu}

| Nickname                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Charybdis](https://atlas.torproject.org/#details/8096552438C9B8AB82BDCB8D5896128B61AAFAF9) | 2016-10-26   | Yes         |                     1 |

## ContactInfo: Syncaddict &lt;tor-node-operations@syncaddict.net&gt; (2) {#syncaddict-tor-node-operationssyncaddictnet}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [DutchDroid](https://atlas.torproject.org/#details/BF5068641A54A9433CA612BDFF7F098B72EB9762)  | 2017-08-09   | Yes         |                     1 |
| [DutchOutlet](https://atlas.torproject.org/#details/F0AAF9279CF541144C374D4D60CDCFA45CDB86E3) | 2017-07-05   | No          |                     1 |

## ContactInfo: visualbasic033@gmail.com (3) {#visualbasic033gmailcom}

| Nickname                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [doutreval](https://atlas.torproject.org/#details/CB4EBE9C475A60A5F2CDA92C83CE093BD945D940) | 2015-12-04   | Yes         |                     1 |
| [dlavolos](https://atlas.torproject.org/#details/6E41F9BC3FE626D1897865CE9A9335D09A8DA5FE)  | 2016-03-07   | No          |                     1 |
| [sowinetz](https://atlas.torproject.org/#details/A041B285B228241C3185483EEF42F0BC96D40BFB)  | 2016-08-08   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://atlas.torproject.org/#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://atlas.torproject.org/#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://atlas.torproject.org/#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |


## Fingerprint List of Guard-only Relays in E2E Groups

4603E997819AC615035369A9DC947FF0CF049D30,1B06E7B8B4DAAED1895A73FFDB1B3E24FFBCA0CA,D86D10F1ADFCB8C58A521E165837D3A90C699418,57436E58262FCB32263108C23631DC6C7064A17F,B4CA5FDB58A06914689BA23ED2C5FED79CFB3950,F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A,20198F4E1A0E23F32C6265DF749BA003DDAF79B1,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,BF5068641A54A9433CA612BDFF7F098B72EB9762,A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13,16273E9FFDF2B5EF64EE187AB1A71D6C6287F02C,A853BA9862837B5FC8E4FF784829DB3BE6F53A75,D5B8C38539C509380767D4DE20DE84CF84EE8299,A20840A16CB658024B0D3A0E3F19A9C0E34C843F,78BC2254D3B31CD865F7682633AA438212132532,8D13A1B5F11E79DCD3B2868215251769C8076AA1,7B700C0C207EBD0002E00F499BE265519AC3C25A,CB4EBE9C475A60A5F2CDA92C83CE093BD945D940,4DAD2D02EC7F3D278AF20B119652BC3CC4988D6A,8096552438C9B8AB82BDCB8D5896128B61AAFAF9