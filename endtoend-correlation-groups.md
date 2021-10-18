---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-10-18 15:00 UTC**

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


## ContactInfo: 0x9F29C15D42A8B6F3 Nos oignons &lt;adminsys@nos-oigno (10) {#0x9f29c15d42a8b6f3-nos-oignons-adminsysnos-oigno}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [arecoque2](https://metrics.torproject.org/rs.html#details/42E817BE07AB39CA3BD7A442AF08E007FF2E3F5B)      | 2021-10-03   | Yes         |                     1 |
| [arecoque1](https://metrics.torproject.org/rs.html#details/CD1FD2C1F330A3293DA6068E6A23866D063D6DCB)      | 2021-10-03   | Yes         |                     1 |
| [mwittig](https://metrics.torproject.org/rs.html#details/2AB6F7D59DF6153F4DB1DB6479C3422F5724C4BA)        | 2020-06-30   | No          |                     8 |
| [marylou1](https://metrics.torproject.org/rs.html#details/578E007E5E4535FBFEF7758D8587B07B4C8C5D06)       | 2014-11-18   | No          |                     8 |
| [AlGrothendieck](https://metrics.torproject.org/rs.html#details/8E6EDA78D8E3ABA88D877C3E37D6D4F0938C7B9F) | 2016-06-09   | No          |                     8 |
| [marylou2](https://metrics.torproject.org/rs.html#details/90FD830C357A5109AB3C505287713F1AC811174C)       | 2015-02-21   | No          |                     8 |
| [ekumen](https://metrics.torproject.org/rs.html#details/9BA84E8C90083676F86C7427C8D105925F13716C)         | 2014-04-08   | No          |                     8 |
| [marcuse2](https://metrics.torproject.org/rs.html#details/C656B41AEFB40A141967EBF49D6E69603C9B4A11)       | 2014-04-08   | No          |                     8 |
| [marcuse1](https://metrics.torproject.org/rs.html#details/EFAE44728264982224445E96214C15F9075DEE1D)       | 2014-04-08   | No          |                     8 |
| [Elenagb](https://metrics.torproject.org/rs.html#details/F47B13BFCE4EF48CDEF6C4D7C7A99208EBB972B5)        | 2018-11-08   | No          |                     8 |


## Fingerprint List of Guard-only Relays in E2E Groups

42E817BE07AB39CA3BD7A442AF08E007FF2E3F5B,CD1FD2C1F330A3293DA6068E6A23866D063D6DCB