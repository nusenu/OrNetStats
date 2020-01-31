---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-01-30 17:00 UTC**

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


## ContactInfo: Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w (16) {#nicholas-merrill-nick-at-calyx-dot-com-btc---14w}

| Nickname                                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CalyxInstitute07](https://metrics.torproject.org/rs.html#details/1B9FACF25E17D26E307EA7CFA7D455B144B032E5) | 2013-11-05   | Yes         |                    13 |
| [CalyxInstitute14](https://metrics.torproject.org/rs.html#details/0011BD2485AD45D984EC4159C88FC066E5E3300E) | 2014-12-23   | No          |                    13 |
| [CalyxInstitute08](https://metrics.torproject.org/rs.html#details/0B5E5E70FFEA9C7F9FFD13B8E16916A608F3E9EB) | 2013-11-12   | No          |                    13 |
| [CalyxInstitute10](https://metrics.torproject.org/rs.html#details/42ED91DD3768F6A2A194D094A7432CBE8DA004B1) | 2016-04-01   | No          |                    13 |
| [CalyxInstitute15](https://metrics.torproject.org/rs.html#details/47E49319DD67784F1E65B5793371BE467365979E) | 2015-08-21   | No          |                    13 |
| [CalyxInstitute04](https://metrics.torproject.org/rs.html#details/501B3DBF250B094A05CA5DBC424AD4C3D46721A2) | 2013-07-08   | No          |                    13 |
| [CalyxInstitute11](https://metrics.torproject.org/rs.html#details/6C143720FFF8469EF6A5C5B4066366340CF6C0D1) | 2014-11-24   | No          |                    13 |
| [CalyxInstitute06](https://metrics.torproject.org/rs.html#details/6F4E9FD00D4251D98BE96FB1AA546FE34676A95B) | 2013-11-23   | No          |                    13 |
| [CalyxInstitute09](https://metrics.torproject.org/rs.html#details/7761DDC7EB1BE26D4155F74A15F12C32A36FE0F2) | 2013-11-19   | No          |                    13 |
| [CalyxInstitute17](https://metrics.torproject.org/rs.html#details/81EDFBC8F6F5C7CF0ADD5F8E08BC8FABA04089C6) | 2020-01-30   | No          |                     1 |
| [CalyxInstitute03](https://metrics.torproject.org/rs.html#details/84D361B736A8CD1E8818D0FC186892E91AB76881) | 2013-06-23   | No          |                    13 |
| [CalyxInstitute12](https://metrics.torproject.org/rs.html#details/B34CC9056250847D1980F08285B01CF0B718C0B6) | 2014-12-16   | No          |                    13 |
| [CalyxInstitute01](https://metrics.torproject.org/rs.html#details/E4D1F25DFBE484208866BA4A1A958B73127CB0AD) | 2013-06-11   | No          |                    13 |
| [CalyxInstitute19](https://metrics.torproject.org/rs.html#details/E8663924FE2AAD4E081A17ED6976D0AE8010F47B) | 2020-01-30   | No          |                     1 |
| [CalyxInstitute18](https://metrics.torproject.org/rs.html#details/EDEDB8797873D340328B5FEDBD7744A7D1DF151F) | 2020-01-30   | No          |                     1 |
| [CalyxInstitute16](https://metrics.torproject.org/rs.html#details/F68A76522D356F89BEC286889A3822250567BE2E) | 2020-01-28   | No          |                     1 |

## ContactInfo: &lt;hostmaster at denetron dot com&gt; (2) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://metrics.torproject.org/rs.html#details/DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4) | 2019-10-25   | Yes         |                     1 |
| [Apollo](https://metrics.torproject.org/rs.html#details/71840F45C2478347B872321066F9805D1A1B79FD)  | 2019-10-25   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

1B9FACF25E17D26E307EA7CFA7D455B144B032E5,DF81D831D4FF686F52C9ACAA9EB5711F95BF4DD4