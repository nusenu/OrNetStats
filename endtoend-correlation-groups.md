---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-07-24 16:00 UTC**

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


## ContactInfo: emg88@duck.com (4) {#emg88duckcom}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [C0UNTCH0CULA4](https://metrics.torproject.org/rs.html#details/1299282E4D20AEFCB97089EC6724E785103E2205) | 2023-06-28   | Yes         |                     1 |
| [C0UNTCH0CULA2](https://metrics.torproject.org/rs.html#details/2C80EB18537317F2D712CE97484E0F052C9DBB3F) | 2023-03-31   | Yes         |                     3 |
| [C0UNTCH0CULA3](https://metrics.torproject.org/rs.html#details/98C2CCD293250286BC628235FA69C57646EAD780) | 2023-05-04   | Yes         |                     3 |
| [C0UNTCH0CULA5](https://metrics.torproject.org/rs.html#details/1192F0EC9316B1C97E815CCE77E49CFE105D41F5) | 2023-07-18   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

1299282E4D20AEFCB97089EC6724E785103E2205,2C80EB18537317F2D712CE97484E0F052C9DBB3F,98C2CCD293250286BC628235FA69C57646EAD780