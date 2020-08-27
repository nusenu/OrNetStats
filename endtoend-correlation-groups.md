---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-08-26 18:00 UTC**

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
| [Fission08](https://metrics.torproject.org/rs.html#details/53134D9637D9FBE565FA1E3AF82B23CC964C56D6)     | 2018-02-06   | Yes         |                    22 |
| [Fission11](https://metrics.torproject.org/rs.html#details/929BB84A68198CE35E2F2828812840AF5C2CBC4A)     | 2019-02-06   | Yes         |                    22 |
| [Fission05](https://metrics.torproject.org/rs.html#details/71539D1911ECB826069A4D156771AC4F9F4632A7)     | 2018-02-06   | Yes         |                    22 |
| [Fission06](https://metrics.torproject.org/rs.html#details/91E7CA6B8D0AAD77C7CFB8FEA25BF4F46DA1042A)     | 2018-02-06   | Yes         |                    22 |
| [Fission12](https://metrics.torproject.org/rs.html#details/C303038FDCC72805A160FF64E994333A49ECDA71)     | 2020-01-24   | Yes         |                    22 |
| [Fission07](https://metrics.torproject.org/rs.html#details/5D765770B4DB110D88787457978AB4008CF65CAC)     | 2018-02-06   | Yes         |                    22 |
| [Fission10](https://metrics.torproject.org/rs.html#details/438DC9B6B5C5375D332BB338D7E5C1B9EF448960)     | 2019-02-05   | Yes         |                    22 |
| [FissionEx6](https://metrics.torproject.org/rs.html#details/20CD933EDC7260B19040475B24FD6B01B73E94BB)    | 2020-08-10   | Yes         |                     1 |
| [Fission04](https://metrics.torproject.org/rs.html#details/0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA)     | 2020-01-04   | Yes         |                    22 |
| [FissionEx4](https://metrics.torproject.org/rs.html#details/3B4C5729F829CA2E895B81AF834A63DB336D0FFE)    | 2019-02-03   | Yes         |                    22 |
| [Fission09](https://metrics.torproject.org/rs.html#details/98138DFD3E2C8C89D8F5AB11EF9B6BFF272D83B4)     | 2019-02-05   | Yes         |                    22 |
| [Fission01](https://metrics.torproject.org/rs.html#details/62712B2C24A169B24336CD2FE2BE55DA67476C8B)     | 2018-01-07   | Yes         |                    22 |
| [Fission02](https://metrics.torproject.org/rs.html#details/937F201D2797314953F268D252F5C98D3FA9F71E)     | 2018-01-07   | Yes         |                    22 |
| [Fission03](https://metrics.torproject.org/rs.html#details/4F500157ABF70A1A94636D268A742A8B227B8BFD)     | 2020-01-04   | Yes         |                    22 |
| [FissionMasq05](https://metrics.torproject.org/rs.html#details/41427448C41642832130C2C29AF1FEAC3B3EED35) | 2020-02-26   | No          |                    22 |
| [FissionEx2](https://metrics.torproject.org/rs.html#details/460E5B882770C19761BC5747541913DB2AD01E35)    | 2018-07-08   | No          |                    22 |
| [FissionMasq01](https://metrics.torproject.org/rs.html#details/4A411DD8EBBD539AA0090A305856B9C838F7F2D6) | 2020-01-12   | No          |                    22 |
| [FissionMasq02](https://metrics.torproject.org/rs.html#details/5FA7596FB2BA2C889337F8B82DD7127BBB240D4D) | 2020-02-25   | No          |                    22 |
| [FissionMasq04](https://metrics.torproject.org/rs.html#details/7533ABDA9027F40CF87FB6189AEBB1F43A132A0B) | 2020-02-25   | No          |                    22 |
| [FissionMasq03](https://metrics.torproject.org/rs.html#details/8628D2ACCA1C9BE596DED1DF9D0099BBDB1352B3) | 2020-02-25   | No          |                    22 |
| [FissionMasq06](https://metrics.torproject.org/rs.html#details/87357FCC2BF2C21F069714381BCA6C3E7EFCBD5D) | 2020-02-26   | No          |                    22 |
| [FissionEx5](https://metrics.torproject.org/rs.html#details/DE0421FBD771E6189205D353366874B1790185C7)    | 2020-05-22   | No          |                    22 |

## ContactInfo: ian@ian.sh (52) {#ianiansh}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [iansh5r](https://metrics.torproject.org/rs.html#details/FEE41B4BC3056FD2B3BF04E20CAC5AD3904CD5AD)   | 2020-07-05   | Yes         |                    42 |
| [iansh5r](https://metrics.torproject.org/rs.html#details/1685E8A79D1D01E4FBC135CD91341C4A4ED802E6)   | 2020-07-05   | Yes         |                    42 |
| [iansh9r](https://metrics.torproject.org/rs.html#details/650FF4A32965D378A55D42A29F6FD1CE914959D3)   | 2020-07-05   | Yes         |                    42 |
| [iansh9r](https://metrics.torproject.org/rs.html#details/C8C46E3E4F00A92C344B367E45F9D63EBB831DE1)   | 2020-07-05   | Yes         |                    42 |
| [iansh8r](https://metrics.torproject.org/rs.html#details/D2F16CBF1BD891968D65D44CD21507E3371279F3)   | 2020-07-05   | Yes         |                    42 |
| [iansh8r](https://metrics.torproject.org/rs.html#details/6A8B54FB9F79E33A307AD0319B62916504A28049)   | 2020-07-05   | Yes         |                    42 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/0C9D7DB63BE030E5CA32E25606632AEB85840F4C) | 2020-07-15   | No          |                    42 |
| [iansh4e](https://metrics.torproject.org/rs.html#details/0F59911D698D3FFE2433B7AB31362FB1EA10237F)   | 2020-07-04   | No          |                    42 |
| [iansh16de](https://metrics.torproject.org/rs.html#details/1044A4B0EEEFE21F99404519F802D00D57CCEF16) | 2020-08-26   | No          |                     1 |
| [iansh16de](https://metrics.torproject.org/rs.html#details/1FB9C354675F7AED809F0037FD1F58C8F6B5A598) | 2020-08-26   | No          |                     1 |
| [iansh16de](https://metrics.torproject.org/rs.html#details/231B7EC3EBA1E36167E10B6781E53F43417BBAFC) | 2020-08-26   | No          |                     1 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/32B4A9F85DC6BFE90DF914C4BAEC5F4EAC793897) | 2020-07-10   | No          |                    42 |
| [iansh16de](https://metrics.torproject.org/rs.html#details/33A678F4B1ACC8066FACD73444F72E097550FF6B) | 2020-08-26   | No          |                     1 |
| [iansh12e](https://metrics.torproject.org/rs.html#details/3466C887F0F53CA5F65662F601A57F329DB460E9)  | 2020-07-08   | No          |                    42 |
| [iansh14fe](https://metrics.torproject.org/rs.html#details/38E75A7B11DFC76A8FC2964DB5DEDDD96B5A5D9C) | 2020-08-26   | No          |                    42 |
| [iansh14fe](https://metrics.torproject.org/rs.html#details/3AB1F18F079CEF1A00E37A4531676C4EB2F867A1) | 2020-08-26   | No          |                    42 |
| [iansh3e](https://metrics.torproject.org/rs.html#details/3CF2646DE677C7A4FD5AE513A6AC59101879A90F)   | 2020-07-04   | No          |                    42 |
| [iansh11e](https://metrics.torproject.org/rs.html#details/462D81E70F753A19C429E31086254DD15034CC9B)  | 2020-07-08   | No          |                    42 |
| [iansh16de](https://metrics.torproject.org/rs.html#details/4A9460C5C3DCF42A357FA6C200A09B60DD065DD5) | 2020-08-26   | No          |                     1 |
| [iansh12e](https://metrics.torproject.org/rs.html#details/4FDC3AE93CD2F81D1B64D94075F6418C06A55314)  | 2020-07-08   | No          |                    42 |
| [iansh16de](https://metrics.torproject.org/rs.html#details/504588F1AEE9E1D64B96BF69ACB607BE82322D4A) | 2020-08-26   | No          |                     1 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/51D3F56EC4543E191B13E614A298ECBC35BEA92E) | 2020-07-30   | No          |                    42 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/5333C98E703385743AE931ECC929C5E4B32A0CD0) | 2020-07-30   | No          |                    42 |
| [iansh2e](https://metrics.torproject.org/rs.html#details/5F29C863F69E9C3B7BD1841B3504FD4173BFA475)   | 2020-07-04   | No          |                    42 |
| [iansh15fe](https://metrics.torproject.org/rs.html#details/5F746B9C4DCF6F50486A1CB27BFD4D7E01689EEE) | 2020-08-26   | No          |                    42 |
| [iansh11e](https://metrics.torproject.org/rs.html#details/65BBE89EF47A0440A72402C40645C9315ADD55F8)  | 2020-07-08   | No          |                    42 |
| [iansh3e](https://metrics.torproject.org/rs.html#details/670507CA6CF7697E6027728CC28BB0AEF1DE1E7C)   | 2020-07-04   | No          |                    42 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/6DCDE835D65C0CC5F8523B42C9FBB7D130E1472D) | 2020-07-30   | No          |                    42 |
| [iansh7e](https://metrics.torproject.org/rs.html#details/73C4C4AE90A8F83D3A091B395C7D5B913D50604D)   | 2020-07-05   | No          |                    42 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/7777F9186C01E44F4A55B7300B19D05B9150588C) | 2020-07-10   | No          |                    42 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/78D1C8763DE548839DDA41C95E7796DD43240355) | 2020-07-07   | No          |                    42 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/7AF8C3C1E0E93D2B9E07C2663DE45B6DF28ED38B) | 2020-07-30   | No          |                    42 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/845C551529FDF63E6FB8C6802F1DF35998DB0FEC) | 2020-07-30   | No          |                    42 |
| [iansh7e](https://metrics.torproject.org/rs.html#details/889C9C1821CAB437ABAA9286E07D3141179F043A)   | 2020-07-05   | No          |                    42 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/92BE02DD3B76061222898FA81268C074046846E9) | 2020-07-30   | No          |                    42 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/A14993020CC672AE519B1F1C9679CE0982C9733F) | 2020-07-30   | No          |                    42 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/A8B44F6FFBDF35F7B0ED6C17E1FD2EDC34F244E9) | 2020-07-10   | No          |                    42 |
| [iansh15fe](https://metrics.torproject.org/rs.html#details/A9B7059C582AB54AF1BE9E4822405312BDC2A9E5) | 2020-08-26   | No          |                    42 |
| [iansh6e](https://metrics.torproject.org/rs.html#details/B0B0D34D0C207589B54D514E8F3AD1D1C6C014CB)   | 2020-07-05   | No          |                    42 |
| [iansh2e](https://metrics.torproject.org/rs.html#details/B0B85C0C0E7B621D0B7BF17FDA0427F3640691FA)   | 2020-07-04   | No          |                    42 |
| [iansh16de](https://metrics.torproject.org/rs.html#details/B817870AE4F844407C21A5519126D619D07726CB) | 2020-08-26   | No          |                     1 |
| [iansh4e](https://metrics.torproject.org/rs.html#details/C554F4F1EF719D33AA612457960C889F1FB64A4B)   | 2020-07-04   | No          |                    42 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/C866C38DA2D102CD88E138F0AF3A9D6B72606730) | 2020-07-15   | No          |                    42 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/D565D581498D9DBA9AF66DC93919157835B8759C) | 2020-07-10   | No          |                    42 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/D76C97B6116E7A153B67B77B656F9C5E8D65D3C1) | 2020-07-30   | No          |                    42 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/D7FE95EA78176F3F8566A7498A928E53D19DFAE5) | 2020-07-07   | No          |                    42 |
| [iansh6e](https://metrics.torproject.org/rs.html#details/D937890C0A73F83E42FEDE3CA8B1BA80A59A29C0)   | 2020-07-05   | No          |                    42 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/E0C3346EBDB9746185D574B92E503DC9AEB160BE) | 2020-07-30   | No          |                    42 |
| [iansh16de](https://metrics.torproject.org/rs.html#details/EC92228D30A32A7D31DFA166BFDBDBCFD24D72B2) | 2020-08-26   | No          |                     1 |
| [iansh16de](https://metrics.torproject.org/rs.html#details/F8875652863BD2E849CC6775AFA141EB64665962) | 2020-08-26   | No          |                     1 |
| [iansh16de](https://metrics.torproject.org/rs.html#details/FB9CE06785861289B9B03A2B87FF25CDFC81609A) | 2020-08-26   | No          |                     1 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/FEA045FF57EE6A7E318DAF72AF916B5F8B0F4997) | 2020-07-30   | No          |                    42 |


## Fingerprint List of Guard-only Relays in E2E Groups

0B841CB70F9ED1FD0322C2BA2EB0D80420D87CFA,1685E8A79D1D01E4FBC135CD91341C4A4ED802E6,20CD933EDC7260B19040475B24FD6B01B73E94BB,3B4C5729F829CA2E895B81AF834A63DB336D0FFE,438DC9B6B5C5375D332BB338D7E5C1B9EF448960,4F500157ABF70A1A94636D268A742A8B227B8BFD,4FDDFAD51B24DDABB62FB59071F4DC421E76C685,53134D9637D9FBE565FA1E3AF82B23CC964C56D6,5D765770B4DB110D88787457978AB4008CF65CAC,62712B2C24A169B24336CD2FE2BE55DA67476C8B,650FF4A32965D378A55D42A29F6FD1CE914959D3,6A8B54FB9F79E33A307AD0319B62916504A28049,71539D1911ECB826069A4D156771AC4F9F4632A7,91E7CA6B8D0AAD77C7CFB8FEA25BF4F46DA1042A,929BB84A68198CE35E2F2828812840AF5C2CBC4A,937F201D2797314953F268D252F5C98D3FA9F71E,98138DFD3E2C8C89D8F5AB11EF9B6BFF272D83B4,C303038FDCC72805A160FF64E994333A49ECDA71,C8C46E3E4F00A92C344B367E45F9D63EBB831DE1,D2F16CBF1BD891968D65D44CD21507E3371279F3,FEE41B4BC3056FD2B3BF04E20CAC5AD3904CD5AD