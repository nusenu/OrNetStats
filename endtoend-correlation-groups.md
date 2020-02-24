---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-02-24 18:00 UTC**

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


## ContactInfo: tor-abuse&lt;at&gt;mailbox&lt;dot&gt;org (4) {#tor-abuseatmailboxdotorg}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [AlanTuring](https://metrics.torproject.org/rs.html#details/2BB85DC5BD3C6F0D81A4F2B5882176C6BF7ECF5A) | 2019-12-17   | Yes         |                     3 |
| [goodwill](https://metrics.torproject.org/rs.html#details/0CF21302931A8B4C67B4DFB03DBEA7BD4AA1E647)   | 2020-02-24   | No          |                     1 |
| [torturing](https://metrics.torproject.org/rs.html#details/6F647831035CDB891B33103A073AEB9028122129)  | 2019-02-13   | No          |                     3 |
| [Nicenstein](https://metrics.torproject.org/rs.html#details/7614EF326635DA810638E2F5D449D10AE2BB7158) | 2020-02-19   | No          |                     3 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (2) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4) | 2019-10-25   | Yes         |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/71840F45C2478347B872321066F9805D1A1B79FD)  | 2019-10-25   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

2BB85DC5BD3C6F0D81A4F2B5882176C6BF7ECF5A,DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4