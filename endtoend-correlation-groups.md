---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-07-06 17:00 UTC**

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


## ContactInfo: 0xDAC4CCB6722FF7E5 Alexander Bu00F6hm &lt;alexander. (2) {#0xdac4ccb6722ff7e5-alexander-bu00f6hm-alexander}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [hera](https://metrics.torproject.org/rs.html#details/C07DCA0B231BE0554AB4D574AC057C7572BD6EF0)           | 2022-06-25   | Yes         |                     1 |
| [freestyle0ffle](https://metrics.torproject.org/rs.html#details/7AA19F3B1AA8146A1839675E1844D51FE9B3FD3B) | 2022-07-02   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

C07DCA0B231BE0554AB4D574AC057C7572BD6EF0