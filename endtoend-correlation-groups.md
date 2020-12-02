---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-12-02 16:00 UTC**

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


## ContactInfo: abuse at yggdrasil dot ws (7) {#abuseatyggdrasildotws}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [BKA](https://metrics.torproject.org/rs.html#details/DA580E4EB2A453298D40F73ECFC78E896B001182)      | 2020-10-07   | Yes         |                     7 |
| [Ragnarok](https://metrics.torproject.org/rs.html#details/02930FFEB87968D518101EB79202F1C3766078DA) | 2020-02-11   | No          |                     8 |
| [Loki](https://metrics.torproject.org/rs.html#details/0ADAC68F29875A1366F06762F2B305B0BFD11364)     | 2020-12-02   | No          |                     1 |
| [Ymir](https://metrics.torproject.org/rs.html#details/4AA0035604DF40E5BA20DBE88EF6D11432421BFA)     | 2020-10-27   | No          |                     7 |
| [Ganymed](https://metrics.torproject.org/rs.html#details/5AFF7583F5ED62A274823C83199F2E19083692EC)  | 2020-08-20   | No          |                     8 |
| [Freya](https://metrics.torproject.org/rs.html#details/85ED839A03D10C46219609625D7FEAE59EDCCFDD)    | 2020-05-27   | No          |                     7 |
| [Kallisto](https://metrics.torproject.org/rs.html#details/D4C5BAEA92CADCC02D64E0DD9F1A49024C57F05C) | 2020-09-11   | No          |                     7 |


## Fingerprint List of Guard-only Relays in E2E Groups

DA580E4EB2A453298D40F73ECFC78E896B001182