---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-03-01 18:00 UTC**

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


## ContactInfo: admin dot tor-operator at firemail dot tech pgp:70 (5) {#admin-dot-tor-operator-at-firemail-dot-tech-pgp70}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Zinc](https://metrics.torproject.org/rs.html#details/01F73DBD9B56C31E3D3AAEB95F8CF1DEB7D9A72F)      | 2020-04-13   | Yes         |                     4 |
| [Oxygen](https://metrics.torproject.org/rs.html#details/B29E6646E11E5E6EAFE7DDE5AD3C3FE966B49E4E)    | 2022-01-11   | Yes         |                     5 |
| [Plutonium](https://metrics.torproject.org/rs.html#details/6859D71E3E1323F959F9E0559E83A9088C462684) | 2021-12-09   | No          |                     4 |
| [Hydrogen](https://metrics.torproject.org/rs.html#details/702FD318AEED49702B5C16255ED5F595DA116516)  | 2020-10-01   | No          |                     5 |
| [Uranium](https://metrics.torproject.org/rs.html#details/90B818902D42800A5E5F31A2C0D9A2B0B31EAC5F)   | 2020-11-29   | No          |                     5 |

## ContactInfo: &lt;nobody AT example dot com&gt; (3) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [node01](https://metrics.torproject.org/rs.html#details/D53AE170BF6650A2C6640484FE1B5DD1C0AB895B)     | 2019-12-14   | Yes         |                     1 |
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

01F73DBD9B56C31E3D3AAEB95F8CF1DEB7D9A72F,B29E6646E11E5E6EAFE7DDE5AD3C3FE966B49E4E,A9A4213EA3D707857368C683F2208C83B8755D8A,D53AE170BF6650A2C6640484FE1B5DD1C0AB895B