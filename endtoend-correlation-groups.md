---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-01-07 15:00 UTC**

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


## ContactInfo: Random Person (3) {#random-person}

| Nickname                                                                                                     | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [onionfarm](https://metrics.torproject.org/rs.html#details/922835625922416F0198AF0B3E6F832B3B1E24D8)         | 2021-04-12   | Yes         |                     1 |
| [iDidEditTheConfig](https://metrics.torproject.org/rs.html#details/56E9882FC7B62C4F2A951C5E2D570D6E74F15C6D) | 2021-10-26   | Yes         |                     1 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/E714A55C2CD59FD24DC1C755B977FD0320632823)           | 2022-01-04   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

56E9882FC7B62C4F2A951C5E2D570D6E74F15C6D,922835625922416F0198AF0B3E6F832B3B1E24D8