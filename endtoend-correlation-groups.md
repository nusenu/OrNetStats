---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-12-07 20:00 UTC**

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
If someone else is using your contactInfo please send an email to ```bad-relays AT lists DOT torproject DOT org```.


## ContactInfo: s013350 6 @gmai l .com (2) {#s0133506gmailcom}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [torrelayepsom](https://metrics.torproject.org/rs.html#details/98518F74702216049283335998B66DC66404C040)   | 2021-10-14   | Yes         |                     1 |
| [pstorrelayepsom](https://metrics.torproject.org/rs.html#details/C9BA228C967E7231CD0B47C49E88BC50A7400584) | 2021-10-29   | No          |                     1 |

## ContactInfo: torix aT=== protonmail&lt;dOT &gt;com (7) {#torixatprotonmaildotcom}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Aramis67](https://metrics.torproject.org/rs.html#details/53C9F4954E7A7332BB0C610C5B8E04CA065AF29B) | 2019-05-13   | Yes         |                     1 |
| [Aramis](https://metrics.torproject.org/rs.html#details/2B3AAC97B269D59E6D642C8BFB174EDD13741C38)   | 2021-11-12   | No          |                     2 |
| [Aramis](https://metrics.torproject.org/rs.html#details/4F9EFCF7689084E4C8EE993E123E32B75368804C)   | 2021-08-22   | No          |                     2 |
| [Aramis71](https://metrics.torproject.org/rs.html#details/AB32B2EA350C10888144A7ECCA7FFACA844C2052) | 2020-04-27   | No          |                     4 |
| [Aramis](https://metrics.torproject.org/rs.html#details/D3F6616034448DEEE369782C96F84FE1407E4200)   | 2021-08-22   | No          |                     2 |
| [Aramis70](https://metrics.torproject.org/rs.html#details/DEAA89B5B8D9CEAD5CE0F9281D482A4EACC30592) | 2020-05-02   | No          |                     4 |
| [Aramis](https://metrics.torproject.org/rs.html#details/F314580EA22CB3DCB135D64E92108BFB8FD209AF)   | 2021-11-12   | No          |                     2 |


## Fingerprint List of Guard-only Relays in E2E Groups

98518F74702216049283335998B66DC66404C040,53C9F4954E7A7332BB0C610C5B8E04CA065AF29B