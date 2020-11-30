---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-11-30 17:00 UTC**

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


## ContactInfo: Privex Inc. https://www.privex.io (3) {#privex-inc-httpswwwprivexio}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [privexrelayde1](https://metrics.torproject.org/rs.html#details/C64EB4553AA308D8FBC314D73B44178E4CB11C35)  | 2020-11-22   | Yes         |                     2 |
| [privexrelayfin1](https://metrics.torproject.org/rs.html#details/C3ACB0492A644E27A549BC3CDF3B7A129186E3BF) | 2018-09-27   | Yes         |                     3 |
| [privexse1exit](https://metrics.torproject.org/rs.html#details/D8A1F5A8EA1AF53E3414B9C48FE6B10C31ACC9B2)   | 2019-06-26   | No          |                     2 |


## Fingerprint List of Guard-only Relays in E2E Groups

C3ACB0492A644E27A549BC3CDF3B7A129186E3BF,C64EB4553AA308D8FBC314D73B44178E4CB11C35