---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-05-28 16:00 UTC**

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


## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; (6) {#neel-chauhan-neel-at-neelc-dot-org}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelayA](https://metrics.torproject.org/rs.html#details/B0F9BA27944FA59E3B1A182208FF7C0CFF5497B2) | 2020-06-14   | Yes         |                     4 |
| [NeelTorRelayB](https://metrics.torproject.org/rs.html#details/DB710B14D7329B7289CFCC547F48EF53F812C40D) | 2020-06-14   | Yes         |                     4 |
| [NeelTorExitA](https://metrics.torproject.org/rs.html#details/035485A94591505E17683D2A350318DE2C384BAA)  | 2020-12-24   | No          |                     6 |
| [NeelTorExitC](https://metrics.torproject.org/rs.html#details/9B49F7C1B0B73988CE01091E963740117DA6D20D)  | 2021-02-03   | No          |                     4 |
| [NeelTorExitD](https://metrics.torproject.org/rs.html#details/B1F9BDD70BC91BFBC9061918C902F40E04E066B2)  | 2021-02-03   | No          |                     4 |
| [NeelTorExitB](https://metrics.torproject.org/rs.html#details/FDE5D296791B47BC99FF7107B188A458C02832FC)  | 2020-12-24   | No          |                     6 |


## Fingerprint List of Guard-only Relays in E2E Groups

B0F9BA27944FA59E3B1A182208FF7C0CFF5497B2,DB710B14D7329B7289CFCC547F48EF53F812C40D