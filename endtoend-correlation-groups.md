---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2018-07-05 07:00 UTC**

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


## ContactInfo: pm@dpjp.ru - 1Hr5ALwotveTsEJpxuyox2en6d62ZVedfs (6) {#pmdpjpru---1hr5alwotvetsejpxuyox2en6d62zvedfs}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [dpjp05](https://metrics.torproject.org/rs.html#details/185CFF801E6BE549F675AD61C3FE04104150AE1F)         | 2018-06-22   | Yes         |                     1 |
| [dpjp01TorExit](https://metrics.torproject.org/rs.html#details/69E06EBB2573A4F89330BDF8BC869794A3E10E4D)  | 2018-01-13   | Yes         |                     4 |
| [dpjp03ny](https://metrics.torproject.org/rs.html#details/BB43D5594590897A1152E5372C74A467BDD2FD99)       | 2018-06-15   | Yes         |                     1 |
| [dpjp07](https://metrics.torproject.org/rs.html#details/A379AD9020BB119B53785888DACC63C712285649)         | 2018-05-20   | Yes         |                     4 |
| [dpjp02reloaded](https://metrics.torproject.org/rs.html#details/AA29ED6C533F78BC1EF3994656048464AEE2A29A) | 2018-04-04   | Yes         |                     4 |
| [dpjp06TorExit](https://metrics.torproject.org/rs.html#details/C5AFC0EC23AC7FB19067FC4C511316A4CE38C32F)  | 2018-04-02   | No          |                     4 |

## ContactInfo: tor-operator@your-emailaddress-domain (3) {#tor-operatoryour-emailaddress-domain}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/64B8A00F64E16BF5C5685A76C4D9722DCBF05400) | 2018-05-01   | Yes         |                     1 |
| [Relay](https://metrics.torproject.org/rs.html#details/7430AD5653ADA688F8EFE4FCE93D7D17A9D45A0F)       | 2018-06-25   | Yes         |                     1 |
| [myNiceRelay](https://metrics.torproject.org/rs.html#details/9FC15C742C2E95A34F104CB5A0826C6659CFF2B7) | 2018-06-20   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

185CFF801E6BE549F675AD61C3FE04104150AE1F,64B8A00F64E16BF5C5685A76C4D9722DCBF05400,69E06EBB2573A4F89330BDF8BC869794A3E10E4D,7430AD5653ADA688F8EFE4FCE93D7D17A9D45A0F,A379AD9020BB119B53785888DACC63C712285649,AA29ED6C533F78BC1EF3994656048464AEE2A29A,BB43D5594590897A1152E5372C74A467BDD2FD99