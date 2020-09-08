---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-09-08 13:00 UTC**

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


## ContactInfo: Kevin Hicks &lt;admin@fissionrelays.net&gt; (23) {#kevin-hicks-adminfissionrelaysnet}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [FissionEx3](https://metrics.torproject.org/rs.html#details/4FDDFAD51B24DDABB62FB59071F4DC421E76C685)    | 2018-10-15   | Yes         |                    22 |
| [Fission07](https://metrics.torproject.org/rs.html#details/5D765770B4DB110D88787457978AB4008CF65CAC)     | 2018-02-06   | Yes         |                    22 |
| [Fission11](https://metrics.torproject.org/rs.html#details/929BB84A68198CE35E2F2828812840AF5C2CBC4A)     | 2019-02-06   | Yes         |                    22 |
| [Fission05](https://metrics.torproject.org/rs.html#details/71539D1911ECB826069A4D156771AC4F9F4632A7)     | 2018-02-06   | Yes         |                    22 |
| [Fission10](https://metrics.torproject.org/rs.html#details/438DC9B6B5C5375D332BB338D7E5C1B9EF448960)     | 2019-02-05   | Yes         |                    22 |
| [Fission08](https://metrics.torproject.org/rs.html#details/53134D9637D9FBE565FA1E3AF82B23CC964C56D6)     | 2018-02-06   | Yes         |                    22 |
| [Fission06](https://metrics.torproject.org/rs.html#details/91E7CA6B8D0AAD77C7CFB8FEA25BF4F46DA1042A)     | 2018-02-06   | Yes         |                    22 |
| [Fission09](https://metrics.torproject.org/rs.html#details/98138DFD3E2C8C89D8F5AB11EF9B6BFF272D83B4)     | 2019-02-05   | Yes         |                    22 |
| [Fission01](https://metrics.torproject.org/rs.html#details/62712B2C24A169B24336CD2FE2BE55DA67476C8B)     | 2018-01-07   | Yes         |                    22 |
| [FissionEx4](https://metrics.torproject.org/rs.html#details/3B4C5729F829CA2E895B81AF834A63DB336D0FFE)    | 2019-02-03   | Yes         |                    22 |
| [Fission04](https://metrics.torproject.org/rs.html#details/0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)     | 2020-01-04   | Yes         |                    22 |
| [Fission02](https://metrics.torproject.org/rs.html#details/937F201D2797314953F268D252F5C98D3FA9F71E)     | 2018-01-07   | Yes         |                    22 |
| [Fission12](https://metrics.torproject.org/rs.html#details/C303038FDCC72805A160FF64E994333A49ECDA71)     | 2020-01-24   | Yes         |                    22 |
| [FissionEx6](https://metrics.torproject.org/rs.html#details/20CD933EDC7260B19040475B24FD6B01B73E94BB)    | 2020-08-10   | Yes         |                     1 |
| [Fission03](https://metrics.torproject.org/rs.html#details/4F500157ABF70A1A94636D268A742A8B227B8BFD)     | 2020-01-04   | Yes         |                    22 |
| [FissionMasq05](https://metrics.torproject.org/rs.html#details/41427448C41642832130C2C29AF1FEAC3B3EED35) | 2020-02-26   | No          |                    22 |
| [FissionEx2](https://metrics.torproject.org/rs.html#details/460E5B882770C19761BC5747541913DB2AD01E35)    | 2018-07-08   | No          |                    22 |
| [FissionMasq01](https://metrics.torproject.org/rs.html#details/4A411DD8EBBD539AA0090A305856B9C838F7F2D6) | 2020-01-12   | No          |                    22 |
| [FissionMasq02](https://metrics.torproject.org/rs.html#details/5FA7596FB2BA2C889337F8B82DD7127BBB240D4D) | 2020-02-25   | No          |                    22 |
| [FissionMasq04](https://metrics.torproject.org/rs.html#details/7533ABDA9027F40CF87FB6189AEBB1F43A132A0B) | 2020-02-25   | No          |                    22 |
| [FissionMasq03](https://metrics.torproject.org/rs.html#details/8628D2ACCA1C9BE596DED1DF9D0099BBDB1352B3) | 2020-02-25   | No          |                    22 |
| [FissionMasq06](https://metrics.torproject.org/rs.html#details/87357FCC2BF2C21F069714381BCA6C3E7EFCBD5D) | 2020-02-26   | No          |                    22 |
| [FissionEx5](https://metrics.torproject.org/rs.html#details/DE0421FBD771E6189205D353366874B1790185C7)    | 2020-05-22   | No          |                    22 |

## ContactInfo: see https://www.artikel5ev.de/torcontact/ (17) {#see-httpswwwartikel5evdetorcontact}

| Nickname                                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [dc6jgk13](https://metrics.torproject.org/rs.html#details/E6D4332BF40FDEE7814F2DBC926650EF8032B643)           | 2020-08-28   | Yes         |                    15 |
| [dc6jgk7b](https://metrics.torproject.org/rs.html#details/F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A)           | 2016-11-04   | Yes         |                    22 |
| [dc6jgk9barm64](https://metrics.torproject.org/rs.html#details/78BC2254D3B31CD865F7682633AA438212132532)      | 2016-11-11   | Yes         |                    22 |
| [dc6jgk11barm64](https://metrics.torproject.org/rs.html#details/7B700C0C207EBD0002E00F499BE265519AC3C25A)     | 2016-11-11   | Yes         |                    22 |
| [dc6jgk2](https://metrics.torproject.org/rs.html#details/A60697FF383EEEE2E88505DD4E305C07BF326B11)            | 2019-04-08   | Yes         |                    22 |
| [dc6jgk1](https://metrics.torproject.org/rs.html#details/486740353B905AA4731F82C0B4CC25821A62C6E3)            | 2014-06-09   | Yes         |                    22 |
| [PiratenparteiH3rmi](https://metrics.torproject.org/rs.html#details/A690C6AA8102C027D297AF3401BFE16918CCF7A6) | 2016-07-22   | Yes         |                    18 |
| [dc6jgk6](https://metrics.torproject.org/rs.html#details/A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13)            | 2016-10-06   | Yes         |                    22 |
| [artikel5ev7](https://metrics.torproject.org/rs.html#details/22404A3E87F2D7FE2FC6359FDE71B6DC2D6E730F)        | 2017-08-30   | Yes         |                    18 |
| [artikel5ev1](https://metrics.torproject.org/rs.html#details/0BC8BA32CC3CB0F598E0C92778F7C0946DFBCE91)        | 2016-10-19   | No          |                    18 |
| [artikel5ev3b](https://metrics.torproject.org/rs.html#details/195712E96FD1C1B18D14D09E9E4E7A6416E23B2C)       | 2017-12-05   | No          |                    18 |
| [artikel5ev4](https://metrics.torproject.org/rs.html#details/26C28F29B611DF4DE23ACF5D9DC1EB4895EF5E8B)        | 2019-01-25   | No          |                    18 |
| [artikel5ev8](https://metrics.torproject.org/rs.html#details/4D0DF468DC816F8096702C2DA2C6FD67561F81C8)        | 2019-12-29   | No          |                    22 |
| [artikel5ev13](https://metrics.torproject.org/rs.html#details/89C7E852CC2FA537ED78775ADC3BEA24672B4154)       | 2020-09-07   | No          |                    15 |
| [artikel5ev10](https://metrics.torproject.org/rs.html#details/AF7094B62864DE941DCD88A2F0DBAFECF3997E47)       | 2020-04-12   | No          |                    22 |
| [artikel5ev2](https://metrics.torproject.org/rs.html#details/DC2191663DD4BAECB34F949CCAC3FDA004CE5BCE)        | 2016-10-29   | No          |                    18 |
| [artikel5ev9](https://metrics.torproject.org/rs.html#details/FC077C25B8DBB3132D397D7DF03C92BFC14C9D76)        | 2020-01-11   | No          |                    22 |

## ContactInfo: tomas.vanagas@knf.vu.lt tor-relay.co (2) {#tomasvanagasknfvult-tor-relayco}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [SatoshiNakamoto](https://metrics.torproject.org/rs.html#details/64B43A6198B6C1F97D9ED8929F5A8913C3815935) | 2020-04-28   | Yes         |                     1 |
| [SatoshiNakamoto](https://metrics.torproject.org/rs.html#details/1939CC1B41298A49C0684878813DED5CD1A9EE98) | 2019-03-29   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA,20CD933EDC7260B19040475B24FD6B01B73E94BB,22404A3E87F2D7FE2FC6359FDE71B6DC2D6E730F,3B4C5729F829CA2E895B81AF834A63DB336D0FFE,438DC9B6B5C5375D332BB338D7E5C1B9EF448960,486740353B905AA4731F82C0B4CC25821A62C6E3,4F500157ABF70A1A94636D268A742A8B227B8BFD,4FDDFAD51B24DDABB62FB59071F4DC421E76C685,53134D9637D9FBE565FA1E3AF82B23CC964C56D6,5D765770B4DB110D88787457978AB4008CF65CAC,62712B2C24A169B24336CD2FE2BE55DA67476C8B,64B43A6198B6C1F97D9ED8929F5A8913C3815935,71539D1911ECB826069A4D156771AC4F9F4632A7,78BC2254D3B31CD865F7682633AA438212132532,7B700C0C207EBD0002E00F499BE265519AC3C25A,91E7CA6B8D0AAD77C7CFB8FEA25BF4F46DA1042A,929BB84A68198CE35E2F2828812840AF5C2CBC4A,937F201D2797314953F268D252F5C98D3FA9F71E,98138DFD3E2C8C89D8F5AB11EF9B6BFF272D83B4,A60697FF383EEEE2E88505DD4E305C07BF326B11,A690C6AA8102C027D297AF3401BFE16918CCF7A6,A6AA94B4007A0E2919B2DA8ECF2CFA3CA1761A13,C303038FDCC72805A160FF64E994333A49ECDA71,E6D4332BF40FDEE7814F2DBC926650EF8032B643,F0F5074A6DADD3DC22E1FAA18FD6D89CBC52771A