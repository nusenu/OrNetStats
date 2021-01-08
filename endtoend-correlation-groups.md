---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-01-08 19:00 UTC**

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


## ContactInfo: Privex Inc. https://www.privex.io (3) {#privex-inc-httpswwwprivexio}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [privexrelayde1](https://metrics.torproject.org/rs.html#details/C64EB4553AA308D8FBC314D73B44178E4CB11C35)  | 2020-11-22   | Yes         |                     2 |
| [privexrelayfin1](https://metrics.torproject.org/rs.html#details/C3ACB0492A644E27A549BC3CDF3B7A129186E3BF) | 2018-09-27   | Yes         |                     3 |
| [privexse1exit](https://metrics.torproject.org/rs.html#details/D8A1F5A8EA1AF53E3414B9C48FE6B10C31ACC9B2)   | 2019-06-26   | No          |                     2 |

## ContactInfo: shebangs@yopmail.fr (15) {#shebangsyopmailfr}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Shebangs](https://metrics.torproject.org/rs.html#details/A4A79E2B8294AA2572B46C5C772E149F84FAF763) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/453E51CBAA4C2169EBCB05583247DD6201E87FAD) | 2020-06-05   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/F5F9B6B40E4D7AFCECDFB1F4503D56D522C7EFAA) | 2020-09-13   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/F3A3461889BF97250F50A7BAAAE4A2B92062F6D7) | 2020-07-03   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/BA8546AE9B27F0C81F98A6C12D96B7DAB0814991) | 2020-06-06   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/CEA2E066A7F8EC0F235F5190E25DD3C9F86F084B) | 2020-06-06   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/E4A8BC82E660528D5B0B8D36C08AB44B77351736) | 2020-12-17   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/AC990FD1FF5058EFA43A809E948B23EF998D021B) | 2020-06-05   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/328ED3A92D1CD621659B4DA6E210FCAED813174B) | 2020-12-20   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/C8B5B2186A2DED8F419EAA933EFB5FFE2D412CF4) | 2020-09-25   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/0794E378A1EE9337D917BEE88607A1C12AC7F906) | 2020-10-03   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/072E4EC47D640118D5438BFFDFF1AF7BB4E2AD2B) | 2020-10-05   | Yes         |                    12 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/60D12B7D7A601622504F74C9A4EB7C8F33FE5C84) | 2020-12-29   | Yes         |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/5A8918BCA6B05FC780CFBDD66703BEF60DE53DA6) | 2020-12-25   | No          |                     1 |
| [Shebangs](https://metrics.torproject.org/rs.html#details/E9272A28DAFABAE4F3D07233A16D13BDD5F58D4A) | 2020-12-25   | No          |                     1 |

## ContactInfo: Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w (20) {#nicholas-merrill-nick-at-calyx-dot-com-btc---14w}

| Nickname                                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CalyxInstitute07](https://metrics.torproject.org/rs.html#details/1B9FACF25E17D26E307EA7CFA7D455B144B032E5) | 2013-11-05   | Yes         |                    20 |
| [CalyxInstitute14](https://metrics.torproject.org/rs.html#details/0011BD2485AD45D984EC4159C88FC066E5E3300E) | 2014-12-23   | No          |                    20 |
| [CalyxInstitute08](https://metrics.torproject.org/rs.html#details/0B5E5E70FFEA9C7F9FFD13B8E16916A608F3E9EB) | 2013-11-12   | No          |                    20 |
| [CalyxInstitute10](https://metrics.torproject.org/rs.html#details/42ED91DD3768F6A2A194D094A7432CBE8DA004B1) | 2016-04-01   | No          |                    20 |
| [CalyxInstitute15](https://metrics.torproject.org/rs.html#details/47E49319DD67784F1E65B5793371BE467365979E) | 2015-08-21   | No          |                    20 |
| [CalyxInstitute22](https://metrics.torproject.org/rs.html#details/4B218691AF8BC02BAB4D856689652E958AF5DCF3) | 2020-12-03   | No          |                     1 |
| [CalyxInstitute04](https://metrics.torproject.org/rs.html#details/501B3DBF250B094A05CA5DBC424AD4C3D46721A2) | 2013-07-08   | No          |                    20 |
| [CalyxInstitute20](https://metrics.torproject.org/rs.html#details/673C081A9502D5D3AB9395FF4257274BE4C7A8A4) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute11](https://metrics.torproject.org/rs.html#details/6C143720FFF8469EF6A5C5B4066366340CF6C0D1) | 2014-11-24   | No          |                    20 |
| [CalyxInstitute06](https://metrics.torproject.org/rs.html#details/6F4E9FD00D4251D98BE96FB1AA546FE34676A95B) | 2013-11-23   | No          |                    20 |
| [CalyxInstitute21](https://metrics.torproject.org/rs.html#details/70ACA07D9276277B82E909C1439E19CCA2FB16CC) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute09](https://metrics.torproject.org/rs.html#details/7761DDC7EB1BE26D4155F74A15F12C32A36FE0F2) | 2013-11-19   | No          |                    20 |
| [CalyxInstitute17](https://metrics.torproject.org/rs.html#details/81EDFBC8F6F5C7CF0ADD5F8E08BC8FABA04089C6) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute03](https://metrics.torproject.org/rs.html#details/84D361B736A8CD1E8818D0FC186892E91AB76881) | 2013-06-23   | No          |                    20 |
| [CalyxInstitute13](https://metrics.torproject.org/rs.html#details/A7C7EB2A0DFB2E3FFFC12B7756707433DD550F9E) | 2014-12-20   | No          |                    20 |
| [CalyxInstitute12](https://metrics.torproject.org/rs.html#details/B34CC9056250847D1980F08285B01CF0B718C0B6) | 2014-12-16   | No          |                    20 |
| [CalyxInstitute01](https://metrics.torproject.org/rs.html#details/E4D1F25DFBE484208866BA4A1A958B73127CB0AD) | 2013-06-11   | No          |                    20 |
| [CalyxInstitute19](https://metrics.torproject.org/rs.html#details/E8663924FE2AAD4E081A17ED6976D0AE8010F47B) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute18](https://metrics.torproject.org/rs.html#details/EDEDB8797873D340328B5FEDBD7744A7D1DF151F) | 2020-01-30   | No          |                    20 |
| [CalyxInstitute16](https://metrics.torproject.org/rs.html#details/F68A76522D356F89BEC286889A3822250567BE2E) | 2020-01-28   | No          |                    20 |


## Fingerprint List of Guard-only Relays in E2E Groups

C3ACB0492A644E27A549BC3CDF3B7A129186E3BF,C64EB4553AA308D8FBC314D73B44178E4CB11C35,072E4EC47D640118D5438BFFDFF1AF7BB4E2AD2B,0794E378A1EE9337D917BEE88607A1C12AC7F906,328ED3A92D1CD621659B4DA6E210FCAED813174B,3688001D75469101F74A5D551A49B0EF410F0E26,453E51CBAA4C2169EBCB05583247DD6201E87FAD,60D12B7D7A601622504F74C9A4EB7C8F33FE5C84,A4A79E2B8294AA2572B46C5C772E149F84FAF763,AC990FD1FF5058EFA43A809E948B23EF998D021B,BA8546AE9B27F0C81F98A6C12D96B7DAB0814991,C8B5B2186A2DED8F419EAA933EFB5FFE2D412CF4,CEA2E066A7F8EC0F235F5190E25DD3C9F86F084B,E4A8BC82E660528D5B0B8D36C08AB44B77351736,F3A3461889BF97250F50A7BAAAE4A2B92062F6D7,F5F9B6B40E4D7AFCECDFB1F4503D56D522C7EFAA,1B9FACF25E17D26E307EA7CFA7D455B144B032E5