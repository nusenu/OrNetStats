---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-11-12 13:00 UTC**

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


## ContactInfo: TheSloth tor &lt;at&gt; slothbucks &lt;dot&gt; net (3) {#thesloth-tor-at-slothbucks-dot--net}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [LucoaKobayashi](https://metrics.torproject.org/rs.html#details/CF072FA81CFC075DA9675DC01394DB580E28958E) | 2022-10-25   | Yes         |                     1 |
| [KannaKobayashi](https://metrics.torproject.org/rs.html#details/B97019FB96C21598057A6A6D87B4C49CFB08C348) | 2022-10-03   | Yes         |                     1 |
| [TohruKobayashi](https://metrics.torproject.org/rs.html#details/D19AFD75C4B098FAAB3F94BD42CAD1607F75FD60) | 2022-10-03   | No          |                     1 |

## ContactInfo: tor-relay-admin@carlos1001.com (2) {#tor-relay-admincarlos1001com}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [carlos1001](https://metrics.torproject.org/rs.html#details/299CC5D7A58E5B92B69DC333B28D926CD7B157D8) | 2021-05-12   | Yes         |                     1 |
| [orion01](https://metrics.torproject.org/rs.html#details/0E0AF3656F3F7914752E013C10E7F46C651BA820)    | 2022-11-05   | No          |                     1 |

## ContactInfo: cam632@gmx.com (2) {#cam632gmxcom}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Praktiker](https://metrics.torproject.org/rs.html#details/E99A1B54541518A8A6058D75762497AE0D3442DC) | 2022-09-23   | Yes         |                     1 |
| [Boro](https://metrics.torproject.org/rs.html#details/5F4BCBC6E20AE074340D0A743E6F2EA4B51B09C1)      | 2022-08-31   | No          |                     1 |

## ContactInfo: 96001reddit at protonmail dot com (2) {#96001redditatprotonmaildotcom}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [RelaysOfBabylon](https://metrics.torproject.org/rs.html#details/0C29BDA07390E89AC6DA4775FB102A1B8183F6C2) | 2022-09-20   | Yes         |                     1 |
| [imboredrelay](https://metrics.torproject.org/rs.html#details/654B364C24573B4631C8AD7C39C161C568C04A3C)    | 2022-09-14   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

B97019FB96C21598057A6A6D87B4C49CFB08C348,CF072FA81CFC075DA9675DC01394DB580E28958E,299CC5D7A58E5B92B69DC333B28D926CD7B157D8,E99A1B54541518A8A6058D75762497AE0D3442DC,0C29BDA07390E89AC6DA4775FB102A1B8183F6C2