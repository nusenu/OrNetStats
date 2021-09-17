---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-09-17 12:00 UTC**

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


## ContactInfo: 4punk7 AT mailbox dot org (5) {#4punk7-at-mailbox-dot-org}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [4punk7r2](https://metrics.torproject.org/rs.html#details/CB2DBDB2D9422D57AD85148EF9511AF4CE4D6052) | 2020-04-04   | Yes         |                     1 |
| [4punk7r1](https://metrics.torproject.org/rs.html#details/ABA31795BAD2AB8097F3AD0FE1A920E518D3D3F3) | 2020-04-02   | Yes         |                     1 |
| [4punk7e1](https://metrics.torproject.org/rs.html#details/2E0C69E59B5B6AA15BB1C269690722607663416C) | 2020-11-27   | No          |                     1 |
| [4punk7e2](https://metrics.torproject.org/rs.html#details/68057FD302B0F83C0ED00B6D70FDAD6BEEF2005B) | 2020-10-21   | No          |                     1 |
| [4punk7e3](https://metrics.torproject.org/rs.html#details/F42FF0E095F23AD253622272F984649DDEEB402C) | 2020-10-26   | No          |                     1 |

## ContactInfo: torix aT=== protonmail&lt;dOT &gt;com (10) {#torixatprotonmaildotcom}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Aramis67](https://metrics.torproject.org/rs.html#details/53C9F4954E7A7332BB0C610C5B8E04CA065AF29B) | 2019-05-13   | Yes         |                    10 |
| [Aramis72](https://metrics.torproject.org/rs.html#details/F5FD7EF4307F8C5C398147877F32A9F9F71E2092) | 2020-05-27   | Yes         |                    10 |
| [Aramis66](https://metrics.torproject.org/rs.html#details/39A18F31B312E5CB211781090766934C1CFDAB36) | 2020-07-10   | Yes         |                    10 |
| [Aramis75](https://metrics.torproject.org/rs.html#details/4D2A4831BB67853A6FA01517A61B810D4480AE2F) | 2020-10-30   | No          |                    10 |
| [Aramis](https://metrics.torproject.org/rs.html#details/4F9EFCF7689084E4C8EE993E123E32B75368804C)   | 2021-08-22   | No          |                    10 |
| [Aramis73](https://metrics.torproject.org/rs.html#details/5FCB4186E2BCD4E8E510EACEC7AABE2194CA36BC) | 2020-10-30   | No          |                    10 |
| [Aramis71](https://metrics.torproject.org/rs.html#details/AB32B2EA350C10888144A7ECCA7FFACA844C2052) | 2020-04-27   | No          |                    10 |
| [Aramis74](https://metrics.torproject.org/rs.html#details/ABA0BAE51160B9DE6C030E070F7EB3D9D605EE7E) | 2021-09-13   | No          |                     1 |
| [Aramis](https://metrics.torproject.org/rs.html#details/D3F6616034448DEEE369782C96F84FE1407E4200)   | 2021-08-22   | No          |                    10 |
| [Aramis70](https://metrics.torproject.org/rs.html#details/DEAA89B5B8D9CEAD5CE0F9281D482A4EACC30592) | 2020-05-02   | No          |                    10 |


## Fingerprint List of Guard-only Relays in E2E Groups

39A18F31B312E5CB211781090766934C1CFDAB36,53C9F4954E7A7332BB0C610C5B8E04CA065AF29B,ABA31795BAD2AB8097F3AD0FE1A920E518D3D3F3,CB2DBDB2D9422D57AD85148EF9511AF4CE4D6052,F5FD7EF4307F8C5C398147877F32A9F9F71E2092