---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-06-03 20:00 UTC**

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


## ContactInfo: abuse@torrelays.ru (32) {#abusetorrelaysru}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Eristof](https://metrics.torproject.org/rs.html#details/DC4349041B89D9FDD4DC53BD680B42B37A9CB195)      | 2021-05-03   | Yes         |                    35 |
| [Geodude](https://metrics.torproject.org/rs.html#details/51BD782616C3EBA543B0D4EE34D7C1CE1ED2291D)      | 2021-03-20   | Yes         |                    35 |
| [Mooncake](https://metrics.torproject.org/rs.html#details/C1C239582DDDA2DFCE674D365861FB2C1A96D8B9)     | 2021-02-28   | Yes         |                    40 |
| [Tepig](https://metrics.torproject.org/rs.html#details/751EDB5D969C72479270D223823A8ED4E578C070)        | 2021-03-19   | Yes         |                    40 |
| [Chespin](https://metrics.torproject.org/rs.html#details/DC862F7BBF619EA3FA4FB667A4D8118652922FC8)      | 2021-03-19   | Yes         |                    40 |
| [Moonpie](https://metrics.torproject.org/rs.html#details/096DE80D4C1E457680C23B56B6DABE9AA6A6260C)      | 2021-02-18   | Yes         |                    40 |
| [SunnyShiner](https://metrics.torproject.org/rs.html#details/1A647701D0368E8F073FF38773986F43A24C60CA)  | 2021-05-13   | Yes         |                    40 |
| [Bulbasaur](https://metrics.torproject.org/rs.html#details/E789DDCFDF2F92F3A6548796A22D5C8E64EE1A1B)    | 2021-03-08   | Yes         |                    40 |
| [Moonshine](https://metrics.torproject.org/rs.html#details/3326C64CD86258ACA4657E3501BE6BECA672DB18)    | 2021-02-12   | Yes         |                    40 |
| [Snivy](https://metrics.torproject.org/rs.html#details/D4C733CA1FF5D85C3571FF39DBC7DB431966A47D)        | 2021-03-19   | Yes         |                    40 |
| [Chimchar](https://metrics.torproject.org/rs.html#details/ED967A94B73BF678660EAA91890F450250CA0575)     | 2021-03-16   | Yes         |                    40 |
| [Oshawott](https://metrics.torproject.org/rs.html#details/55ED11C6B5A35D40CD07F5A8DC12B82F0B7AADDF)     | 2021-03-18   | Yes         |                    40 |
| [MoonLoon](https://metrics.torproject.org/rs.html#details/261A7D651D319021D7141B7CE3ECA6E9DA983540)     | 2021-03-02   | Yes         |                    40 |
| [Rowlet](https://metrics.torproject.org/rs.html#details/690FC3ACBBBC970309A9A0993EE12AF44C0C8E62)       | 2021-03-16   | Yes         |                    40 |
| [Moonlight](https://metrics.torproject.org/rs.html#details/9546182589B1E4BF6B025875FAEBE309E7359D56)    | 2021-03-05   | Yes         |                    40 |
| [MoonBeam](https://metrics.torproject.org/rs.html#details/B08504ABC6BBA71D78163EADDB8D8248D7DB53F4)     | 2021-03-05   | Yes         |                    40 |
| [Turtwig](https://metrics.torproject.org/rs.html#details/8B9110B997437724115CFCDB1B2495463F77669B)      | 2021-03-16   | Yes         |                    40 |
| [Cyndaquil](https://metrics.torproject.org/rs.html#details/ADA98E1C50E0635BDDECB4C9D448C72040275045)    | 2021-03-09   | Yes         |                    40 |
| [Charmander](https://metrics.torproject.org/rs.html#details/45DC9BCF0E44A22D246ECC02234B216EAA02155E)   | 2021-03-08   | Yes         |                    40 |
| [Chikorita](https://metrics.torproject.org/rs.html#details/55566C567D7F9E9EE70368AEFA29593EC34FB0A5)    | 2021-03-09   | Yes         |                    40 |
| [Totodile](https://metrics.torproject.org/rs.html#details/BF8A9BCA68F14B49939063B7BD3D32E23533C125)     | 2021-03-09   | Yes         |                    40 |
| [Pickachu](https://metrics.torproject.org/rs.html#details/34F2DBF5595FF8323665BEC7DD8D2D28F9697B2C)     | 2021-03-07   | Yes         |                    40 |
| [Piplup](https://metrics.torproject.org/rs.html#details/62F65E6377F0647CE0F0EE2AAE1641EC4AA2BD3B)       | 2021-03-07   | Yes         |                    40 |
| [Squirtle](https://metrics.torproject.org/rs.html#details/ADDFC1F6208B4C59A6FF3DAAA5A93B481720595A)     | 2021-03-08   | Yes         |                    40 |
| [dragonbleu](https://metrics.torproject.org/rs.html#details/24DC6F435824B3D82BFD7841D6FC2216BA11B8BC)   | 2021-05-05   | No          |                    40 |
| [saturn](https://metrics.torproject.org/rs.html#details/5ECBA2DDE6403E0F0B73E452F65EA2606929332A)       | 2021-05-09   | No          |                    40 |
| [Mudkip](https://metrics.torproject.org/rs.html#details/75983F5660D894FCF2BE452DB35F3E594ADE4B08)       | 2021-03-13   | No          |                    40 |
| [Torchick](https://metrics.torproject.org/rs.html#details/91D129CEBBC3F1BE27BCF8019F1F7A8B0F27E1C2)     | 2021-03-13   | No          |                    40 |
| [Treecko](https://metrics.torproject.org/rs.html#details/9A1B7A104EDDB799E1063EF0C27342E7BD1B465D)      | 2021-06-03   | No          |                     1 |
| [venus](https://metrics.torproject.org/rs.html#details/A979319FECD831EE650297E3C7E54DFF9A561C0D)        | 2021-05-09   | No          |                    40 |
| [Rachmaninoff](https://metrics.torproject.org/rs.html#details/DF187D0E3481F6C6FE60836C28AE4948A77A4761) | 2021-05-05   | No          |                    40 |
| [Litten](https://metrics.torproject.org/rs.html#details/F1C4F08DE356EFC6495B40E3E7698F0ACAD4C5AC)       | 2021-05-19   | No          |                    40 |

## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; (6) {#neel-chauhan-neel-at-neelc-dot-org}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelayA](https://metrics.torproject.org/rs.html#details/B0F9BA27944FA59E3B1A182208FF7C0CFF5497B2) | 2020-06-14   | Yes         |                     4 |
| [NeelTorRelayB](https://metrics.torproject.org/rs.html#details/DB710B14D7329B7289CFCC547F48EF53F812C40D) | 2020-06-14   | Yes         |                     4 |
| [NeelTorExitA](https://metrics.torproject.org/rs.html#details/035485A94591505E17683D2A350318DE2C384BAA)  | 2020-12-24   | No          |                     6 |
| [NeelTorExitC](https://metrics.torproject.org/rs.html#details/9B49F7C1B0B73988CE01091E963740117DA6D20D)  | 2021-02-03   | No          |                     4 |
| [NeelTorExitD](https://metrics.torproject.org/rs.html#details/B1F9BDD70BC91BFBC9061918C902F40E04E066B2)  | 2021-02-03   | No          |                     4 |
| [NeelTorExitB](https://metrics.torproject.org/rs.html#details/FDE5D296791B47BC99FF7107B188A458C02832FC)  | 2020-12-24   | No          |                     6 |


## Fingerprint List of Guard-only Relays in E2E Groups

07007CB632002FC92FB11DE78C72C44B5160A1A3,096DE80D4C1E457680C23B56B6DABE9AA6A6260C,1A647701D0368E8F073FF38773986F43A24C60CA,261A7D651D319021D7141B7CE3ECA6E9DA983540,3326C64CD86258ACA4657E3501BE6BECA672DB18,34F2DBF5595FF8323665BEC7DD8D2D28F9697B2C,45DC9BCF0E44A22D246ECC02234B216EAA02155E,51BD782616C3EBA543B0D4EE34D7C1CE1ED2291D,55566C567D7F9E9EE70368AEFA29593EC34FB0A5,55ED11C6B5A35D40CD07F5A8DC12B82F0B7AADDF,62F65E6377F0647CE0F0EE2AAE1641EC4AA2BD3B,690FC3ACBBBC970309A9A0993EE12AF44C0C8E62,751EDB5D969C72479270D223823A8ED4E578C070,8B9110B997437724115CFCDB1B2495463F77669B,9546182589B1E4BF6B025875FAEBE309E7359D56,9F1687D0D79A74F2C6F9FB918089405565BA5329,ADA98E1C50E0635BDDECB4C9D448C72040275045,ADDFC1F6208B4C59A6FF3DAAA5A93B481720595A,B08504ABC6BBA71D78163EADDB8D8248D7DB53F4,BF8A9BCA68F14B49939063B7BD3D32E23533C125,C1C239582DDDA2DFCE674D365861FB2C1A96D8B9,D4C733CA1FF5D85C3571FF39DBC7DB431966A47D,DC4349041B89D9FDD4DC53BD680B42B37A9CB195,DC862F7BBF619EA3FA4FB667A4D8118652922FC8,E789DDCFDF2F92F3A6548796A22D5C8E64EE1A1B,ED967A94B73BF678660EAA91890F450250CA0575,B0F9BA27944FA59E3B1A182208FF7C0CFF5497B2,DB710B14D7329B7289CFCC547F48EF53F812C40D