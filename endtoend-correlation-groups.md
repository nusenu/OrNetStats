---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-04-28 18:00 UTC**

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


## ContactInfo: shebangs@yopmail.fr (15) {#shebangsyopmailfr}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Shebangs](https://metrics.torproject.org/rs.html#details/F5F9B6B40E4D7AFCECDFB1F4503D56D522C7EFAA) | 2020-09-13   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/453E51CBAA4C2169EBCB05583247DD6201E87FAD) | 2020-06-05   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/BA8546AE9B27F0C81F98A6C12D96B7DAB0814991) | 2020-06-06   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/CEA2E066A7F8EC0F235F5190E25DD3C9F86F084B) | 2020-06-06   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/AC990FD1FF5058EFA43A809E948B23EF998D021B) | 2020-06-05   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/F3A3461889BF97250F50A7BAAAE4A2B92062F6D7) | 2020-07-03   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/E4A8BC82E660528D5B0B8D36C08AB44B77351736) | 2020-12-17   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/328ED3A92D1CD621659B4DA6E210FCAED813174B) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/072E4EC47D640118D5438BFFDFF1AF7BB4E2AD2B) | 2020-10-05   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/1ACC9F9550F6DD6AC3FE8BC9B2F1CF42C968099C) | 2021-02-06   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/EF2A6ECE4277F55F29253DEBA80F04DA66BEA166) | 2021-02-13   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/A4A79E2B8294AA2572B46C5C772E149F84FAF763) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/3688001D75469101F74A5D551A49B0EF410F0E26) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/5A8918BCA6B05FC780CFBDD66703BEF60DE53DA6) | 2020-12-25   | No          |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/E9272A28DAFABAE4F3D07233A16D13BDD5F58D4A) | 2020-12-25   | No          |                     1 |

## ContactInfo: karabyte@disroot.org (2) {#karabytedisrootorg}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [KarabyteRelay2](https://metrics.torproject.org/rs.html#details/27A5A753D0664A94C319F9C3D2241F2E80993D12) | 2021-04-12   | Yes         |                     1 |
| [KarabyteExit1](https://metrics.torproject.org/rs.html#details/3367BFB7140BDF16C72A9A5A1CF757E993998D2A)  | 2021-04-03   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

072E4EC47D640118D5438BFFDFF1AF7BB4E2AD2B,1ACC9F9550F6DD6AC3FE8BC9B2F1CF42C968099C,328ED3A92D1CD621659B4DA6E210FCAED813174B,3688001D75469101F74A5D551A49B0EF410F0E26,453E51CBAA4C2169EBCB05583247DD6201E87FAD,A4A79E2B8294AA2572B46C5C772E149F84FAF763,AC990FD1FF5058EFA43A809E948B23EF998D021B,BA8546AE9B27F0C81F98A6C12D96B7DAB0814991,CEA2E066A7F8EC0F235F5190E25DD3C9F86F084B,E4A8BC82E660528D5B0B8D36C08AB44B77351736,EF2A6ECE4277F55F29253DEBA80F04DA66BEA166,F3A3461889BF97250F50A7BAAAE4A2B92062F6D7,F5F9B6B40E4D7AFCECDFB1F4503D56D522C7EFAA,27A5A753D0664A94C319F9C3D2241F2E80993D12