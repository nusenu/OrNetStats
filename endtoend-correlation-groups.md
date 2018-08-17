---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-08-17 07:00 UTC**

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


## ContactInfo: Random Person &lt;periplanetaamericanus AT gmail dot (11) {#random-person-periplanetaamericanus-at-gmail-dot-}

| Nickname                                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Priya1](https://metrics.torproject.org/rs.html#details/0337174B5BC470FBCAEF715FE8E89162FB75B2FB)              | 2018-06-21   | Yes         |                     7 |
| [Layla8](https://metrics.torproject.org/rs.html#details/7D4838AB4D937795306135418D8D5E07A93E3836)              | 2018-06-20   | Yes         |                     5 |
| [yetstillmoretshirts](https://metrics.torproject.org/rs.html#details/4B7B1260325E36820030C7E61AC3273CADEC2DB8) | 2018-06-23   | Yes         |                     7 |
| [Layla9](https://metrics.torproject.org/rs.html#details/5B7C417927B2C7C0A8F7C8669876746B95D11693)              | 2018-07-14   | Yes         |                     2 |
| [Layla2](https://metrics.torproject.org/rs.html#details/7D01B2CD3095EAAF69639B8F6AED0463B7262975)              | 2018-08-09   | Yes         |                     1 |
| [moretshirts](https://metrics.torproject.org/rs.html#details/D7F13CC027BBD37DC706CF7B27C07716CF88440B)         | 2018-06-21   | Yes         |                     7 |
| [Abbey2](https://metrics.torproject.org/rs.html#details/C546FD12702A9539D1F50B87C7AAC9A983B2C00F)              | 2018-08-06   | Yes         |                     1 |
| [Abbey1](https://metrics.torproject.org/rs.html#details/BEF0D05BEE9CB62989B78125EAEFFFE97241373D)              | 2018-07-20   | Yes         |                     1 |
| [Layla3](https://metrics.torproject.org/rs.html#details/B910D70B1ADADED099283C3F895D53638027DD1D)              | 2018-06-27   | Yes         |                     5 |
| [evenmoretshirts](https://metrics.torproject.org/rs.html#details/CA8C21E0082046BA4894CD625E4E27DFE8544B92)     | 2018-06-22   | Yes         |                     7 |
| [torrobert1](https://metrics.torproject.org/rs.html#details/FF79CA5A50970E21E9AB320CE62C2178E963970C)          | 2018-08-11   | No          |                     1 |

## ContactInfo: VSIF Support &lt;support AT vsif dot ca&gt; (7) {#vsif-support-support-at-vsif-dot-ca}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [VSIFweb](https://metrics.torproject.org/rs.html#details/78378DDD015C4E1C9242A5EC41158AF1E24CF43E)        | 2017-06-23   | Yes         |                     5 |
| [VSIFviking1](https://metrics.torproject.org/rs.html#details/1DEB985E3EEC0E7E0F6A887B417065E63522C5E2)    | 2017-06-15   | No          |                     7 |
| [VSIFenterprise](https://metrics.torproject.org/rs.html#details/59AE2B55941324B24354ADAAF971FC2C9F836963) | 2017-06-15   | No          |                     7 |
| [VSIFsalyut4](https://metrics.torproject.org/rs.html#details/D2461A903A754DEA625827AB333A2ECD06CE2E43)    | 2017-06-09   | No          |                     7 |
| [VSIFcopernicus](https://metrics.torproject.org/rs.html#details/D509A7A321FF9660665B75CB19F0FF09964C0B80) | 2018-02-11   | No          |                     6 |
| [VSIFvoyager](https://metrics.torproject.org/rs.html#details/E1DDAE70F14B9A6A7C01BDB9BDCCB70307BEE90A)    | 2018-02-11   | No          |                     6 |
| [VSIFskylab](https://metrics.torproject.org/rs.html#details/F13B97699EF7328A6289E5C2540560903CBC79A8)     | 2017-06-04   | No          |                     7 |


## Fingerprint List of Guard-only Relays in E2E Groups

0337174B5BC470FBCAEF715FE8E89162FB75B2FB,4B7B1260325E36820030C7E61AC3273CADEC2DB8,5B7C417927B2C7C0A8F7C8669876746B95D11693,78378DDD015C4E1C9242A5EC41158AF1E24CF43E,7D01B2CD3095EAAF69639B8F6AED0463B7262975,7D4838AB4D937795306135418D8D5E07A93E3836,B910D70B1ADADED099283C3F895D53638027DD1D,BEF0D05BEE9CB62989B78125EAEFFFE97241373D,C546FD12702A9539D1F50B87C7AAC9A983B2C00F,CA8C21E0082046BA4894CD625E4E27DFE8544B92,D7F13CC027BBD37DC706CF7B27C07716CF88440B