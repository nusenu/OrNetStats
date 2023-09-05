---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-09-05 21:00 UTC**

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


## ContactInfo: &lt;nobody AT example dot com&gt; (2) {#nobody-at-example-dot-com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [u698id1147](https://metrics.torproject.org/rs.html#details/A9A4213EA3D707857368C683F2208C83B8755D8A) | 2018-02-06   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392)   | 2018-11-22   | No          |                     1 |

## ContactInfo: email:torix protonmail.com url:https://torix-rela (54) {#emailtorixprotonmailcom-urlhttpstorix-rela}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Aramis67](https://metrics.torproject.org/rs.html#details/53C9F4954E7A7332BB0C610C5B8E04CA065AF29B) | 2019-05-13   | Yes         |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/900C879966F1F13F0D407E583DC6FDFFAD05B814)   | 2023-08-09   | Yes         |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/0806B64E53BD3ED2F0BDB5EED8DBF81DF331F45A)   | 2023-05-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/17F41F8DAFA4B36AAB10E202ABA14601AAE1D616)   | 2022-05-10   | No          |                    25 |
| [Aramis](https://metrics.torproject.org/rs.html#details/18105829C1D3A4438C5C156CA7C08FA62279D0C2)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/214F5F96C5AD4EC3858A1CF7665502845496E40A)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/2308F5B08A85F8600DEC23F9C127E1F16E988595)   | 2023-05-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/26551EE9CF98BEE9E7CCA1954B71CC724B3D1A25)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/27AD2A9591BA4809ED2B1F1983AF49CF80919319)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/2B3AAC97B269D59E6D642C8BFB174EDD13741C38)   | 2021-11-12   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/301081DF6A56B542710E5A19C893DA910ABD3C2F)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/33BD34F3E3006EB1375B08995BC7A6988D6F188E)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/359C5231AC2452D365B64A23C27817A1DFEE56B4)   | 2022-05-10   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/410D5B5847C199DE15DE80741BDC0000A5A53C8F)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/4C209C991956896A830890ED74A8AE1207EB8AF4)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/4F9EFCF7689084E4C8EE993E123E32B75368804C)   | 2021-08-22   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/5ECD28C3476E6B3BFFC68E3AB9F2DAFBE3238A95)   | 2023-05-18   | No          |                    25 |
| [Aramis](https://metrics.torproject.org/rs.html#details/62C6E6E50670985089E82FCE16ED841A0728FC3F)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/64163502DFDE9A8BCA73B525170F484DFA703727)   | 2023-05-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/673ABF8132785E24CE48606AD783FDE9BAA92964)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/68F09FE1CD22572D38980184D848BA456302C826)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/6F3E7CD6B97E33F6A91824164A1A9085C045E2C0)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/791DEA860D359D3A3D2F6F13B9856EB0507ED835)   | 2022-06-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/7E0D8A3CD0E0CE0146B1BB8C8CC24FC5F1BBED8D)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/8039659C27E3CB5155CD74FC8CA102BA825FA03B)   | 2023-05-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/828EFC54AF1D0675E6F12F372E46CCE652674359)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/86D98BB659A7EE58F7185EF310358D435F1A32AC)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/89940F610EFB0ED4E624838EAE561ADE55C03321)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/8AA75B47426A2FAE3075AF6EBC2ABDEE02FAD58F)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/8B8CC31223D5E9C413C4E025940B59F7FFF27483)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/92DEFEC7D97366F02043C4F7055CF4A4886817D9)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/96F8ACE10EAC14E76CDEA4C45679EAFFB833F453)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/99A333B824BF47D2C9F2C6DDCBAB856324D428E5)   | 2023-05-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/9A8902B985E2F58BC740671040E7165AC904DD40)   | 2022-06-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/9DBBED552C198FE98520F1190BE35D0534ECDB67)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/9EF49A075A79F657708F5EE00B05CE7B0B79DA35)   | 2022-05-10   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/A0073095A9F39393546FF1A9E997D1A22C0946E1)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/A549E57FC2A060FA20051537E6738B3ED5B98463)   | 2022-05-10   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/B5A65B997C898583F9C4CA16FE603B7347C89588)   | 2022-06-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/B6A5986F404B2C5EB604A37276C0CB7B24FB6631)   | 2023-05-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/C29FEF6A405E730DE07EC74CCF0623D95F0D3A4E)   | 2022-06-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/C528B22D4BA220639F9DCE86A50BB98BDD2FCFB9)   | 2022-06-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/CE0E8EE797257C9F2EB195528CC152FBCF4F2959)   | 2023-05-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/CFF9C18036D401579C473177C0D95B463AD371F7)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/D3F6616034448DEEE369782C96F84FE1407E4200)   | 2021-08-22   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/D510FE86C46E01F24CF4B07C36B55E2619F245BF)   | 2023-05-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/D9CD0C9CE39E91C2996A016A6356FBF4970D96C6)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/DD60CABFEE514E50E8E4B502457E62F667538573)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/E2C0AD7114510F21B9F09E7900185D440C20CC0E)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/F14D2EC67D3B27BE46839D156660F80220660299)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/F314580EA22CB3DCB135D64E92108BFB8FD209AF)   | 2021-11-12   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/F3E6F01671C087AD318BBA47FCD08B65D1A4460E)   | 2022-06-18   | No          |                    54 |
| [Aramis](https://metrics.torproject.org/rs.html#details/F80348BA5A1B758D378C1E7AA7F2E8CC0845A39E)   | 2023-07-18   | No          |                    52 |
| [Aramis](https://metrics.torproject.org/rs.html#details/FC09FFDEB7FFB716B19305A1CE49D2DE88A58E05)   | 2023-05-18   | No          |                    54 |


## Fingerprint List of Guard-only Relays in E2E Groups

A9A4213EA3D707857368C683F2208C83B8755D8A