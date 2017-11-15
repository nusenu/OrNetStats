---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2017-11-15 08:00 UTC**

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


## ContactInfo: tormazter@sentries.org z is s (3) {#tormaztersentriesorg-z-is-s}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [SentriesExperiment4](https://atlas.torproject.org/#details/49F5F13DAA45D6BF6A97DBD5E008DF99F50207DD) | 2017-11-06   | Yes         |                     3 |
| [SentriesExit2](https://atlas.torproject.org/#details/366E36894AF7ED5AEAE3D26FBEBD3FA29AA34FDD)       | 2016-09-11   | No          |                     2 |
| [SentriesExit1](https://atlas.torproject.org/#details/EBFBFC15C343AE2A16DFBED651E44DCA81E29083)       | 2016-09-01   | No          |                     2 |

## ContactInfo: AnonyMaid Team &lt;info@anonymaid.net&gt; (4) {#anonymaid-team-infoanonymaidnet}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [DutchDroid](https://atlas.torproject.org/#details/BF5068641A54A9433CA612BDFF7F098B72EB9762)  | 2017-08-09   | Yes         |                     1 |
| [DutchMaid04](https://atlas.torproject.org/#details/44182447E5E9F2997754CE53FFB4881942B5B3C6) | 2017-10-01   | No          |                     1 |
| [DutchMaid03](https://atlas.torproject.org/#details/7FAB8FED1A821455902BEA3388A6DA5BF6F78198) | 2017-10-01   | No          |                     1 |
| [DutchMaid02](https://atlas.torproject.org/#details/F0AAF9279CF541144C374D4D60CDCFA45CDB86E3) | 2017-07-05   | No          |                     1 |

## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv (3) {#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay2](https://atlas.torproject.org/#details/D5B8C38539C509380767D4DE20DE84CF84EE8299)      | 2016-09-05   | Yes         |                     1 |
| [NeelTorRelay1](https://atlas.torproject.org/#details/3A3811F5ECD29528E3855C76B7B58D9B94AAEC51)      | 2017-08-28   | Yes         |                     2 |
| [NeelTorExitUSMdwst](https://atlas.torproject.org/#details/46583FB9E1E914D26D05F8073A740857DBCDFE70) | 2017-08-23   | No          |                     2 |

## ContactInfo: VSIF Support &lt;support AT vsif dot ca&gt; (5) {#vsif-support-support-at-vsif-dot-ca}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [VSIFweb](https://atlas.torproject.org/#details/78378DDD015C4E1C9242A5EC41158AF1E24CF43E)        | 2017-06-23   | Yes         |                     1 |
| [VSIFviking1](https://atlas.torproject.org/#details/1DEB985E3EEC0E7E0F6A887B417065E63522C5E2)    | 2017-06-15   | No          |                     4 |
| [VSIFenterprise](https://atlas.torproject.org/#details/59AE2B55941324B24354ADAAF971FC2C9F836963) | 2017-06-15   | No          |                     4 |
| [VSIFsalyut4](https://atlas.torproject.org/#details/D2461A903A754DEA625827AB333A2ECD06CE2E43)    | 2017-06-09   | No          |                     4 |
| [VSIFskylab](https://atlas.torproject.org/#details/F13B97699EF7328A6289E5C2540560903CBC79A8)     | 2017-06-04   | No          |                     4 |


## Fingerprint List of Guard-only Relays in E2E Groups

78378DDD015C4E1C9242A5EC41158AF1E24CF43E,49F5F13DAA45D6BF6A97DBD5E008DF99F50207DD,BF5068641A54A9433CA612BDFF7F098B72EB9762,D5B8C38539C509380767D4DE20DE84CF84EE8299,3A3811F5ECD29528E3855C76B7B58D9B94AAEC51