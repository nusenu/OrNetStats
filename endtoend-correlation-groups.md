---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-10-01 21:00 UTC**

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


## ContactInfo: Brandon Kuschel &lt;kusch023 AT NOSPAM umn dot edu&gt; (8) {#brandon-kuschel-kusch023-at-nospam-umn-dot-edu}

| Nickname                                                                                              | First Seen   | Guardonly   |   Eff. Family Members |
|:------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Charybdis2](https://metrics.torproject.org/rs.html#details/1DEECD906AFECF496B7DC1E40829F4563517B4CC) | 2022-09-19   | Yes         |                     7 |
| [Lamia](https://metrics.torproject.org/rs.html#details/C46548D44C0CA5855C175CE26F5817D38F833C9F)      | 2022-08-21   | Yes         |                     8 |
| [Minotaur2](https://metrics.torproject.org/rs.html#details/6E586C8F62D0E153792095AFDA55D4E2E3F3421F)  | 2022-09-19   | Yes         |                     8 |
| [Echidna](https://metrics.torproject.org/rs.html#details/BA57222A0EC9ECDF003AED665DFB0B1287EA039D)    | 2022-08-21   | Yes         |                     8 |
| [Polyphemus](https://metrics.torproject.org/rs.html#details/0CABED9159F1E4BE82879F5A34ED8D7349E931BD) | 2022-09-14   | No          |                     7 |
| [Chimera](https://metrics.torproject.org/rs.html#details/2946159CF9D8EAEB8C4A27F6A54B01A459DEE164)    | 2022-08-21   | No          |                     7 |
| [Minotaur](https://metrics.torproject.org/rs.html#details/8BDBE498180C41249D3230FC5092CB3EB5A62482)   | 2021-04-06   | No          |                     8 |
| [Charybdis](https://metrics.torproject.org/rs.html#details/CBF59EC5B9FD108092AE9149EFDAE41F882DA669)  | 2022-08-19   | No          |                     7 |

## ContactInfo: tor at reichsfunkma dot st tor-relay.co (5) {#tor-at-reichsfunkma-dot-st-tor-relayco}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Reichsfunkmast4](https://metrics.torproject.org/rs.html#details/4F35C7CA62740A43AC6A46A355516B85018AC8A0) | 2022-08-20   | Yes         |                     6 |
| [Reichsfunkmast5](https://metrics.torproject.org/rs.html#details/B0A134CAF4494B3913E05DB46347633D9C4A8A8B) | 2022-06-23   | Yes         |                     6 |
| [Reichsfunkmast9](https://metrics.torproject.org/rs.html#details/0CF8D1A7921192BDED02CA577A7D93654B59B83A) | 2022-10-01   | No          |                     1 |
| [Reichsfunkmast1](https://metrics.torproject.org/rs.html#details/3B43FB4F237EBE3570CB06B500CA1E8B46EEAFA1) | 2022-06-03   | No          |                     6 |
| [Reichsfunkmast2](https://metrics.torproject.org/rs.html#details/F3A9588FB45F76DA4DE5B350C425C130F6FFA983) | 2022-06-22   | No          |                     6 |

## ContactInfo: cam632@gmx.com (2) {#cam632gmxcom}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Praktiker](https://metrics.torproject.org/rs.html#details/E99A1B54541518A8A6058D75762497AE0D3442DC) | 2022-09-23   | Yes         |                     1 |
| [Boro](https://metrics.torproject.org/rs.html#details/5F4BCBC6E20AE074340D0A743E6F2EA4B51B09C1)      | 2022-08-31   | No          |                     1 |

## ContactInfo: tor at reichsfunkma dot st (4) {#tor-at-reichsfunkma-dot-st}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Reichsfunkmast6](https://metrics.torproject.org/rs.html#details/3B42ABB5E5338BD98BDB44918581379107B54AEF) | 2022-09-23   | Yes         |                     6 |
| [Reichsfunkmast7](https://metrics.torproject.org/rs.html#details/3006DF6A83292E3472BEC461543CEB775C00BB9B) | 2022-09-30   | No          |                     1 |
| [Reichsfunkmast3](https://metrics.torproject.org/rs.html#details/99A6EDEC44F733ACAF2539B353118F36D27322E3) | 2022-09-20   | No          |                     6 |
| [Reichsfunkmast8](https://metrics.torproject.org/rs.html#details/E8B477C17E9FC1A535BBC2468957F7B9282A783A) | 2022-09-30   | No          |                     1 |


## Fingerprint List of Guard-only Relays in E2E Groups

1DEECD906AFECF496B7DC1E40829F4563517B4CC,6E586C8F62D0E153792095AFDA55D4E2E3F3421F,BA57222A0EC9ECDF003AED665DFB0B1287EA039D,C46548D44C0CA5855C175CE26F5817D38F833C9F,4F35C7CA62740A43AC6A46A355516B85018AC8A0,B0A134CAF4494B3913E05DB46347633D9C4A8A8B,E99A1B54541518A8A6058D75762497AE0D3442DC,3B42ABB5E5338BD98BDB44918581379107B54AEF