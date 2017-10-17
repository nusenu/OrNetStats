---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2017-10-17 15:00 UTC**

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


## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv (3) {#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay2](https://atlas.torproject.org/#details/D5B8C38539C509380767D4DE20DE84CF84EE8299)      | 2016-09-05   | Yes         |                     1 |
| [NeelTorExitUSWest](https://atlas.torproject.org/#details/0D8211D34F29F51D690303E319766E1B7C28BADB)  | 2017-05-25   | No          |                     1 |
| [NeelTorExitUSMdwst](https://atlas.torproject.org/#details/46583FB9E1E914D26D05F8073A740857DBCDFE70) | 2017-08-23   | No          |                     2 |

## ContactInfo: torrelays A-T cyb3rwr3ck D-O-T net (2) {#torrelays-a-t-cyb3rwr3ck-d-o-t-net}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [wr3ck3d0ni0n03](https://atlas.torproject.org/#details/85A885433E50B1874F11CEC9BE98451E24660976) | 2017-06-15   | Yes         |                     1 |
| [wr3ck3d0ni0n02](https://atlas.torproject.org/#details/8559AFB9496C349A528C1F0753D3869CE56574D1) | 2016-09-17   | No          |                     1 |

## ContactInfo: VSIF Support &lt;support AT vsif dot ca&gt; (5) {#vsif-support-support-at-vsif-dot-ca}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [VSIFweb](https://atlas.torproject.org/#details/78378DDD015C4E1C9242A5EC41158AF1E24CF43E)        | 2017-06-23   | Yes         |                     1 |
| [VSIFviking1](https://atlas.torproject.org/#details/1DEB985E3EEC0E7E0F6A887B417065E63522C5E2)    | 2017-06-15   | No          |                     4 |
| [VSIFenterprise](https://atlas.torproject.org/#details/59AE2B55941324B24354ADAAF971FC2C9F836963) | 2017-06-15   | No          |                     4 |
| [VSIFsalyut4](https://atlas.torproject.org/#details/D2461A903A754DEA625827AB333A2ECD06CE2E43)    | 2017-06-09   | No          |                     4 |
| [VSIFskylab](https://atlas.torproject.org/#details/F13B97699EF7328A6289E5C2540560903CBC79A8)     | 2017-06-04   | No          |                     4 |

## ContactInfo: emerson tor@emersonveenstra.net bitcoin:126gyYcBji (5) {#emerson-toremersonveenstranet-bitcoin126gyycbji}

| Nickname                                                                                     | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [emvnrelay1](https://atlas.torproject.org/#details/C20681C998369024A91C6692100A1080E1FCCC28) | 2017-09-30   | Yes         |                     5 |
| [emvnrelay2](https://atlas.torproject.org/#details/056CF262BCC6E4AE8FFB22790DAB8D34C519CC1B) | 2017-10-02   | Yes         |                     5 |
| [emvnexit3](https://atlas.torproject.org/#details/24337497701FD761A5E7FB7A4E5DC72D5421045F)  | 2017-10-04   | No          |                     1 |
| [emvnexit2](https://atlas.torproject.org/#details/4B007F4B6DF506278BB2CE54F08767728551867A)  | 2017-10-02   | No          |                     5 |
| [emvnexit1](https://atlas.torproject.org/#details/7E42EB420668BBE44DA9974B4F81B527A220CAEE)  | 2017-10-02   | No          |                     5 |

## ContactInfo: AnonyMaid Team &lt;info@anonymaid.net&gt; (4) {#anonymaid-team-infoanonymaidnet}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [DutchDroid](https://atlas.torproject.org/#details/BF5068641A54A9433CA612BDFF7F098B72EB9762)  | 2017-08-09   | Yes         |                     1 |
| [DutchMaid04](https://atlas.torproject.org/#details/44182447E5E9F2997754CE53FFB4881942B5B3C6) | 2017-10-01   | No          |                     1 |
| [DutchMaid03](https://atlas.torproject.org/#details/7FAB8FED1A821455902BEA3388A6DA5BF6F78198) | 2017-10-01   | No          |                     1 |
| [DutchMaid02](https://atlas.torproject.org/#details/F0AAF9279CF541144C374D4D60CDCFA45CDB86E3) | 2017-07-05   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://atlas.torproject.org/#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://atlas.torproject.org/#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://atlas.torproject.org/#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://atlas.torproject.org/#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://atlas.torproject.org/#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |

## ContactInfo: visualbasic033@gmail.com (2) {#visualbasic033gmailcom}

| Nickname                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [doutreval](https://atlas.torproject.org/#details/CB4EBE9C475A60A5F2CDA92C83CE093BD945D940) | 2015-12-04   | Yes         |                     1 |
| [dlavolos](https://atlas.torproject.org/#details/6E41F9BC3FE626D1897865CE9A9335D09A8DA5FE)  | 2016-03-07   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

C20681C998369024A91C6692100A1080E1FCCC28,C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7,78378DDD015C4E1C9242A5EC41158AF1E24CF43E,85A885433E50B1874F11CEC9BE98451E24660976,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,BF5068641A54A9433CA612BDFF7F098B72EB9762,056CF262BCC6E4AE8FFB22790DAB8D34C519CC1B,D5B8C38539C509380767D4DE20DE84CF84EE8299,CB4EBE9C475A60A5F2CDA92C83CE093BD945D940