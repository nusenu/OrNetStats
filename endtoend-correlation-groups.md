---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-01-21 20:00 UTC**

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


## ContactInfo: Hurdy-Gurdy &lt;admin AT my-mail dot rocks&gt; (6) {#hurdy-gurdy-admin-at-my-mail-dot-rocks}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [0x90](https://metrics.torproject.org/rs.html#details/EF25C1F9BEF8C4A3F2859493C7C8C5148725B4E7)       | 2021-09-07   | Yes         |                    11 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/42A955B09A4E327FBFB46A08F6E21705271CCA12) | 2021-08-21   | Yes         |                    11 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/0EC5AB1F97865D703014E845F39B7E9A4B28A6B1) | 2021-10-22   | Yes         |                     1 |
| [0x539](https://metrics.torproject.org/rs.html#details/CC61C2BE6689D36042FA0FB9E3F29E58854F50AB)      | 2021-11-20   | Yes         |                    11 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/233830F0A052F3845789607D1EC15457CF15F9AE) | 2021-11-15   | No          |                    11 |
| [0xdeadbeef](https://metrics.torproject.org/rs.html#details/D1B853ED27E4DFDCA3A54D3F2E269C4D94677F66) | 2018-04-16   | No          |                    11 |


## Fingerprint List of Guard-only Relays in E2E Groups

0EC5AB1F97865D703014E845F39B7E9A4B28A6B1,42A955B09A4E327FBFB46A08F6E21705271CCA12,CC61C2BE6689D36042FA0FB9E3F29E58854F50AB,EF25C1F9BEF8C4A3F2859493C7C8C5148725B4E7