---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-08-31 18:00 UTC**

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


## ContactInfo: torrelaysaregreat@gmail.com (21) {#torrelaysaregreatgmailcom}

| Nickname                                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [rinderwahnRelay3L](https://metrics.torproject.org/rs.html#details/FF9FC6D130FA26AE3AE8B23688691DC419F0F22E)  | 2019-09-19   | Yes         |                    27 |
| [rinderwahnRelay23L](https://metrics.torproject.org/rs.html#details/EFA2E7B073AA4CE2DAF7160F23C90DB805948F4A) | 2019-04-26   | Yes         |                    27 |
| [rinderwahnRelay29L](https://metrics.torproject.org/rs.html#details/73283C4DEBC01D3E4A5FD1BB1F2B50D927379F59) | 2019-12-11   | Yes         |                    27 |
| [rinderwahnR10L2](https://metrics.torproject.org/rs.html#details/2A87609DA1B48F68E30D0993838126D015884AB9)    | 2021-03-19   | Yes         |                    27 |
| [rinderwahnRelay17L](https://metrics.torproject.org/rs.html#details/F8AA8D8CCBA0C5F2836DE6315CDFA6E4A31A0890) | 2019-11-02   | Yes         |                    27 |
| [rinderwahnRelay30L](https://metrics.torproject.org/rs.html#details/B93503D458D9FE97DE5C12D211082871D08F1284) | 2019-12-24   | Yes         |                    27 |
| [rinderwahnRelay10L](https://metrics.torproject.org/rs.html#details/C1939D36649DE98A202429631D8EFC70128D5F5F) | 2019-10-02   | Yes         |                    27 |
| [rinderwahnRelay7L](https://metrics.torproject.org/rs.html#details/EE4AF632058F0734C1426B1AD689F47445CA2056)  | 2018-09-05   | Yes         |                    27 |
| [rinderwahnRelay14L](https://metrics.torproject.org/rs.html#details/465D17C6FC297E3857B5C6F152006A1E212944EA) | 2018-12-15   | Yes         |                    27 |
| [rinderwahnR30L2](https://metrics.torproject.org/rs.html#details/ADF9A16AE8478CDD203CA3664A9B8CA3E38B77AE)    | 2021-03-28   | Yes         |                    27 |
| [rinderwahnRelay34L](https://metrics.torproject.org/rs.html#details/D4DC70B25409B8E4B0FD482B8A70CA6A3F4A123C) | 2020-08-03   | Yes         |                    27 |
| [rinderwahnRelay37L](https://metrics.torproject.org/rs.html#details/6429B0D703EB90A18528F9F8B843504AA27765C6) | 2020-12-29   | Yes         |                    27 |
| [rinderwahnRelay18L](https://metrics.torproject.org/rs.html#details/B517198B86B3859C307857C59F6660A281FC8B47) | 2019-01-10   | Yes         |                    27 |
| [rinderwahnRelay33L](https://metrics.torproject.org/rs.html#details/4BF3D299BC500C350868F078749291C766C7AA6F) | 2020-02-01   | Yes         |                    27 |
| [rinderwahnRelay5L](https://metrics.torproject.org/rs.html#details/39C6F833D4B09524770D3655DF825A11213CA0A9)  | 2019-11-01   | Yes         |                    27 |
| [rinderwahnRelay39L](https://metrics.torproject.org/rs.html#details/9160D3B62CDD78142AB0BFA4276E17409575F3E6) | 2021-02-01   | Yes         |                    27 |
| [rinderwahnRelay9L](https://metrics.torproject.org/rs.html#details/9288B75B5FF8861EFF32A6BE8825CC38A4F9F8C2)  | 2018-09-07   | Yes         |                    27 |
| [Unnamed](https://metrics.torproject.org/rs.html#details/33263BEFC7E6A0D695C049380B4C72A6FBACB857)            | 2022-07-30   | Yes         |                     2 |
| [rinderwahnRelay38L](https://metrics.torproject.org/rs.html#details/61E431EC074880C4CAAE98F1E525E0128762E065) | 2021-01-12   | Yes         |                    27 |
| [rinderwahnRelay16L](https://metrics.torproject.org/rs.html#details/6DC6CDC6DDA99915EB0232071C6DD2C8784A191F) | 2020-07-23   | Yes         |                    28 |
| [rinderwahnExit1W](https://metrics.torproject.org/rs.html#details/DC81AA3B1D51566DBF27BFA562E4047AEB1C52DA)   | 2020-02-11   | No          |                    27 |

## ContactInfo: tor at reichsfunkma dot st tor-relay.co (5) {#tor-at-reichsfunkma-dot-st-tor-relayco}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Reichsfunkmast4](https://metrics.torproject.org/rs.html#details/4F35C7CA62740A43AC6A46A355516B85018AC8A0) | 2022-08-20   | Yes         |                     1 |
| [Reichsfunkmast6](https://metrics.torproject.org/rs.html#details/B0A134CAF4494B3913E05DB46347633D9C4A8A8B) | 2022-06-23   | Yes         |                     4 |
| [Reichsfunkmast](https://metrics.torproject.org/rs.html#details/3B43FB4F237EBE3570CB06B500CA1E8B46EEAFA1)  | 2022-06-03   | No          |                     4 |
| [Reichsfunkmast3](https://metrics.torproject.org/rs.html#details/4977F97D96681EF747441639C4B4A7CA6FFBD132) | 2022-06-16   | No          |                     4 |
| [Reichsfunkmast2](https://metrics.torproject.org/rs.html#details/F3A9588FB45F76DA4DE5B350C425C130F6FFA983) | 2022-06-22   | No          |                     4 |


## Fingerprint List of Guard-only Relays in E2E Groups

2A87609DA1B48F68E30D0993838126D015884AB9,33263BEFC7E6A0D695C049380B4C72A6FBACB857,39C6F833D4B09524770D3655DF825A11213CA0A9,465D17C6FC297E3857B5C6F152006A1E212944EA,4BF3D299BC500C350868F078749291C766C7AA6F,57C6DF5B93E54EB9C8DB90029D9E9A1111BD34D2,61E431EC074880C4CAAE98F1E525E0128762E065,6429B0D703EB90A18528F9F8B843504AA27765C6,6DC6CDC6DDA99915EB0232071C6DD2C8784A191F,73283C4DEBC01D3E4A5FD1BB1F2B50D927379F59,9160D3B62CDD78142AB0BFA4276E17409575F3E6,9288B75B5FF8861EFF32A6BE8825CC38A4F9F8C2,ADF9A16AE8478CDD203CA3664A9B8CA3E38B77AE,B517198B86B3859C307857C59F6660A281FC8B47,B93503D458D9FE97DE5C12D211082871D08F1284,C1939D36649DE98A202429631D8EFC70128D5F5F,D4DC70B25409B8E4B0FD482B8A70CA6A3F4A123C,EE4AF632058F0734C1426B1AD689F47445CA2056,EFA2E7B073AA4CE2DAF7160F23C90DB805948F4A,F8AA8D8CCBA0C5F2836DE6315CDFA6E4A31A0890,4F35C7CA62740A43AC6A46A355516B85018AC8A0,B0A134CAF4494B3913E05DB46347633D9C4A8A8B,FF9FC6D130FA26AE3AE8B23688691DC419F0F22E