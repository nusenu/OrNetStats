---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-09-19 16:00 UTC**

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


## ContactInfo: your@e-mail (5) {#youre-mail}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [AMSRelay](https://metrics.torproject.org/rs.html#details/A9DA735C9DE7C891B9EDD6B433B458F7687E829B)    | 2022-08-29   | Yes         |                     1 |
| [BlackMesaAG](https://metrics.torproject.org/rs.html#details/14693074C2325CEC8746AFBB85291E749AC45D5D) | 2021-12-29   | Yes         |                     1 |
| [CoolRelay](https://metrics.torproject.org/rs.html#details/D594BC4244636CC342973B594B707685DCAA0C87)   | 2022-07-11   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/21524A2BC6C4275B2FDC23F0FF2344B6D8FEC255) | 2022-08-18   | Yes         |                     1 |
| [0d210s](https://metrics.torproject.org/rs.html#details/D2B845D50ED5B49A8B8B425AB530C38D952E5C3C)      | 2022-09-08   | No          |                     1 |

## ContactInfo: potlatch protonmail com (7) {#potlatch-protonmail-com}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [TorExitCz](https://metrics.torproject.org/rs.html#details/FFEA37B6DA76C458D3E35476DD7D1FD0A98AE731)      | 2021-12-07   | Yes         |                     8 |
| [lollipop](https://metrics.torproject.org/rs.html#details/08CD9D4224058DC97A1F27679A5BEE5724C4C6EC)       | 2020-08-15   | Yes         |                     8 |
| [rome2](https://metrics.torproject.org/rs.html#details/02357911B882F257676E75B07ECFFF5885E4B345)          | 2022-09-15   | No          |                     1 |
| [TorExitRomania](https://metrics.torproject.org/rs.html#details/4061C553CA88021B8302F0814365070AAE617270) | 2016-03-02   | No          |                     8 |
| [TorExitMoldova](https://metrics.torproject.org/rs.html#details/742C45F2D9004AADE0077E528A4418A6A81BC2BA) | 2019-01-01   | No          |                     8 |
| [TorExitFinland](https://metrics.torproject.org/rs.html#details/9B31F1F1C1554F9FFB3455911F82E818EF7C7883) | 2015-12-31   | No          |                     8 |
| [TorExitMoldova](https://metrics.torproject.org/rs.html#details/B06F093A3D4DFAD3E923F4F28A74901BD4F74EB1) | 2017-05-24   | No          |                     8 |


## Fingerprint List of Guard-only Relays in E2E Groups

14693074C2325CEC8746AFBB85291E749AC45D5D,21524A2BC6C4275B2FDC23F0FF2344B6D8FEC255,5788F2CD0808CC2BB3F3679DC4BB40FCDB0C152C,A9DA735C9DE7C891B9EDD6B433B458F7687E829B,D594BC4244636CC342973B594B707685DCAA0C87,08CD9D4224058DC97A1F27679A5BEE5724C4C6EC,FFEA37B6DA76C458D3E35476DD7D1FD0A98AE731