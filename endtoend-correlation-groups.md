---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-02-14 21:00 UTC**

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
If someone else is using your contactInfo please send an email to bad-relays AT lists DOT torproject DOT org.


## ContactInfo: torrpi1405@gmail.com (28) {#torrpi1405gmailcom}

| Nickname                                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [angeltest3](https://metrics.torproject.org/rs.html#details/FF9FC6D130FA26AE3AE8B23688691DC419F0F22E)       | 2019-09-19   | Yes         |                    27 |
| [angeltest10](https://metrics.torproject.org/rs.html#details/C1939D36649DE98A202429631D8EFC70128D5F5F)      | 2019-10-02   | Yes         |                    27 |
| [angeltest9](https://metrics.torproject.org/rs.html#details/9288B75B5FF8861EFF32A6BE8825CC38A4F9F8C2)       | 2018-09-07   | Yes         |                    27 |
| [angeltest14](https://metrics.torproject.org/rs.html#details/465D17C6FC297E3857B5C6F152006A1E212944EA)      | 2018-12-15   | Yes         |                    27 |
| [angeltest29](https://metrics.torproject.org/rs.html#details/73283C4DEBC01D3E4A5FD1BB1F2B50D927379F59)      | 2019-12-11   | Yes         |                    27 |
| [angeltest7](https://metrics.torproject.org/rs.html#details/EE4AF632058F0734C1426B1AD689F47445CA2056)       | 2018-09-05   | Yes         |                    27 |
| [angeltest28](https://metrics.torproject.org/rs.html#details/1A7A2516A961F2838F7F94786A8811BE82F9CFFE)      | 2019-08-19   | Yes         |                    27 |
| [angeltest6](https://metrics.torproject.org/rs.html#details/295F1BD8995A12ECC77E050CCF6EC641572739E9)       | 2019-08-13   | Yes         |                    27 |
| [angeltest18](https://metrics.torproject.org/rs.html#details/B517198B86B3859C307857C59F6660A281FC8B47)      | 2019-01-10   | Yes         |                    27 |
| [angeltest23](https://metrics.torproject.org/rs.html#details/EFA2E7B073AA4CE2DAF7160F23C90DB805948F4A)      | 2019-04-26   | Yes         |                    27 |
| [angeltest8](https://metrics.torproject.org/rs.html#details/7AAF5597B18D82CC90CA95FB7976A1CEA4A32E06)       | 2018-09-05   | Yes         |                    27 |
| [angeltest13](https://metrics.torproject.org/rs.html#details/A4CC39184AD287D72C2247738835811C7A7ECB8E)      | 2019-11-05   | Yes         |                    27 |
| [angeltest19](https://metrics.torproject.org/rs.html#details/A86EC24F5B8B964F67AC7C27CE92842025983274)      | 2019-01-10   | Yes         |                    27 |
| [angeltest5](https://metrics.torproject.org/rs.html#details/39C6F833D4B09524770D3655DF825A11213CA0A9)       | 2019-11-01   | Yes         |                    27 |
| [angeltest5test](https://metrics.torproject.org/rs.html#details/951307BA74E44A9C9C208B2F134CDA2409944075)   | 2020-01-11   | Yes         |                     1 |
| [angeltest11](https://metrics.torproject.org/rs.html#details/39F91959416763AFD34DBEEC05474411B964B2DC)      | 2018-09-27   | Yes         |                    27 |
| [angeltest17](https://metrics.torproject.org/rs.html#details/F8AA8D8CCBA0C5F2836DE6315CDFA6E4A31A0890)      | 2019-11-02   | Yes         |                    27 |
| [angeltest27](https://metrics.torproject.org/rs.html#details/95C8B9418E74F3FF80E5C3D3AF7F03156FFBBFBE)      | 2019-08-06   | Yes         |                    27 |
| [angeltest12](https://metrics.torproject.org/rs.html#details/57C6DF5B93E54EB9C8DB90029D9E9A1111BD34D2)      | 2018-09-27   | Yes         |                    27 |
| [angeltest26](https://metrics.torproject.org/rs.html#details/40108FDFA40EDB013F7291F3B4DA3D412ED3A5EF)      | 2019-05-29   | Yes         |                    27 |
| [angeltest26test](https://metrics.torproject.org/rs.html#details/F51A927E34662D6005393F2327C870FB0D0D7FE0)  | 2019-11-21   | Yes         |                     1 |
| [angeltest27test](https://metrics.torproject.org/rs.html#details/1323D34C2FA4AE0EC4EEA9853F3464693EF428E7)  | 2019-11-01   | Yes         |                     1 |
| [angeltest20](https://metrics.torproject.org/rs.html#details/ADE6AB2BFBD7A5780B321DC33BBACCD0D777C94D)      | 2019-02-26   | Yes         |                    27 |
| [angeltest31](https://metrics.torproject.org/rs.html#details/2F8B9500DC98C13FD28CC51E47D3416DE423ED78)      | 2020-01-12   | Yes         |                    27 |
| [angeltest2](https://metrics.torproject.org/rs.html#details/3B07C500AC17E7B5A1EE616613E104A094AB87F3)       | 2018-08-28   | Yes         |                    27 |
| [angeltest30](https://metrics.torproject.org/rs.html#details/B93503D458D9FE97DE5C12D211082871D08F1284)      | 2019-12-24   | Yes         |                    27 |
| [angeltest32](https://metrics.torproject.org/rs.html#details/12B1A5769D38FF47CF68C2235E1BDA315DF400F2)      | 2020-01-14   | Yes         |                    27 |
| [angeltestwindows](https://metrics.torproject.org/rs.html#details/DC81AA3B1D51566DBF27BFA562E4047AEB1C52DA) | 2020-02-11   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (2) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4) | 2019-10-25   | Yes         |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/71840F45C2478347B872321066F9805D1A1B79FD)  | 2019-10-25   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

12B1A5769D38FF47CF68C2235E1BDA315DF400F2,1323D34C2FA4AE0EC4EEA9853F3464693EF428E7,1A7A2516A961F2838F7F94786A8811BE82F9CFFE,295F1BD8995A12ECC77E050CCF6EC641572739E9,2F8B9500DC98C13FD28CC51E47D3416DE423ED78,39C6F833D4B09524770D3655DF825A11213CA0A9,39F91959416763AFD34DBEEC05474411B964B2DC,3B07C500AC17E7B5A1EE616613E104A094AB87F3,40108FDFA40EDB013F7291F3B4DA3D412ED3A5EF,465D17C6FC297E3857B5C6F152006A1E212944EA,57C6DF5B93E54EB9C8DB90029D9E9A1111BD34D2,73283C4DEBC01D3E4A5FD1BB1F2B50D927379F59,7AAF5597B18D82CC90CA95FB7976A1CEA4A32E06,9288B75B5FF8861EFF32A6BE8825CC38A4F9F8C2,951307BA74E44A9C9C208B2F134CDA2409944075,95C8B9418E74F3FF80E5C3D3AF7F03156FFBBFBE,A4CC39184AD287D72C2247738835811C7A7ECB8E,A86EC24F5B8B964F67AC7C27CE92842025983274,ADE6AB2BFBD7A5780B321DC33BBACCD0D777C94D,B517198B86B3859C307857C59F6660A281FC8B47,B93503D458D9FE97DE5C12D211082871D08F1284,C1939D36649DE98A202429631D8EFC70128D5F5F,DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4,EE4AF632058F0734C1426B1AD689F47445CA2056,EFA2E7B073AA4CE2DAF7160F23C90DB805948F4A