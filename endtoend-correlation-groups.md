---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-12-08 17:00 UTC**

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


## ContactInfo: potlatch protonmail com (8) {#potlatch-protonmail-com}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [TorExitAlbania](https://metrics.torproject.org/rs.html#details/373BF7A2CD16E86D4C5BEC591A41945C9AED392D)  | 2020-07-14   | Yes         |                    10 |
| [TorExitAlbania2](https://metrics.torproject.org/rs.html#details/D78D1B4489CF4FFB0FD74014BDF2D600D8EE5B05) | 2020-06-13   | Yes         |                    10 |
| [TorExitBulgaria](https://metrics.torproject.org/rs.html#details/961B9D86125A08FAA9F7E742B228307EF7E2E082) | 2021-06-30   | Yes         |                    10 |
| [TorExitLatvia](https://metrics.torproject.org/rs.html#details/08CD9D4224058DC97A1F27679A5BEE5724C4C6EC)   | 2020-08-15   | Yes         |                    10 |
| [TorExitMoldova](https://metrics.torproject.org/rs.html#details/742C45F2D9004AADE0077E528A4418A6A81BC2BA)  | 2019-01-01   | No          |                    11 |
| [TorExitFinland](https://metrics.torproject.org/rs.html#details/9B31F1F1C1554F9FFB3455911F82E818EF7C7883)  | 2015-12-31   | No          |                    10 |
| [TorExitMoldova](https://metrics.torproject.org/rs.html#details/B06F093A3D4DFAD3E923F4F28A74901BD4F74EB1)  | 2017-05-24   | No          |                    10 |
| [TorExitCz](https://metrics.torproject.org/rs.html#details/FFEA37B6DA76C458D3E35476DD7D1FD0A98AE731)       | 2021-12-07   | No          |                     2 |


## Fingerprint List of Guard-only Relays in E2E Groups

08CD9D4224058DC97A1F27679A5BEE5724C4C6EC,373BF7A2CD16E86D4C5BEC591A41945C9AED392D,961B9D86125A08FAA9F7E742B228307EF7E2E082,D78D1B4489CF4FFB0FD74014BDF2D600D8EE5B05