---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2017-12-09 07:00 UTC**

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


## ContactInfo: $ CONTACT GPG FINGERPRINT $ CONTACT NAME $ CONTA (6) {#contactgpgfingerprint-contactname-conta}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [justhelpingout](https://atlas.torproject.org/#details/C4F69F1DF9D73E3E0046F3793081288DF5C66247) | 2017-11-28   | Yes         |                     1 |
| [PieceOfShitSrv](https://atlas.torproject.org/#details/8D13A1B5F11E79DCD3B2868215251769C8076AA1) | 2017-03-05   | Yes         |                     1 |
| [netnognrelay](https://atlas.torproject.org/#details/BA66A1600751BF6BB39056A40FAD5831CC46AC56)   | 2017-11-13   | Yes         |                     1 |
| [hacktheplanet](https://atlas.torproject.org/#details/9F729DB3AE1ED73B19A846E217255CF017EEB2B5)  | 2017-10-02   | Yes         |                     1 |
| [hacktheplanet](https://atlas.torproject.org/#details/578181FDA505323F16896F1CFCBD025DA8465FA3)  | 2017-11-29   | No          |                     1 |
| [hacktheplanet](https://atlas.torproject.org/#details/6549C60CC844036B7C7C22A75B2C384041EFEAB1)  | 2017-11-29   | No          |                     1 |

## ContactInfo: abuse AT torworld.org - BTC 17iwdtpmgHdPt15twdT2 (6) {#abuse-at-torworldorg---btc-17iwdtpmghdpt15twdt2}

| Nickname                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Freya](https://atlas.torproject.org/#details/88C3708A9D71ECEC1910B63C3FAA5BF60CD7E199)   | 2016-10-28   | Yes         |                     5 |
| [Vor](https://atlas.torproject.org/#details/157106182B9F33663CAEDCD883D302316331DE5E)     | 2016-12-11   | Yes         |                     5 |
| [Mani](https://atlas.torproject.org/#details/B756D7123D759EAB62CB6A09148AD65AC216F3E3)    | 2017-11-25   | Yes         |                     5 |
| [Tyr](https://atlas.torproject.org/#details/C238E705C538F5844B75DF1E082323387212C931)     | 2017-10-13   | Yes         |                     5 |
| [Astraea](https://atlas.torproject.org/#details/660CD5F78740B89A34A5C31BE46877EFD891163A) | 2017-11-27   | No          |                     2 |
| [Gawain](https://atlas.torproject.org/#details/CDAF4916D0553E1E7B81CF83556073761E98A5F4)  | 2017-12-01   | No          |                     2 |

## ContactInfo: Viktor &lt;vnikolov AT vnikolov dot cz&gt; (4) {#viktor-vnikolov-at-vnikolov-dot-cz}

| Nickname                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [torzabehlice](https://atlas.torproject.org/#details/B6904ADD4C0D10CDA7179E051962350A69A63243) | 2016-01-26   | Yes         |                     5 |
| [TorScale2](https://atlas.torproject.org/#details/0ED52C42A7E9316F0CB8D4CA6BB9E14E9C5D599A)    | 2017-12-08   | No          |                     1 |
| [TorScale](https://atlas.torproject.org/#details/84E1D0F9D6B0E173D020DD673F9ECA26510CD706)     | 2017-11-29   | No          |                     5 |
| [torpulse](https://atlas.torproject.org/#details/9327368438ECD084FD08BF014C76E1754E35036B)     | 2016-08-26   | No          |                     5 |

## ContactInfo: AnonyMaid Team &lt;info@anonymaid.net&gt; (3) {#anonymaid-team-infoanonymaidnet}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [DutchDroid](https://atlas.torproject.org/#details/BF5068641A54A9433CA612BDFF7F098B72EB9762)  | 2017-08-09   | Yes         |                     1 |
| [DutchMaid04](https://atlas.torproject.org/#details/44182447E5E9F2997754CE53FFB4881942B5B3C6) | 2017-10-01   | No          |                     1 |
| [DutchMaid03](https://atlas.torproject.org/#details/7FAB8FED1A821455902BEA3388A6DA5BF6F78198) | 2017-10-01   | No          |                     1 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://atlas.torproject.org/#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://atlas.torproject.org/#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |

## ContactInfo: VSIF Support &lt;support AT vsif dot ca&gt; (5) {#vsif-support-support-at-vsif-dot-ca}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [VSIFweb](https://atlas.torproject.org/#details/78378DDD015C4E1C9242A5EC41158AF1E24CF43E)        | 2017-06-23   | Yes         |                     1 |
| [VSIFviking1](https://atlas.torproject.org/#details/1DEB985E3EEC0E7E0F6A887B417065E63522C5E2)    | 2017-06-15   | No          |                     4 |
| [VSIFenterprise](https://atlas.torproject.org/#details/59AE2B55941324B24354ADAAF971FC2C9F836963) | 2017-06-15   | No          |                     4 |
| [VSIFsalyut4](https://atlas.torproject.org/#details/D2461A903A754DEA625827AB333A2ECD06CE2E43)    | 2017-06-09   | No          |                     4 |
| [VSIFskylab](https://atlas.torproject.org/#details/F13B97699EF7328A6289E5C2540560903CBC79A8)     | 2017-06-04   | No          |                     4 |


## Fingerprint List of Guard-only Relays in E2E Groups

C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7,C238E705C538F5844B75DF1E082323387212C931,C4F69F1DF9D73E3E0046F3793081288DF5C66247,78378DDD015C4E1C9242A5EC41158AF1E24CF43E,157106182B9F33663CAEDCD883D302316331DE5E,BF5068641A54A9433CA612BDFF7F098B72EB9762,B756D7123D759EAB62CB6A09148AD65AC216F3E3,9F729DB3AE1ED73B19A846E217255CF017EEB2B5,BA66A1600751BF6BB39056A40FAD5831CC46AC56,B6904ADD4C0D10CDA7179E051962350A69A63243,8D13A1B5F11E79DCD3B2868215251769C8076AA1,88C3708A9D71ECEC1910B63C3FAA5BF60CD7E199