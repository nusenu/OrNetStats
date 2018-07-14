---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-07-14 10:00 UTC**

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


## ContactInfo: pm@dpjp.ru - 1Hr5ALwotveTsEJpxuyox2en6d62ZVedfs (3) {#pmdpjpru---1hr5alwotvetsejpxuyox2en6d62zvedfs}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [dpjp05](https://metrics.torproject.org/rs.html#details/185CFF801E6BE549F675AD61C3FE04104150AE1F)        | 2018-06-22   | Yes         |                     2 |
| [dpjp01TorExit](https://metrics.torproject.org/rs.html#details/69E06EBB2573A4F89330BDF8BC869794A3E10E4D) | 2018-01-13   | Yes         |                     3 |
| [dpjp06TorExit](https://metrics.torproject.org/rs.html#details/C5AFC0EC23AC7FB19067FC4C511316A4CE38C32F) | 2018-04-02   | No          |                     2 |

## ContactInfo: tor at releasing dot fun (3) {#toratreleasingdotfun}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [releasingFun04](https://metrics.torproject.org/rs.html#details/E91FC7ABF7708A584FCFE88DB5CEA083D00E6511) | 2018-07-04   | Yes         |                     1 |
| [releasingFun03](https://metrics.torproject.org/rs.html#details/0644F3CCE5141F679D8509D100E068FFAA531350) | 2018-07-03   | No          |                     3 |
| [releasingFun02](https://metrics.torproject.org/rs.html#details/B26F12939CE5FE0D21E70429DDB51DDA3DB4CACF) | 2018-07-03   | No          |                     3 |


## Fingerprint List of Guard-only Relays in E2E Groups

185CFF801E6BE549F675AD61C3FE04104150AE1F,69E06EBB2573A4F89330BDF8BC869794A3E10E4D,E91FC7ABF7708A584FCFE88DB5CEA083D00E6511