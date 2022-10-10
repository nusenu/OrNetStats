---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-10-10 19:00 UTC**

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


## ContactInfo: tor at reichsfunkma dot st (4) {#tor-at-reichsfunkma-dot-st}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Reichsfunkmast6](https://metrics.torproject.org/rs.html#details/3B42ABB5E5338BD98BDB44918581379107B54AEF) | 2022-09-23   | Yes         |                     8 |
| [Reichsfunkmast7](https://metrics.torproject.org/rs.html#details/73DA3211EF6B5F427E5014FBF926B151AFBD9C91) | 2022-10-10   | No          |                     1 |
| [Reichsfunkmast3](https://metrics.torproject.org/rs.html#details/99A6EDEC44F733ACAF2539B353118F36D27322E3) | 2022-09-20   | No          |                     8 |
| [Reichsfunkmast8](https://metrics.torproject.org/rs.html#details/E8B477C17E9FC1A535BBC2468957F7B9282A783A) | 2022-09-30   | No          |                     7 |


## Fingerprint List of Guard-only Relays in E2E Groups

3B42ABB5E5338BD98BDB44918581379107B54AEF