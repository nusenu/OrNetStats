---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-05-06 17:00 UTC**

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


## ContactInfo: James at charles dot onion (8) {#jamesatcharlesdotonion}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Mooncake](https://metrics.torproject.org/rs.html#details/C1C239582DDDA2DFCE674D365861FB2C1A96D8B9)     | 2021-02-28   | Yes         |                    29 |
| [Zekrom](https://metrics.torproject.org/rs.html#details/9F1687D0D79A74F2C6F9FB918089405565BA5329)       | 2021-04-28   | Yes         |                    29 |
| [MewTwo](https://metrics.torproject.org/rs.html#details/8198249E251A7072D8481D19BE45C77FCA709EB6)       | 2021-04-22   | Yes         |                    29 |
| [Moonpie](https://metrics.torproject.org/rs.html#details/096DE80D4C1E457680C23B56B6DABE9AA6A6260C)      | 2021-02-18   | Yes         |                    29 |
| [Reshiram](https://metrics.torproject.org/rs.html#details/07007CB632002FC92FB11DE78C72C44B5160A1A3)     | 2021-04-28   | Yes         |                    29 |
| [MoonLoon](https://metrics.torproject.org/rs.html#details/261A7D651D319021D7141B7CE3ECA6E9DA983540)     | 2021-03-02   | Yes         |                    29 |
| [Rachmaninoff](https://metrics.torproject.org/rs.html#details/DF187D0E3481F6C6FE60836C28AE4948A77A4761) | 2021-05-05   | No          |                     1 |
| [Treecko](https://metrics.torproject.org/rs.html#details/E0F4900D063080D44AB4C043FBAB4C2F964CB612)      | 2021-03-11   | No          |                    29 |

## ContactInfo: james at charles dot onion tor-relay.co (10) {#jamesatcharlesdotonion-tor-relayco}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Chespin](https://metrics.torproject.org/rs.html#details/DC862F7BBF619EA3FA4FB667A4D8118652922FC8)    | 2021-03-19   | Yes         |                    29 |
| [Tepig](https://metrics.torproject.org/rs.html#details/751EDB5D969C72479270D223823A8ED4E578C070)      | 2021-03-19   | Yes         |                    29 |
| [Snivy](https://metrics.torproject.org/rs.html#details/D4C733CA1FF5D85C3571FF39DBC7DB431966A47D)      | 2021-03-19   | Yes         |                    29 |
| [Chimchar](https://metrics.torproject.org/rs.html#details/ED967A94B73BF678660EAA91890F450250CA0575)   | 2021-03-16   | Yes         |                    29 |
| [Turtwig](https://metrics.torproject.org/rs.html#details/8B9110B997437724115CFCDB1B2495463F77669B)    | 2021-03-16   | Yes         |                    29 |
| [Rowlet](https://metrics.torproject.org/rs.html#details/690FC3ACBBBC970309A9A0993EE12AF44C0C8E62)     | 2021-03-16   | Yes         |                    29 |
| [Zaranof](https://metrics.torproject.org/rs.html#details/1CC1D5835BA99A01FFE4D88E83D115E54F2D698C)    | 2021-05-05   | No          |                     1 |
| [dragonbleu](https://metrics.torproject.org/rs.html#details/24DC6F435824B3D82BFD7841D6FC2216BA11B8BC) | 2021-05-05   | No          |                     1 |
| [Mudkip](https://metrics.torproject.org/rs.html#details/75983F5660D894FCF2BE452DB35F3E594ADE4B08)     | 2021-03-13   | No          |                    29 |
| [Torchick](https://metrics.torproject.org/rs.html#details/91D129CEBBC3F1BE27BCF8019F1F7A8B0F27E1C2)   | 2021-03-13   | No          |                    29 |


## Fingerprint List of Guard-only Relays in E2E Groups

07007CB632002FC92FB11DE78C72C44B5160A1A3,096DE80D4C1E457680C23B56B6DABE9AA6A6260C,261A7D651D319021D7141B7CE3ECA6E9DA983540,8198249E251A7072D8481D19BE45C77FCA709EB6,9F1687D0D79A74F2C6F9FB918089405565BA5329,C1C239582DDDA2DFCE674D365861FB2C1A96D8B9,690FC3ACBBBC970309A9A0993EE12AF44C0C8E62,751EDB5D969C72479270D223823A8ED4E578C070,8B9110B997437724115CFCDB1B2495463F77669B,D4C733CA1FF5D85C3571FF39DBC7DB431966A47D,DC862F7BBF619EA3FA4FB667A4D8118652922FC8,ED967A94B73BF678660EAA91890F450250CA0575