---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

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


## ContactInfo: yscoder@foxmail.com (3) {#yscoderfoxmailcom}

| Nickname                                                                                          | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [keepongoing](https://atlas.torproject.org/#details/D844412187933013C9D36F32AC279D72945F0BD0)     | 2017-05-31   | Yes         |                     1 |
| [xietongguanguan](https://atlas.torproject.org/#details/1D5DD271A465B227B35526FA0A82658BDDF9680E) | 2017-06-08   | No          |                     1 |
| [xietongguan](https://atlas.torproject.org/#details/C567E7F2CC9335ECED038FE564A64974B9E2BC88)     | 2017-06-08   | No          |                     1 |

## ContactInfo: George Shuklin &lt;george.shuklin@gmail.com&gt; (2) {#george-shuklin-georgeshuklingmailcom}

| Nickname                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NSA42](https://atlas.torproject.org/#details/20198F4E1A0E23F32C6265DF749BA003DDAF79B1)       | 2016-02-15   | Yes         |                     1 |
| [freeBogatov](https://atlas.torproject.org/#details/CB6FF27F3A474F6A67D20683C9C97DC275F2658F) | 2016-07-21   | No          |                     1 |

## ContactInfo: visualbasic033@gmail.com (3) {#visualbasic033gmailcom}

| Nickname                                                                                    | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [doutreval](https://atlas.torproject.org/#details/CB4EBE9C475A60A5F2CDA92C83CE093BD945D940) | 2015-12-04   | Yes         |                     1 |
| [dlavolos](https://atlas.torproject.org/#details/6E41F9BC3FE626D1897865CE9A9335D09A8DA5FE)  | 2016-03-07   | No          |                     1 |
| [sowinetz](https://atlas.torproject.org/#details/A041B285B228241C3185483EEF42F0BC96D40BFB)  | 2016-08-08   | No          |                     1 |

## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; BTC: 1KogNv (4) {#neel-chauhan-neel-at-neelc-dot-org--btc-1kognv}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay2](https://atlas.torproject.org/#details/D5B8C38539C509380767D4DE20DE84CF84EE8299)     | 2016-09-05   | Yes         |                     3 |
| [NeelTorRelay1](https://atlas.torproject.org/#details/A20840A16CB658024B0D3A0E3F19A9C0E34C843F)     | 2017-01-17   | Yes         |                     4 |
| [NeelTorExitUSWest](https://atlas.torproject.org/#details/0D8211D34F29F51D690303E319766E1B7C28BADB) | 2017-05-25   | No          |                     3 |
| [NeelTorExitCZ](https://atlas.torproject.org/#details/1602E42D1DE3C7B3EF042F357F906DE55FA6C7C6)     | 2016-08-10   | No          |                     4 |


## Fingerprint List of Guard-only Relays in E2E Groups

20198F4E1A0E23F32C6265DF749BA003DDAF79B1,CB4EBE9C475A60A5F2CDA92C83CE093BD945D940,D844412187933013C9D36F32AC279D72945F0BD0,A20840A16CB658024B0D3A0E3F19A9C0E34C843F,D5B8C38539C509380767D4DE20DE84CF84EE8299