---
layout: default
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2019-09-06 21:00 UTC**

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


## ContactInfo: runtime-error at riseup dot net (6) {#runtime-erroratriseupdotnet}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Daenerys](https://metrics.torproject.org/rs.html#details/E312A938D71045BE3A5C1FF3AB87CF7464194861)  | 2019-07-13   | Yes         |                     1 |
| [Dreamfyre](https://metrics.torproject.org/rs.html#details/1CA9B177EB87B679883D3C520AF5F1AA104E573E) | 2019-08-22   | No          |                     1 |
| [Viserion](https://metrics.torproject.org/rs.html#details/4C5B8134341E66CB09246985E4039F9BFC0ADCE3)  | 2019-07-19   | No          |                     1 |
| [Visenya](https://metrics.torproject.org/rs.html#details/A339297680115D931FA2B98C311300E8492D83AA)   | 2019-07-10   | No          |                     1 |
| [Targaryen](https://metrics.torproject.org/rs.html#details/B0D0C294326E940CE335E484A338153F2911D2C8) | 2019-08-04   | No          |                     1 |
| [Dracarys](https://metrics.torproject.org/rs.html#details/D954378F53DD7B01063B8E742D973DC12D11F34A)  | 2019-08-14   | No          |                     1 |

## ContactInfo: Steven S &lt;katsalmovies@gmail.com&gt; (3) {#steven-s-katsalmoviesgmailcom}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [bigdaddyny](https://metrics.torproject.org/rs.html#details/0BCCF364C4EE7338B6E920E63E951922C85F91F7)  | 2019-07-15   | Yes         |                     1 |
| [bigdaddyny3](https://metrics.torproject.org/rs.html#details/AE236568ED01527850FA0D5BEFBBF6C6BDA47AF0) | 2019-07-28   | Yes         |                     1 |
| [bigdaddyny2](https://metrics.torproject.org/rs.html#details/25AA19700404E2B482B60B9F52AED83E3E73B5FC) | 2019-07-21   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

0BCCF364C4EE7338B6E920E63E951922C85F91F7,AE236568ED01527850FA0D5BEFBBF6C6BDA47AF0,E312A938D71045BE3A5C1FF3AB87CF7464194861