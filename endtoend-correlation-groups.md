---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-10-03 07:00 UTC**

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


## ContactInfo: tor-operator@your-emailaddress-domain (7) {#tor-operatoryour-emailaddress-domain}

| Nickname                                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [demeter](https://metrics.torproject.org/rs.html#details/97B7BA747B62A9962DEDCE404FF33106D4032F91)            | 2020-05-05   | Yes         |                     1 |
| [SuchaNiceRelay](https://metrics.torproject.org/rs.html#details/93FFDC0C36C316208AC6291DE754D733B4D88A13)     | 2020-04-23   | Yes         |                     1 |
| [Marsu](https://metrics.torproject.org/rs.html#details/1DE8E81240D20D9755B29A8AEA131BE2CD537FB8)              | 2020-01-01   | Yes         |                     1 |
| [anotherRelay](https://metrics.torproject.org/rs.html#details/F6691E3EB7CAB3C876AAA885E6801B63DC998C39)       | 2018-10-29   | Yes         |                     1 |
| [BanderaHuesosochka](https://metrics.torproject.org/rs.html#details/304B186CC793A0BA6E63C2D360C99D500DBDB9E4) | 2020-09-30   | No          |                     1 |
| [aabbcc](https://metrics.torproject.org/rs.html#details/E7C1FAFB7525149A0E911512F511D942BA5EEAAF)             | 2019-05-29   | No          |                     1 |
| [Goodspeed](https://metrics.torproject.org/rs.html#details/F311EFECFF1EA0E05D0B7F35CCF056AB5142B5BE)          | 2020-09-15   | No          |                     1 |

## ContactInfo: ian@ian.sh (50) {#ianiansh}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [iansh9r](https://metrics.torproject.org/rs.html#details/650FF4A32965D378A55D42A29F6FD1CE914959D3)   | 2020-07-05   | Yes         |                    48 |
| [iansh9r](https://metrics.torproject.org/rs.html#details/C8C46E3E4F00A92C344B367E45F9D63EBB831DE1)   | 2020-07-05   | Yes         |                    48 |
| [iansh8r](https://metrics.torproject.org/rs.html#details/6A8B54FB9F79E33A307AD0319B62916504A28049)   | 2020-07-05   | Yes         |                    48 |
| [iansh8r](https://metrics.torproject.org/rs.html#details/D2F16CBF1BD891968D65D44CD21507E3371279F3)   | 2020-07-05   | Yes         |                    48 |
| [iansh19e](https://metrics.torproject.org/rs.html#details/0999DA65DB24513CB0084B967A19E47FC037D08C)  | 2020-10-02   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/0C9D7DB63BE030E5CA32E25606632AEB85840F4C) | 2020-07-15   | No          |                    48 |
| [iansh4e](https://metrics.torproject.org/rs.html#details/0F59911D698D3FFE2433B7AB31362FB1EA10237F)   | 2020-07-04   | No          |                    48 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/32B4A9F85DC6BFE90DF914C4BAEC5F4EAC793897) | 2020-07-10   | No          |                    48 |
| [iansh12e](https://metrics.torproject.org/rs.html#details/3466C887F0F53CA5F65662F601A57F329DB460E9)  | 2020-07-08   | No          |                    48 |
| [iansh14fe](https://metrics.torproject.org/rs.html#details/38E75A7B11DFC76A8FC2964DB5DEDDD96B5A5D9C) | 2020-08-26   | No          |                    48 |
| [iansh17e](https://metrics.torproject.org/rs.html#details/39EC14A9BD010485F9219A9D2FF9F29690260053)  | 2020-10-02   | No          |                    48 |
| [iansh14fe](https://metrics.torproject.org/rs.html#details/3AB1F18F079CEF1A00E37A4531676C4EB2F867A1) | 2020-08-26   | No          |                    48 |
| [iansh3e](https://metrics.torproject.org/rs.html#details/3CF2646DE677C7A4FD5AE513A6AC59101879A90F)   | 2020-07-04   | No          |                    48 |
| [iansh20e](https://metrics.torproject.org/rs.html#details/41D456D7CF52FA16A544633CC586814C51F3AF64)  | 2020-10-02   | No          |                    48 |
| [iansh17e](https://metrics.torproject.org/rs.html#details/428A661B415A055E27A769CC3EAD86DE384312CD)  | 2020-10-02   | No          |                    48 |
| [iansh11e](https://metrics.torproject.org/rs.html#details/462D81E70F753A19C429E31086254DD15034CC9B)  | 2020-07-08   | No          |                    48 |
| [iansh18e](https://metrics.torproject.org/rs.html#details/487EB35B2CF580B8DAE0E8E5730109A52C6FB211)  | 2020-10-02   | No          |                    48 |
| [iansh12e](https://metrics.torproject.org/rs.html#details/4FDC3AE93CD2F81D1B64D94075F6418C06A55314)  | 2020-07-08   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/51D3F56EC4543E191B13E614A298ECBC35BEA92E) | 2020-07-30   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/5333C98E703385743AE931ECC929C5E4B32A0CD0) | 2020-07-30   | No          |                    48 |
| [iansh2e](https://metrics.torproject.org/rs.html#details/5F29C863F69E9C3B7BD1841B3504FD4173BFA475)   | 2020-07-04   | No          |                    48 |
| [iansh15fe](https://metrics.torproject.org/rs.html#details/5F746B9C4DCF6F50486A1CB27BFD4D7E01689EEE) | 2020-08-26   | No          |                    48 |
| [iansh11e](https://metrics.torproject.org/rs.html#details/65BBE89EF47A0440A72402C40645C9315ADD55F8)  | 2020-07-08   | No          |                    48 |
| [iansh3e](https://metrics.torproject.org/rs.html#details/670507CA6CF7697E6027728CC28BB0AEF1DE1E7C)   | 2020-07-04   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/6DCDE835D65C0CC5F8523B42C9FBB7D130E1472D) | 2020-07-30   | No          |                    48 |
| [iansh19e](https://metrics.torproject.org/rs.html#details/719E0BA572DE9CA95C6663BFF44297305C5293EC)  | 2020-10-02   | No          |                    48 |
| [iansh7e](https://metrics.torproject.org/rs.html#details/73C4C4AE90A8F83D3A091B395C7D5B913D50604D)   | 2020-07-05   | No          |                    48 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/7777F9186C01E44F4A55B7300B19D05B9150588C) | 2020-07-10   | No          |                    48 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/78D1C8763DE548839DDA41C95E7796DD43240355) | 2020-07-07   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/7AF8C3C1E0E93D2B9E07C2663DE45B6DF28ED38B) | 2020-07-30   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/845C551529FDF63E6FB8C6802F1DF35998DB0FEC) | 2020-07-30   | No          |                    48 |
| [iansh7e](https://metrics.torproject.org/rs.html#details/889C9C1821CAB437ABAA9286E07D3141179F043A)   | 2020-07-05   | No          |                    48 |
| [iansh21e](https://metrics.torproject.org/rs.html#details/8E8BD142819B954F3A6E3E1AA941E0B4217CE4E3)  | 2020-10-03   | No          |                     1 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/92BE02DD3B76061222898FA81268C074046846E9) | 2020-07-30   | No          |                    48 |
| [iansh18e](https://metrics.torproject.org/rs.html#details/9C69356D254BB5BDA6403F3D3FBF486BDCC798F6)  | 2020-10-02   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/A14993020CC672AE519B1F1C9679CE0982C9733F) | 2020-07-30   | No          |                    48 |
| [iansh20e](https://metrics.torproject.org/rs.html#details/A5490FE201BFA31694884206F4797A6E6A222C50)  | 2020-10-02   | No          |                    48 |
| [iansh21e](https://metrics.torproject.org/rs.html#details/A8A65E73C5C36854FE2CBE3E0196745169BFE6CB)  | 2020-10-03   | No          |                     1 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/A8B44F6FFBDF35F7B0ED6C17E1FD2EDC34F244E9) | 2020-07-10   | No          |                    48 |
| [iansh15fe](https://metrics.torproject.org/rs.html#details/A9B7059C582AB54AF1BE9E4822405312BDC2A9E5) | 2020-08-26   | No          |                    48 |
| [iansh6e](https://metrics.torproject.org/rs.html#details/B0B0D34D0C207589B54D514E8F3AD1D1C6C014CB)   | 2020-07-05   | No          |                    48 |
| [iansh2e](https://metrics.torproject.org/rs.html#details/B0B85C0C0E7B621D0B7BF17FDA0427F3640691FA)   | 2020-07-04   | No          |                    48 |
| [iansh4e](https://metrics.torproject.org/rs.html#details/C554F4F1EF719D33AA612457960C889F1FB64A4B)   | 2020-07-04   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/C866C38DA2D102CD88E138F0AF3A9D6B72606730) | 2020-07-15   | No          |                    48 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/D565D581498D9DBA9AF66DC93919157835B8759C) | 2020-07-10   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/D76C97B6116E7A153B67B77B656F9C5E8D65D3C1) | 2020-07-30   | No          |                    48 |
| [iansh10fe](https://metrics.torproject.org/rs.html#details/D7FE95EA78176F3F8566A7498A928E53D19DFAE5) | 2020-07-07   | No          |                    48 |
| [iansh6e](https://metrics.torproject.org/rs.html#details/D937890C0A73F83E42FEDE3CA8B1BA80A59A29C0)   | 2020-07-05   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/E0C3346EBDB9746185D574B92E503DC9AEB160BE) | 2020-07-30   | No          |                    48 |
| [iansh13fe](https://metrics.torproject.org/rs.html#details/FEA045FF57EE6A7E318DAF72AF916B5F8B0F4997) | 2020-07-30   | No          |                    48 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (2) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4) | 2019-10-25   | Yes         |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/71840F45C2478347B872321066F9805D1A1B79FD)  | 2019-10-25   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

1DE8E81240D20D9755B29A8AEA131BE2CD537FB8,400C053623F36C5C3D1CFC73F1AB9DA6E24DEEB7,4B550F757A5904939280CB85DE61F125A08AE5DE,93FFDC0C36C316208AC6291DE754D733B4D88A13,97B7BA747B62A9962DEDCE404FF33106D4032F91,F6691E3EB7CAB3C876AAA885E6801B63DC998C39,650FF4A32965D378A55D42A29F6FD1CE914959D3,6A8B54FB9F79E33A307AD0319B62916504A28049,C8C46E3E4F00A92C344B367E45F9D63EBB831DE1,D2F16CBF1BD891968D65D44CD21507E3371279F3,DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4