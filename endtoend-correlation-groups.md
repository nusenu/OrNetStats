---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2017-12-27 13:00 UTC**

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


## ContactInfo: https://www.torservers.net/donate.html &lt;support .A (11) {#httpswwwtorserversnetdonatehtml-support-a}

| Nickname                                                                                         | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [hackeriet1](https://atlas.torproject.org/#details/E379A6CACEFAFE1B8EA68503BFCFF1215BF1EE7F)     | 2015-12-02   | Yes         |                     1 |
| [criticalmass](https://atlas.torproject.org/#details/1D3174338A1131A53E098443E76E1103CDED00DC)   | 2016-12-30   | No          |                    12 |
| [HaveHeart](https://atlas.torproject.org/#details/204DFD2A2C6A0DC1FA0EACB495218E0B661704FD)      | 2017-10-03   | No          |                    12 |
| [amazonas](https://atlas.torproject.org/#details/5974B3F4C66D83BBC9622E0F0F023FE48428DB9B)       | 2017-11-01   | No          |                    12 |
| [CriticalMass](https://atlas.torproject.org/#details/77131D7E2EC1CA9B8D737502256DA9103599CE51)   | 2017-10-03   | No          |                    12 |
| [sofia](https://atlas.torproject.org/#details/7BFB908A3AA5B491DA4CA72CCBEE0E1F2A939B55)          | 2017-10-03   | No          |                    12 |
| [amartysen](https://atlas.torproject.org/#details/8EF8766E1645A41A2AE1565EB673A4957C8D5AD2)      | 2017-11-01   | No          |                    12 |
| [iVPN](https://atlas.torproject.org/#details/A2534EF23390CAE079B1586F0FDF9CE11F556062)           | 2016-12-30   | No          |                    12 |
| [HSLtor](https://atlas.torproject.org/#details/E43A346CB81DDF364B6FF68235AFADBA0E8692B8)         | 2017-01-22   | No          |                    12 |
| [freeBogatov](https://atlas.torproject.org/#details/F4594608272C82407E9D137F1AE89A408CCFD285)    | 2017-11-01   | No          |                    12 |
| [dorrisdeebrown](https://atlas.torproject.org/#details/FDAED15C98CFE7A416E5676F614254F78406105C) | 2016-12-23   | No          |                    12 |

## ContactInfo: Nicholas Merrill &lt;nick AT calyx dot com&gt; 14wntQ8cB (12) {#nicholas-merrill-nick-at-calyx-dot-com-14wntq8cb}

| Nickname                                                                                           | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [CalyxInstitute07](https://atlas.torproject.org/#details/1B9FACF25E17D26E307EA7CFA7D455B144B032E5) | 2013-11-05   | Yes         |                    12 |
| [CalyxInstitute10](https://atlas.torproject.org/#details/42ED91DD3768F6A2A194D094A7432CBE8DA004B1) | 2016-04-01   | Yes         |                     4 |
| [CalyxInstitute14](https://atlas.torproject.org/#details/0011BD2485AD45D984EC4159C88FC066E5E3300E) | 2014-12-23   | No          |                    13 |
| [CalyxInstitute08](https://atlas.torproject.org/#details/0B5E5E70FFEA9C7F9FFD13B8E16916A608F3E9EB) | 2013-11-12   | No          |                    12 |
| [CalyxInstitute15](https://atlas.torproject.org/#details/47E49319DD67784F1E65B5793371BE467365979E) | 2015-08-21   | No          |                    12 |
| [CalyxInstitute11](https://atlas.torproject.org/#details/6C143720FFF8469EF6A5C5B4066366340CF6C0D1) | 2014-11-24   | No          |                    13 |
| [CalyxInstitute06](https://atlas.torproject.org/#details/6F4E9FD00D4251D98BE96FB1AA546FE34676A95B) | 2013-11-23   | No          |                    12 |
| [CalyxInstitute09](https://atlas.torproject.org/#details/7761DDC7EB1BE26D4155F74A15F12C32A36FE0F2) | 2013-11-19   | No          |                    12 |
| [CalyxInstitute03](https://atlas.torproject.org/#details/84D361B736A8CD1E8818D0FC186892E91AB76881) | 2013-06-23   | No          |                    12 |
| [CalyxInstitute13](https://atlas.torproject.org/#details/A7C7EB2A0DFB2E3FFFC12B7756707433DD550F9E) | 2014-12-20   | No          |                    13 |
| [CalyxInstitute12](https://atlas.torproject.org/#details/B34CC9056250847D1980F08285B01CF0B718C0B6) | 2014-12-16   | No          |                    12 |
| [CalyxInstitute01](https://atlas.torproject.org/#details/E4D1F25DFBE484208866BA4A1A958B73127CB0AD) | 2013-06-11   | No          |                    12 |

## ContactInfo: AnonyMaid Team &lt;info@anonymaid.net&gt; (3) {#anonymaid-team-infoanonymaidnet}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [DutchDroid](https://atlas.torproject.org/#details/BF5068641A54A9433CA612BDFF7F098B72EB9762)  | 2017-08-09   | Yes         |                     1 |
| [DutchMaid04](https://atlas.torproject.org/#details/44182447E5E9F2997754CE53FFB4881942B5B3C6) | 2017-10-01   | No          |                     1 |
| [DutchMaid03](https://atlas.torproject.org/#details/7FAB8FED1A821455902BEA3388A6DA5BF6F78198) | 2017-10-01   | No          |                     1 |

## ContactInfo: Digineo GmbH &lt;tor AT digineo dot de&gt; (2) {#digineo-gmbh-tor-at-digineo-dot-de}

| Nickname                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [digineo2](https://atlas.torproject.org/#details/C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7) | 2014-05-29   | Yes         |                     1 |
| [digineo3](https://atlas.torproject.org/#details/B21211A1A2C68F2D9E57E3C7AEAF4F04AFC10E7F) | 2017-02-16   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

C0A05D6DC0987D0BF32F0FF00A9BF791E7CA79D7,BF5068641A54A9433CA612BDFF7F098B72EB9762,E379A6CACEFAFE1B8EA68503BFCFF1215BF1EE7F