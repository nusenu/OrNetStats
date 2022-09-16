---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-09-16 15:00 UTC**

For each operator the list of running relays is shown (relays are linked to [Relay Search](https://metrics.torproject.org/rs.html)).
Operators and relays are sorted from more relevant to less relevant. More relevant in terms of guard probability.
Guardonly relays have the guard flag but not the exit flag.
Since exits are less common than guards their guard probability is usually 0% even when they have the guard flag.
The number next to the contactinfo shows the number of relays running with the given ContactInfo (excluding middle-only relays).
Middle-only relays (no guard and exit flag) are excluded to reduce the size of this list.

At the end of this page you can find a comma separated list of fingerprints of all guard-only relays on this page.

## If your relay is listed here
Please configure MyFamily in your torrc configuration files.
This page should help you with debugging your MyFamily configuration. The number in the last column should equal to the number of
relays you operate (for every relay).

Once MyFamily is fixed the relays will automatically disappear from this page (within ~1-2 days).
If you need help with the MyFamily configuration you can reach out to the
[tor-relays mailing list](https://lists.torproject.org/cgi-bin/mailman/listinfo/tor-relays).
You can also use tools that handle MyFamily automatically (I maintain an ansible role - 
[relayor](https://medium.com/@nusenu/deploying-tor-relays-with-ansible-6612593fa34d))
If someone else is using your contactInfo please send an email to ```bad-relays AT lists DOT torproject DOT org```.


## ContactInfo: your@e-mail (6) {#youre-mail}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [AMSRelay](https://metrics.torproject.org/rs.html#details/A9DA735C9DE7C891B9EDD6B433B458F7687E829B)    | 2022-08-29   | Yes         |                     1 |
| [CoolRelay](https://metrics.torproject.org/rs.html#details/D594BC4244636CC342973B594B707685DCAA0C87)   | 2022-07-11   | Yes         |                     1 |
| [BlackMesaAG](https://metrics.torproject.org/rs.html#details/14693074C2325CEC8746AFBB85291E749AC45D5D) | 2021-12-29   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/21524A2BC6C4275B2FDC23F0FF2344B6D8FEC255) | 2022-08-18   | Yes         |                     1 |
| [koaxedrelay](https://metrics.torproject.org/rs.html#details/5788F2CD0808CC2BB3F3679DC4BB40FCDB0C152C) | 2022-03-01   | Yes         |                     1 |
| [0d210s](https://metrics.torproject.org/rs.html#details/D2B845D50ED5B49A8B8B425AB530C38D952E5C3C)      | 2022-09-08   | No          |                     1 |

## ContactInfo: Brandon Kuschel &lt;kusch023 AT NOSPAM umn dot edu&gt; (6) {#brandon-kuschel-kusch023-at-nospam-umn-dot-edu}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Lamia](https://metrics.torproject.org/rs.html#details/C46548D44C0CA5855C175CE26F5817D38F833C9F)      | 2022-08-21   | Yes         |                     6 |
| [Echidna](https://metrics.torproject.org/rs.html#details/BA57222A0EC9ECDF003AED665DFB0B1287EA039D)    | 2022-08-21   | Yes         |                     6 |
| [Polyphemus](https://metrics.torproject.org/rs.html#details/0CABED9159F1E4BE82879F5A34ED8D7349E931BD) | 2022-09-14   | No          |                     5 |
| [Chimera](https://metrics.torproject.org/rs.html#details/2946159CF9D8EAEB8C4A27F6A54B01A459DEE164)    | 2022-08-21   | No          |                     5 |
| [Minotaur](https://metrics.torproject.org/rs.html#details/8BDBE498180C41249D3230FC5092CB3EB5A62482)   | 2021-04-06   | No          |                     6 |
| [Charybdis](https://metrics.torproject.org/rs.html#details/CBF59EC5B9FD108092AE9149EFDAE41F882DA669)  | 2022-08-19   | No          |                     6 |


## Fingerprint List of Guard-only Relays in E2E Groups

14693074C2325CEC8746AFBB85291E749AC45D5D,21524A2BC6C4275B2FDC23F0FF2344B6D8FEC255,5788F2CD0808CC2BB3F3679DC4BB40FCDB0C152C,A9DA735C9DE7C891B9EDD6B433B458F7687E829B,D594BC4244636CC342973B594B707685DCAA0C87,BA57222A0EC9ECDF003AED665DFB0B1287EA039D,C46548D44C0CA5855C175CE26F5817D38F833C9F