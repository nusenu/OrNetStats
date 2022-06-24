---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-06-24 20:00 UTC**

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


## ContactInfo: tor@gusntwrk.xyz (6) {#torgusntwrkxyz}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [elhombre](https://metrics.torproject.org/rs.html#details/B6FD5EF28CF44D882660C042D3DABE7714A059DD) | 2021-10-18   | Yes         |                     2 |
| [gusntwrk](https://metrics.torproject.org/rs.html#details/6933B9BC32FAF71AE2B8360EE8606354737AB5C3) | 2022-04-29   | No          |                     6 |
| [gusntwrk](https://metrics.torproject.org/rs.html#details/6A6C3391DA324E96973690BF45202F2C9159F884) | 2022-05-23   | No          |                     5 |
| [gusntwrk](https://metrics.torproject.org/rs.html#details/6D86FB336DE95CC14C588E92EB1FA1DDC7B8D1B6) | 2022-05-25   | No          |                     5 |
| [gusntwrk](https://metrics.torproject.org/rs.html#details/7EBB68DD851CA98DF268CAB7BD63D4A031855FB0) | 2022-05-25   | No          |                     5 |
| [gusntwrk](https://metrics.torproject.org/rs.html#details/7F39B23F6CD4CBC69C561D4A30C4DC35F0D06396) | 2022-05-25   | No          |                     5 |


## Fingerprint List of Guard-only Relays in E2E Groups

B6FD5EF28CF44D882660C042D3DABE7714A059DD