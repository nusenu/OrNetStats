---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-08-04 15:00 UTC**

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


## ContactInfo: gus@riseup.net (12) {#gusriseupnet}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Kanellos](https://metrics.torproject.org/rs.html#details/028BEF4A81578286BAA1352C73E4609B9915C687)    | 2023-07-14   | Yes         |                    18 |
| [Kanellos](https://metrics.torproject.org/rs.html#details/73D5045F4AE50B224CABDADC339B5D101CF5A465)    | 2023-07-14   | Yes         |                    18 |
| [Kanellos](https://metrics.torproject.org/rs.html#details/9E47303453F961132C2A59D2966F5A6EFA13B6A5)    | 2023-07-14   | Yes         |                    18 |
| [Kanellos](https://metrics.torproject.org/rs.html#details/531B3B0391A92F08376A4D5FAFAAC04009690FD1)    | 2023-07-14   | Yes         |                    18 |
| [Kanellos](https://metrics.torproject.org/rs.html#details/D14B58EACE3EC7D1B367C881B85815B9E985BCE7)    | 2023-07-14   | Yes         |                    18 |
| [Kanellos](https://metrics.torproject.org/rs.html#details/58FE6772343FF6CD9E53D8B040A2CE495808E93D)    | 2023-07-14   | Yes         |                    18 |
| [Kanellos](https://metrics.torproject.org/rs.html#details/70B0FD26318C6058D363059C69CAD9CE9CA587C1)    | 2023-07-14   | Yes         |                    18 |
| [Kanellos](https://metrics.torproject.org/rs.html#details/83F02FD5FEA0B87A6FB18EEC52E3006766E1E92E)    | 2023-07-14   | Yes         |                    18 |
| [RunBSD](https://metrics.torproject.org/rs.html#details/568E434F725B7828D17EF2B33C2F5CC84F18FCE3)      | 2020-01-03   | Yes         |                    19 |
| [Caramelo](https://metrics.torproject.org/rs.html#details/DE15A1432DFB127B49F4C6FD9D48771683732995)    | 2023-07-17   | Yes         |                     8 |
| [HangTheDJ](https://metrics.torproject.org/rs.html#details/1DA888D47E43EDFCC60CBC0E1FDF0C8A43D64343)   | 2020-08-29   | No          |                    11 |
| [ZeroCalcare](https://metrics.torproject.org/rs.html#details/FED2F5D81CCA06698E540A42038CB3D6AEF747C2) | 2021-11-26   | No          |                    19 |


## Fingerprint List of Guard-only Relays in E2E Groups

028BEF4A81578286BAA1352C73E4609B9915C687,531B3B0391A92F08376A4D5FAFAAC04009690FD1,568E434F725B7828D17EF2B33C2F5CC84F18FCE3,58FE6772343FF6CD9E53D8B040A2CE495808E93D,70B0FD26318C6058D363059C69CAD9CE9CA587C1,73D5045F4AE50B224CABDADC339B5D101CF5A465,83F02FD5FEA0B87A6FB18EEC52E3006766E1E92E,9E47303453F961132C2A59D2966F5A6EFA13B6A5,D14B58EACE3EC7D1B367C881B85815B9E985BCE7,DE15A1432DFB127B49F4C6FD9D48771683732995