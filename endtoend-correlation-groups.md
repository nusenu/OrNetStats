---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-10-13 16:00 UTC**

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


## ContactInfo: abuse-node49 AT posteo DOT de (22) {#abuse-node49-at-posteo-dot-de}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Hydra7](https://metrics.torproject.org/rs.html#details/C013F6A7A2297FA4CD00D05EF4A1C5222B844B25)  | 2019-08-21   | Yes         |                    22 |
| [Hydra6](https://metrics.torproject.org/rs.html#details/63DE54637F349FD686CF1C036827B5BE826B9F7C)  | 2018-12-27   | Yes         |                    21 |
| [Hydra4](https://metrics.torproject.org/rs.html#details/B3DA9D673321B92253DCCD38A9740F2C562C91EA)  | 2019-08-20   | Yes         |                    22 |
| [Hydra13](https://metrics.torproject.org/rs.html#details/8CDF2F3A8ABD834CF9F3E8FC202DF64625BFB443) | 2020-02-10   | Yes         |                    21 |
| [Hydra14](https://metrics.torproject.org/rs.html#details/01B70C7C497FC8667DB5EB82C40D8F9214D6A484) | 2019-12-29   | Yes         |                    21 |
| [Hydra5](https://metrics.torproject.org/rs.html#details/034AA4B30F77DF0FE183602EA7F8251FF2CF1BA2)  | 2019-11-23   | No          |                    22 |
| [Hydra2](https://metrics.torproject.org/rs.html#details/0443D98C0C44D3E0E6238790345DB5624DB41B28)  | 2019-12-05   | No          |                    22 |
| [Hydra1](https://metrics.torproject.org/rs.html#details/0647C3F8352BBFA0D57A1C3E0DCF67FC3E073D2C)  | 2017-01-06   | No          |                    22 |
| [Hydra12](https://metrics.torproject.org/rs.html#details/180A5BCC01866E09E4D229B6C084CD1E3C75636F) | 2019-12-15   | No          |                    21 |
| [Hydra16](https://metrics.torproject.org/rs.html#details/1DFE397493D0791DE63F2D6EA5AB6EBCB7B9871A) | 2020-06-09   | No          |                    21 |
| [Hydra3](https://metrics.torproject.org/rs.html#details/27D02579AD5F3E32895D99C38E482D1DC6CBAE5E)  | 2019-10-17   | No          |                    22 |
| [Hydra18](https://metrics.torproject.org/rs.html#details/3AD29FE1241B73595F99BA2C6D830AF0B6874043) | 2020-06-30   | No          |                    21 |
| [Hydra21](https://metrics.torproject.org/rs.html#details/5B7C577DDEBC6B2C39B55364F4EAD69FE8181067) | 2020-10-05   | No          |                    21 |
| [Hydra11](https://metrics.torproject.org/rs.html#details/70A4372ED8F5DDE3BA05A17491BB6032EAC02692) | 2019-11-15   | No          |                    21 |
| [Hydra8](https://metrics.torproject.org/rs.html#details/7716DE8030A56A80080446E0CBC59738605454E6)  | 2019-11-23   | No          |                    22 |
| [Hydra20](https://metrics.torproject.org/rs.html#details/86E479266EBB982E204009532ED460628689E5B5) | 2020-10-07   | No          |                    21 |
| [Hydra15](https://metrics.torproject.org/rs.html#details/C72E73566CB3377AAE5849F5926AD660E4AF82A2) | 2020-01-21   | No          |                    21 |
| [Hydra9](https://metrics.torproject.org/rs.html#details/CB28925DA61069A43584030D2610471F1FFD4100)  | 2019-02-10   | No          |                    22 |
| [Hydra10](https://metrics.torproject.org/rs.html#details/CD21B997AF3D30AD719C066C38C7FA8C8FE83C70) | 2019-02-13   | No          |                    22 |
| [Hydra17](https://metrics.torproject.org/rs.html#details/E3DAF067B028450B31CF5CE118F2F9AC53146ABD) | 2020-06-09   | No          |                    21 |
| [Hydra19](https://metrics.torproject.org/rs.html#details/E465AD166798A3CD0A4866FA2A8BB5ADD157FBD5) | 2020-06-30   | No          |                    21 |
| [Hydra22](https://metrics.torproject.org/rs.html#details/F0B1C546ADA1A199D601727C0C401D0C6F78AB71) | 2020-10-12   | No          |                    10 |


## Fingerprint List of Guard-only Relays in E2E Groups

01B70C7C497FC8667DB5EB82C40D8F9214D6A484,63DE54637F349FD686CF1C036827B5BE826B9F7C,8CDF2F3A8ABD834CF9F3E8FC202DF64625BFB443,B3DA9D673321B92253DCCD38A9740F2C562C91EA,C013F6A7A2297FA4CD00D05EF4A1C5222B844B25