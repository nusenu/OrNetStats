---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-04-13 19:00 UTC**

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


## ContactInfo: abuse at yggdrasil dot ws url:yggdrasil.ws proof:u (21) {#abuseatyggdrasildotws-urlyggdrasilws-proofu}

| Nickname                                                                                                | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Odin](https://metrics.torproject.org/rs.html#details/15B1F023B0C16A608E89F867D96856AC8D2F0048)         | 2022-02-17   | Yes         |                    21 |
| [Heidrun](https://metrics.torproject.org/rs.html#details/0071933EB152FD69EE909A90B1084DFDE91FC988)      | 2022-03-16   | No          |                    21 |
| [Fenrir](https://metrics.torproject.org/rs.html#details/02326DAE399F3A6A829B7A65348F191B77282AB9)       | 2022-03-31   | No          |                     1 |
| [Gullinborsti](https://metrics.torproject.org/rs.html#details/24362E7E61E6D72FE70262C8C11D5035712D56B8) | 2022-03-08   | No          |                    21 |
| [Loki](https://metrics.torproject.org/rs.html#details/2A88B370BC0519F80E930A3776579E59B7383B08)         | 2022-02-22   | No          |                    21 |
| [Ymir](https://metrics.torproject.org/rs.html#details/4AA0035604DF40E5BA20DBE88EF6D11432421BFA)         | 2020-10-27   | No          |                    21 |
| [Freya](https://metrics.torproject.org/rs.html#details/4BE441A6F75DEA5C738C91655418D3F9845B2143)        | 2022-02-21   | No          |                    21 |
| [Hugin](https://metrics.torproject.org/rs.html#details/4E533D0E42D41968875911C419A9BA265EFA9883)        | 2019-12-02   | No          |                    21 |
| [Ganymed](https://metrics.torproject.org/rs.html#details/5AFF7583F5ED62A274823C83199F2E19083692EC)      | 2020-08-20   | No          |                    21 |
| [Asgard](https://metrics.torproject.org/rs.html#details/5C8AB2BC9588553948BE931B5374B98EC5760650)       | 2022-03-08   | No          |                    21 |
| [Ragnarok](https://metrics.torproject.org/rs.html#details/7B077965A032FEE91F8DDFD3F18F9943398AAE3F)     | 2022-02-01   | No          |                    21 |
| [Gimli](https://metrics.torproject.org/rs.html#details/7DA4235E725388111A6BDD965742A9E58A7D1451)        | 2022-02-21   | No          |                    20 |
| [Njord](https://metrics.torproject.org/rs.html#details/869CB6932EF87DC152D6B12BDFE5C82677975E79)        | 2022-04-09   | No          |                     1 |
| [Heimdall](https://metrics.torproject.org/rs.html#details/8C9347D033ED0E7B2D57C1DA9028AE8F152ADD48)     | 2022-02-21   | No          |                    21 |
| [Frigg](https://metrics.torproject.org/rs.html#details/98EC17CE329197A4A81C2B122806CE9E315A7518)        | 2022-02-22   | No          |                    21 |
| [Tyr](https://metrics.torproject.org/rs.html#details/9CD41AC4F0054E9A8452732F86BD8D84FC812572)          | 2022-02-21   | No          |                    21 |
| [Hildisvini](https://metrics.torproject.org/rs.html#details/9CD42CD6B94B7CEED2B915491EA6457ABD8E5675)   | 2022-03-16   | No          |                    21 |
| [Thor](https://metrics.torproject.org/rs.html#details/A6A45A07C3AF4F37F6ADAFB5BCEE7E42D44A3899)         | 2022-04-13   | No          |                     1 |
| [Gulltopp](https://metrics.torproject.org/rs.html#details/C0DC5DC08B91A5A17BF530E33F02FF4236ADE001)     | 2022-03-16   | No          |                    21 |
| [Moona](https://metrics.torproject.org/rs.html#details/C58FA99811371C688012A5DE427685B62C778FE9)        | 2022-03-16   | No          |                    21 |
| [Vale](https://metrics.torproject.org/rs.html#details/E2FECC8FDBA00078C2820129518D9E18C2148952)         | 2022-03-06   | No          |                    20 |

## ContactInfo: &lt;nobody AT example dot com&gt; (2) {#nobody-at-example-dot-com}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [node01](https://metrics.torproject.org/rs.html#details/D53AE170BF6650A2C6640484FE1B5DD1C0AB895B)   | 2019-12-14   | Yes         |                     1 |
| [giovanna](https://metrics.torproject.org/rs.html#details/1137AB1F84EC2D52DFB1915717F14FF1A10EB392) | 2018-11-22   | No          |                     1 |

## ContactInfo: tor at p073 dot nl (2) {#toratp073dotnl}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [LAYLOtor02](https://metrics.torproject.org/rs.html#details/B8ADD5706960E26810345BDA1FEB7771FDCE3A5E) | 2022-03-01   | Yes         |                     1 |
| [LAYLOtor01](https://metrics.torproject.org/rs.html#details/EF02EF768B54E29C50D13E6589FF82FFD7791F0B) | 2022-03-27   | No          |                     1 |

## ContactInfo: tor-operator@your-emailaddress-domain (4) {#tor-operatoryour-emailaddress-domain}

| Nickname                                                                                                       | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [anotherRelay](https://metrics.torproject.org/rs.html#details/F6691E3EB7CAB3C876AAA885E6801B63DC998C39)        | 2018-10-29   | Yes         |                     1 |
| [myNiceBionicRelay](https://metrics.torproject.org/rs.html#details/D90A78790098F7C0639DC2D3A8016948EAE5E2B1)   | 2021-10-14   | Yes         |                     1 |
| [emandeman44678gudno](https://metrics.torproject.org/rs.html#details/1939469D1E898F7674A55F09BE46EE9742C33FA4) | 2022-01-31   | Yes         |                     1 |
| [SpiralExitRelay](https://metrics.torproject.org/rs.html#details/824E2894713F8249B7C2735176BE0564BD1ED5B7)     | 2022-04-08   | No          |                     1 |

## ContactInfo: gusntwrk.xyz (2) {#gusntwrkxyz}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [elhombre](https://metrics.torproject.org/rs.html#details/D7910C73B9092697D7D2AF14E5CA09112F0C6EA9) | 2021-12-11   | Yes         |                     1 |
| [rknchan](https://metrics.torproject.org/rs.html#details/A5B984C20AF47731B911CDF68032A36F8678C25B)  | 2022-02-19   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

15B1F023B0C16A608E89F867D96856AC8D2F0048,B8ADD5706960E26810345BDA1FEB7771FDCE3A5E,1939469D1E898F7674A55F09BE46EE9742C33FA4,D53AE170BF6650A2C6640484FE1B5DD1C0AB895B,F6691E3EB7CAB3C876AAA885E6801B63DC998C39,D7910C73B9092697D7D2AF14E5CA09112F0C6EA9