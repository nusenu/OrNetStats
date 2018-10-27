---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-10-27 07:00 UTC**

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


## ContactInfo: tor-operator@your-emailaddress-domain (5) {#tor-operatoryour-emailaddress-domain}

| Nickname                                                                                                     | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [HOLARELAY](https://metrics.torproject.org/rs.html#details/B2DA2FA9EABEF4138C8CE549D09C44B82550A2BB)         | 2018-09-25   | Yes         |                     1 |
| [DimasNiceRelay2nd](https://metrics.torproject.org/rs.html#details/10901213FFAB09B5085131D57311563424CF2DBD) | 2018-09-25   | Yes         |                     1 |
| [DimasNiceRelay](https://metrics.torproject.org/rs.html#details/BE5CE67AAC8EC61551173844D874385996F4C439)    | 2018-08-15   | Yes         |                     1 |
| [jgautRelay](https://metrics.torproject.org/rs.html#details/21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA)        | 2018-08-17   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/9FC15C742C2E95A34F104CB5A0826C6659CFF2B7)       | 2018-06-20   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://metrics.torproject.org/rs.html#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: &lt;nobody AT example dot com&gt; (2) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/CD7B3EFFB0BEE35A57A3AE7646DFBCD9B0BD9E76)   | 2018-05-21   | No          |                     1 |

## ContactInfo: tor@sechsnulldrei.org (4) {#torsechsnulldreiorg}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [ephesysein](https://metrics.torproject.org/rs.html#details/785934EF33E67C1322CE783338778C1A4E5532CD)  | 2018-10-10   | Yes         |                     2 |
| [ephesysein](https://metrics.torproject.org/rs.html#details/343384832FF3056C27714526101BA95B81DE3767)  | 2018-10-09   | Yes         |                     2 |
| [ephesysnull](https://metrics.torproject.org/rs.html#details/051F744E4E5CDBBAC14C1BC33F928F1B1FC24C1D) | 2018-10-19   | No          |                     2 |
| [ephesysnull](https://metrics.torproject.org/rs.html#details/675B01ACB6D2875AFC81B34B2C4A0B68EE174291) | 2018-10-19   | No          |                     2 |


## Fingerprint List of Guard-only Relays in E2E Groups

10901213FFAB09B5085131D57311563424CF2DBD,21EB9AC554EA44FA6AB564B4D1CC9E445D88FECA,343384832FF3056C27714526101BA95B81DE3767,785934EF33E67C1322CE783338778C1A4E5532CD,A9A4213EA3D707857368C683F2208C83B8755D8A,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,B2DA2FA9EABEF4138C8CE549D09C44B82550A2BB,BE5CE67AAC8EC61551173844D874385996F4C439