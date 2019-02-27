---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2019-02-27 18:00 UTC**

For each operator the list of running relays is shown (relays are linked to [Relay Search](https://metrics.torproject.org/rs.html)).
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


## ContactInfo: tor-operator@your-emailaddress-domain (6) {#tor-operatoryour-emailaddress-domain}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [anotherRelay](https://metrics.torproject.org/rs.html#details/F6691E3EB7CAB3C876AAA885E6801B63DC998C39)   | 2018-10-29   | Yes         |                     1 |
| [DivisionBy1](https://metrics.torproject.org/rs.html#details/9879492B344126F899254E0F618F43D2B51F7505)    | 2018-11-08   | Yes         |                     1 |
| [DimasNiceRelay](https://metrics.torproject.org/rs.html#details/BE5CE67AAC8EC61551173844D874385996F4C439) | 2018-08-15   | Yes         |                     1 |
| [Marsu](https://metrics.torproject.org/rs.html#details/8750A946DD5AB24AE71A40B1BA7672034F24663F)          | 2018-12-23   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/9FC15C742C2E95A34F104CB5A0826C6659CFF2B7)    | 2018-06-20   | No          |                     1 |
| [SlurmExit](https://metrics.torproject.org/rs.html#details/C0BFC0A0341BD0293F093DEC6966B99038A31B79)      | 2018-11-24   | No          |                     1 |

## ContactInfo: Accessnow.org &lt;abuse .AT. accessnow .DOT. org&gt; (13) {#accessnoworg-abuse-at-accessnow-dot-org}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [AccessNow](https://metrics.torproject.org/rs.html#details/64299E6F2CF4E9F6CDDC72B999E89E6BE4FD4EC0)    | 2018-01-10   | Yes         |                     1 |
| [AccessNow007](https://metrics.torproject.org/rs.html#details/0516085D6CAC40ED4CDCEFDFC5CCF6B00DE61DED) | 2017-12-08   | No          |                    12 |
| [AccessNow003](https://metrics.torproject.org/rs.html#details/2DFDEA5DD415B95594BFB12D59FE841167F94B5F) | 2017-12-08   | No          |                    12 |
| [toritico01](https://metrics.torproject.org/rs.html#details/3A4D13F52A4C9A13AD60D94615D4C0B2F5F69E3C)   | 2019-02-13   | No          |                    12 |
| [AccessNow001](https://metrics.torproject.org/rs.html#details/3C5915348D731505C48112F4F03235FDE7B8C837) | 2017-12-08   | No          |                    12 |
| [AccessNow000](https://metrics.torproject.org/rs.html#details/4273E6D162ED2717A1CF4207A254004CD3F5307B) | 2017-12-05   | No          |                    12 |
| [AccessNow010](https://metrics.torproject.org/rs.html#details/46F90EF3A3628C134DBB4654D0E4FF7EB914B690) | 2017-12-08   | No          |                    12 |
| [AccessNow002](https://metrics.torproject.org/rs.html#details/6290A2D08E5EB89C809223C5C7BF52597690751D) | 2017-12-08   | No          |                    12 |
| [AccessNow006](https://metrics.torproject.org/rs.html#details/65E6EB676633328ADE3BD3168A59134CDDD21E19) | 2017-12-08   | No          |                    12 |
| [AccessNow008](https://metrics.torproject.org/rs.html#details/7E006A46A222CE42F84B4A175698B3B593A7B3B7) | 2017-12-08   | No          |                    12 |
| [AccessNow009](https://metrics.torproject.org/rs.html#details/8D093C9C2B42BC224A5319A660A6CF5EDEFE839F) | 2017-12-08   | No          |                    12 |
| [AccessNow005](https://metrics.torproject.org/rs.html#details/B0DD527BE01842D46030265FBD9928217A709F28) | 2017-12-08   | No          |                    12 |
| [AccessNow004](https://metrics.torproject.org/rs.html#details/D255268BACBB4562554CF20147731BDA0D8C452B) | 2017-12-08   | No          |                    12 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (2) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     1 |
| [Mercury](https://metrics.torproject.org/rs.html#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |

## ContactInfo: &lt;nobody AT example dot com&gt; (2) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |

## ContactInfo: Jelle Jansen &lt;tormail@gigawebs.net&gt; (3) {#jelle-jansen-tormailgigawebsnet}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [TVISION02](https://metrics.torproject.org/rs.html#details/52E018563FA31D13D6776E0897AF68AA3E21EA08) | 2019-01-09   | Yes         |                     2 |
| [TVISION04](https://metrics.torproject.org/rs.html#details/2E254E254A1FC66D6AD968E567B22F378C063026) | 2017-10-24   | Yes         |                     5 |
| [TVISION01](https://metrics.torproject.org/rs.html#details/8DAF2CAF4BFB0DD56B51955A17599A9FB0E933D3) | 2017-08-06   | No          |                     3 |


## Fingerprint List of Guard-only Relays in E2E Groups

2E254E254A1FC66D6AD968E567B22F378C063026,52E018563FA31D13D6776E0897AF68AA3E21EA08,64299E6F2CF4E9F6CDDC72B999E89E6BE4FD4EC0,8750A946DD5AB24AE71A40B1BA7672034F24663F,9879492B344126F899254E0F618F43D2B51F7505,A9A4213EA3D707857368C683F2208C83B8755D8A,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,BE5CE67AAC8EC61551173844D874385996F4C439,F6691E3EB7CAB3C876AAA885E6801B63DC998C39