---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-08-10 15:00 UTC**

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


## ContactInfo: Hurdy-Gurdy &lt;admin AT my-mail dot rocks&gt; (10) {#hurdy-gurdy-admin-at-my-mail-dot-rocks}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [0x90](https://metrics.torproject.org/rs.html#details/EF25C1F9BEF8C4A3F2859493C7C8C5148725B4E7)       | 2021-09-07   | Yes         |                    12 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/2717355D1ED1C421E3F8930F721BF2FDABA35CDA) | 2022-07-18   | Yes         |                    12 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/6C11461E189674B86A75EFE2A1E2B22713A46E8C) | 2022-01-14   | Yes         |                    12 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/42A955B09A4E327FBFB46A08F6E21705271CCA12) | 2021-08-21   | Yes         |                    12 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/37B8ECB953FC3C3E09722BFB8EEFD0334DDF4628) | 2022-01-14   | Yes         |                    12 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/8A530A9CE2EF8EA7D9E2B496566FD847E76C71E6) | 2022-01-07   | Yes         |                    12 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/0256CC7F76E46157F95705DAC58F0E3EF9CD1583) | 2022-01-31   | Yes         |                    12 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/233830F0A052F3845789607D1EC15457CF15F9AE) | 2021-11-15   | No          |                    12 |
| [0x539](https://metrics.torproject.org/rs.html#details/53A997230640C04C998A1DE3F5D3CD303C4481B0)      | 2022-08-10   | No          |                     1 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/D1B853ED27E4DFDCA3A54D3F2E269C4D94677F66) | 2018-04-16   | No          |                    12 |


## Fingerprint List of Guard-only Relays in E2E Groups

0256CC7F76E46157F95705DAC58F0E3EF9CD1583,2717355D1ED1C421E3F8930F721BF2FDABA35CDA,37B8ECB953FC3C3E09722BFB8EEFD0334DDF4628,42A955B09A4E327FBFB46A08F6E21705271CCA12,6C11461E189674B86A75EFE2A1E2B22713A46E8C,8A530A9CE2EF8EA7D9E2B496566FD847E76C71E6,EF25C1F9BEF8C4A3F2859493C7C8C5148725B4E7