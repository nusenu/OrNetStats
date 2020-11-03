---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2020-11-02 14:00 UTC**

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


## ContactInfo: tor-operator@your-emailaddress-domain (8) {#tor-operatoryour-emailaddress-domain}

| Nickname                                                                                                      | First Seen   | Guardonly   |   Eff. Family Members |
|:--------------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [crypt0Dude01](https://metrics.torproject.org/rs.html#details/6CD171AD2C407711CBFD5BFDA79CB7F6A74C3252)       | 2020-09-30   | Yes         |                     1 |
| [aabbcc](https://metrics.torproject.org/rs.html#details/E7C1FAFB7525149A0E911512F511D942BA5EEAAF)             | 2019-05-29   | Yes         |                     1 |
| [phenix](https://metrics.torproject.org/rs.html#details/08CE663363148E992595724A2B29BF8EE68D32A4)             | 2020-10-11   | Yes         |                     1 |
| [aabbcc](https://metrics.torproject.org/rs.html#details/6C12C06131E103C1703B2037CC3386B69C0BCAC4)             | 2020-10-13   | Yes         |                     1 |
| [anotherRelay](https://metrics.torproject.org/rs.html#details/F6691E3EB7CAB3C876AAA885E6801B63DC998C39)       | 2018-10-29   | Yes         |                     1 |
| [SuchaNiceRelay](https://metrics.torproject.org/rs.html#details/93FFDC0C36C316208AC6291DE754D733B4D88A13)     | 2020-04-23   | Yes         |                     1 |
| [Marsu](https://metrics.torproject.org/rs.html#details/1DE8E81240D20D9755B29A8AEA131BE2CD537FB8)              | 2020-01-01   | Yes         |                     1 |
| [BanderaHuesosochka](https://metrics.torproject.org/rs.html#details/304B186CC793A0BA6E63C2D360C99D500DBDB9E4) | 2020-09-30   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

08CE663363148E992595724A2B29BF8EE68D32A4,1DE8E81240D20D9755B29A8AEA131BE2CD537FB8,4B550F757A5904939280CB85DE61F125A08AE5DE,6C12C06131E103C1703B2037CC3386B69C0BCAC4,6CD171AD2C407711CBFD5BFDA79CB7F6A74C3252,93FFDC0C36C316208AC6291DE754D733B4D88A13,E7C1FAFB7525149A0E911512F511D942BA5EEAAF,F6691E3EB7CAB3C876AAA885E6801B63DC998C39