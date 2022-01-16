---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-01-16 11:00 UTC**

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


## ContactInfo: shebangs@yopmail.fr (8) {#shebangsyopmailfr}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Shebangs](https://metrics.torproject.org/rs.html#details/E4A8BC82E660528D5B0B8D36C08AB44B77351736) | 2020-12-17   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/328ED3A92D1CD621659B4DA6E210FCAED813174B) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/A4A79E2B8294AA2572B46C5C772E149F84FAF763) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/3688001D75469101F74A5D551A49B0EF410F0E26) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/D8CE67E09B3E0B0D5A5CBF3AA0C702B804D5B7C8) | 2021-12-29   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/4918A461CEE1C8E65F4272E40CF3C6C6E70BB22C) | 2021-02-04   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/AC87DB1D965362FBCB9FC8BA32986718D3EC6AB6) | 2020-12-21   | No          |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/EF882724909A6A91D588C9081EC5B5107F3875E4) | 2020-12-21   | No          |                     1 |

## ContactInfo: twentytwo at countermail dot com tor-relay.co (3) {#twentytwoatcountermaildotcom-tor-relayco}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Shibaa](https://metrics.torproject.org/rs.html#details/313BFC204E905916C303D246BD20CC1B140B13FE)    | 2021-12-23   | Yes         |                     1 |
| [Shibuu](https://metrics.torproject.org/rs.html#details/BC82C406F93334DE16F7984996CEB0908B348C78)    | 2021-12-18   | Yes         |                     1 |
| [Shibanode](https://metrics.torproject.org/rs.html#details/6802A281D24F4A3FE1DD90EA37EC233B7F83C9D5) | 2021-12-18   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

328ED3A92D1CD621659B4DA6E210FCAED813174B,3688001D75469101F74A5D551A49B0EF410F0E26,4918A461CEE1C8E65F4272E40CF3C6C6E70BB22C,A4A79E2B8294AA2572B46C5C772E149F84FAF763,D8CE67E09B3E0B0D5A5CBF3AA0C702B804D5B7C8,313BFC204E905916C303D246BD20CC1B140B13FE,BC82C406F93334DE16F7984996CEB0908B348C78,E4A8BC82E660528D5B0B8D36C08AB44B77351736