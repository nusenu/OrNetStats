---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-01-17 08:00 UTC**

For each operator the list of running relays is shown (relays are linked to [Atlas](https://atlas.torproject.org)).
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


## ContactInfo: &lt;hostmaster at denetron dot com&gt; (3) {#hostmaster-at-denetron-dot-com}

| Nickname                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Voyager](https://atlas.torproject.org/#details/AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16) | 2016-08-28   | Yes         |                     2 |
| [Mercury](https://atlas.torproject.org/#details/484CEAF51A37EC992645FB6257B2EBC4AE20D9B7) | 2014-10-05   | No          |                     1 |
| [Apollo](https://atlas.torproject.org/#details/9A630383897133B05DB56532ECC91214CF195F68)  | 2016-03-16   | No          |                     2 |

## ContactInfo: Nicholas Merrill &lt;nick AT calyx dot com&gt; BTC - 14w (12) {#nicholas-merrill-nick-at-calyx-dot-com-btc---14w}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CalyxInstitute07](https://atlas.torproject.org/#details/1B9FACF25E17D26E307EA7CFA7D455B144B032E5) | 2013-11-05   | Yes         |                    12 |
| [CalyxInstitute10](https://atlas.torproject.org/#details/42ED91DD3768F6A2A194D094A7432CBE8DA004B1) | 2016-04-01   | Yes         |                     4 |
| [CalyxInstitute14](https://atlas.torproject.org/#details/0011BD2485AD45D984EC4159C88FC066E5E3300E) | 2014-12-23   | No          |                    13 |
| [CalyxInstitute08](https://atlas.torproject.org/#details/0B5E5E70FFEA9C7F9FFD13B8E16916A608F3E9EB) | 2013-11-12   | No          |                    12 |
| [CalyxInstitute15](https://atlas.torproject.org/#details/47E49319DD67784F1E65B5793371BE467365979E) | 2015-08-21   | No          |                    12 |
| [CalyxInstitute04](https://atlas.torproject.org/#details/501B3DBF250B094A05CA5DBC424AD4C3D46721A2) | 2013-07-08   | No          |                    12 |
| [CalyxInstitute11](https://atlas.torproject.org/#details/6C143720FFF8469EF6A5C5B4066366340CF6C0D1) | 2014-11-24   | No          |                    13 |
| [CalyxInstitute06](https://atlas.torproject.org/#details/6F4E9FD00D4251D98BE96FB1AA546FE34676A95B) | 2013-11-23   | No          |                    12 |
| [CalyxInstitute09](https://atlas.torproject.org/#details/7761DDC7EB1BE26D4155F74A15F12C32A36FE0F2) | 2013-11-19   | No          |                    12 |
| [CalyxInstitute13](https://atlas.torproject.org/#details/A7C7EB2A0DFB2E3FFFC12B7756707433DD550F9E) | 2014-12-20   | No          |                    13 |
| [CalyxInstitute12](https://atlas.torproject.org/#details/B34CC9056250847D1980F08285B01CF0B718C0B6) | 2014-12-16   | No          |                    12 |
| [CalyxInstitute01](https://atlas.torproject.org/#details/E4D1F25DFBE484208866BA4A1A958B73127CB0AD) | 2013-06-11   | No          |                    12 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://atlas.torproject.org/#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://atlas.torproject.org/#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7,AE75A16A33040CA8A25D3BEFB66BE94F92FBCC16,1B9FACF25E17D26E307EA7CFA7D455B144B032E5,42ED91DD3768F6A2A194D094A7432CBE8DA004B1