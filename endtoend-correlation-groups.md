---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-07-10 13:00 UTC**

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


## ContactInfo: info@fileditch.com (4) {#infofileditchcom}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [FileDitchRelay0](https://metrics.torproject.org/rs.html#details/1D58C94057CFA3A875208BD699B2CA262E7C7C1C) | 2022-07-01   | Yes         |                     3 |
| [FileDitchExit1](https://metrics.torproject.org/rs.html#details/667741676DD35F168C1858232928AA26564A2EC6)  | 2022-07-07   | No          |                     1 |
| [FileDitchExit2](https://metrics.torproject.org/rs.html#details/C92DE921C34ACB1C1B4EA7D2C1ECF4A0ACD2CA00)  | 2022-06-09   | No          |                     3 |
| [FileDitchExit0](https://metrics.torproject.org/rs.html#details/ED13907E3BD2901D6DFB2036805640EA3A33D97A)  | 2022-06-09   | No          |                     3 |


## Fingerprint List of Guard-only Relays in E2E Groups

1D58C94057CFA3A875208BD699B2CA262E7C7C1C