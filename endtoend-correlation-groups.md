---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-02-15 18:00 UTC**

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


## ContactInfo: tor at xtom dot com (6) {#toratxtomdotcom}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [XTOMAMS](https://metrics.torproject.org/rs.html#details/A41A8317A5BD4DD10BE9925277DB332395F50F17)     | 2021-12-07   | Yes         |                     1 |
| [XTOMLON](https://metrics.torproject.org/rs.html#details/5ABC7AAFA86CA890242DE79582125B18C3B0E541)     | 2021-12-03   | Yes         |                     1 |
| [XTOMDUS](https://metrics.torproject.org/rs.html#details/955F15325D6F3E3350EA8A70EB5C49C5BF95C5A0)     | 2021-12-03   | Yes         |                     1 |
| [XTOMFRA](https://metrics.torproject.org/rs.html#details/AB12F88E52C439769EDB592B89AA36D8AF5A1C0C)     | 2021-12-07   | Yes         |                     1 |
| [XTOMSJC](https://metrics.torproject.org/rs.html#details/280F26E75C5ED7C292DD5AC5A9695C47B7784DC8)     | 2021-12-09   | Yes         |                     1 |
| [XTOMLONEXIT](https://metrics.torproject.org/rs.html#details/9331E29298E40EB28A01C780E73954CD73237F50) | 2022-02-03   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

280F26E75C5ED7C292DD5AC5A9695C47B7784DC8,5ABC7AAFA86CA890242DE79582125B18C3B0E541,955F15325D6F3E3350EA8A70EB5C49C5BF95C5A0,A41A8317A5BD4DD10BE9925277DB332395F50F17,AB12F88E52C439769EDB592B89AA36D8AF5A1C0C