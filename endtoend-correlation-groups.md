---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-12-11 15:00 UTC**

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


## ContactInfo: abuse@torexit.in (5) {#abusetorexitin}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [BerndPommes](https://metrics.torproject.org/rs.html#details/E695F831BE527A96682A652970AD05BACF28665B) | 2023-06-15   | Yes         |                     4 |
| [OBFS](https://metrics.torproject.org/rs.html#details/F92539C0DD7B315E4CCA3ECF33C4A06304A783EB)        | 2023-09-27   | Yes         |                     1 |
| [AlexPommes](https://metrics.torproject.org/rs.html#details/7C73B2E52AAFAEEE11BAA4379D6CF09899EC0E1F)  | 2023-06-15   | No          |                     4 |
| [DerPommes](https://metrics.torproject.org/rs.html#details/87BB4F7F894090A2084A9C3E3CD40792C342FA32)   | 2023-01-04   | No          |                     4 |
| [pommes](https://metrics.torproject.org/rs.html#details/92FEA999E7EF9C39CD8A18D87E21824D0C97B97C)      | 2022-12-30   | No          |                     4 |


## Fingerprint List of Guard-only Relays in E2E Groups

E695F831BE527A96682A652970AD05BACF28665B,F92539C0DD7B315E4CCA3ECF33C4A06304A783EB