---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-10-17 16:00 UTC**

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


## ContactInfo: Random Person nobody@tor.org (11) {#random-person-nobodytororg}

| Nickname                                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [pooclown](https://metrics.torproject.org/rs.html#details/F7BB03BC77CEB6EF66478C58A343028958EB7693)            | 2022-09-20   | Yes         |                     1 |
| [maddy](https://metrics.torproject.org/rs.html#details/E79404C7477110F73863BC5908F3F1C70990B685)               | 2022-10-08   | Yes         |                     1 |
| [ididnteditheconfig](https://metrics.torproject.org/rs.html#details/80F597A2715438BDD986E6F7AC8646EEA4E492F0)  | 2020-10-21   | Yes         |                     1 |
| [wehrhaftedemokratie](https://metrics.torproject.org/rs.html#details/60B6F3FAF65C4434F7A1F68216206BE807CE8075) | 2022-07-31   | Yes         |                     1 |
| [ididreadtheconfig](https://metrics.torproject.org/rs.html#details/F96CBFC5C079D839E01902802A70029486D2AD82)   | 2022-08-09   | Yes         |                     1 |
| [3303d3fe5c280f65](https://metrics.torproject.org/rs.html#details/1222A9B0071CD04E80C28D5A16F4BB74856067D3)    | 2022-10-16   | No          |                     1 |
| [ada97e41bada065b](https://metrics.torproject.org/rs.html#details/4739AC5558C54C9955D832CACB72814B2315AD32)    | 2022-10-16   | No          |                     1 |
| [e129fba5dc46c8f3](https://metrics.torproject.org/rs.html#details/6F928075B92C8CB151F94C56C87784A6BFA07A93)    | 2022-10-16   | No          |                     1 |
| [169fc1786a2ff861](https://metrics.torproject.org/rs.html#details/96DD805CB253A0C469927290680B8F14AA6FE273)    | 2022-10-16   | No          |                     1 |
| [c7650d47136f596e](https://metrics.torproject.org/rs.html#details/B54459C05D8FEF67E31B4817ECC2178C8296EA27)    | 2022-10-16   | No          |                     1 |
| [theglowingones](https://metrics.torproject.org/rs.html#details/E399BF6C6EEB4D63A388911B84C16909CD84A13E)      | 2022-10-13   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

60B6F3FAF65C4434F7A1F68216206BE807CE8075,80F597A2715438BDD986E6F7AC8646EEA4E492F0,9B44CAE280BDDC8B79999427FFA459A2EC2E9EB2,E79404C7477110F73863BC5908F3F1C70990B685,F7BB03BC77CEB6EF66478C58A343028958EB7693,F96CBFC5C079D839E01902802A70029486D2AD82