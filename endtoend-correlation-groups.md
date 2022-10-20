---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-10-20 15:00 UTC**

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


## ContactInfo: your@e-mail (4) {#youre-mail}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CoolRelay](https://metrics.torproject.org/rs.html#details/D594BC4244636CC342973B594B707685DCAA0C87) | 2022-07-11   | Yes         |                     1 |
| [myRelay](https://metrics.torproject.org/rs.html#details/0CABC7987695482274734502CBB8E4AB550C1141)   | 2022-10-11   | Yes         |                     1 |
| [AMSRelay](https://metrics.torproject.org/rs.html#details/A9DA735C9DE7C891B9EDD6B433B458F7687E829B)  | 2022-08-29   | Yes         |                     1 |
| [newRelay](https://metrics.torproject.org/rs.html#details/9DEDA0B85B2388BE592B64598EA92414EB3E8D3B)  | 2022-10-14   | No          |                     1 |

## ContactInfo: Random Person nobody@tor.org (8) {#random-person-nobodytororg}

| Nickname                                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [imherefortheparty](https://metrics.torproject.org/rs.html#details/3540A4DD39DCF318842B295CDDD49118924F2A57)   | 2022-04-08   | Yes         |                     1 |
| [maddy](https://metrics.torproject.org/rs.html#details/E79404C7477110F73863BC5908F3F1C70990B685)               | 2022-10-08   | Yes         |                     1 |
| [pooclown](https://metrics.torproject.org/rs.html#details/F7BB03BC77CEB6EF66478C58A343028958EB7693)            | 2022-09-20   | Yes         |                     1 |
| [ididnteditheconfig](https://metrics.torproject.org/rs.html#details/80F597A2715438BDD986E6F7AC8646EEA4E492F0)  | 2020-10-21   | Yes         |                     1 |
| [wehrhaftedemokratie](https://metrics.torproject.org/rs.html#details/60B6F3FAF65C4434F7A1F68216206BE807CE8075) | 2022-07-31   | Yes         |                     1 |
| [ididreadtheconfig](https://metrics.torproject.org/rs.html#details/F96CBFC5C079D839E01902802A70029486D2AD82)   | 2022-08-09   | Yes         |                     1 |
| [ididnteditheconfig](https://metrics.torproject.org/rs.html#details/5EA46A3C23E4A3905DAAE9BD4801142E20AEA780)  | 2022-10-05   | No          |                     1 |
| [theglowingones](https://metrics.torproject.org/rs.html#details/E399BF6C6EEB4D63A388911B84C16909CD84A13E)      | 2022-10-13   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

0CABC7987695482274734502CBB8E4AB550C1141,A9DA735C9DE7C891B9EDD6B433B458F7687E829B,D594BC4244636CC342973B594B707685DCAA0C87,3540A4DD39DCF318842B295CDDD49118924F2A57,60B6F3FAF65C4434F7A1F68216206BE807CE8075,80F597A2715438BDD986E6F7AC8646EEA4E492F0,E79404C7477110F73863BC5908F3F1C70990B685,F7BB03BC77CEB6EF66478C58A343028958EB7693,F96CBFC5C079D839E01902802A70029486D2AD82