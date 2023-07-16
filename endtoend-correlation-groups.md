---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-07-16 17:00 UTC**

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


## ContactInfo: Neel Chauhan &lt;neel AT neelc DOT org&gt; (28) {#neel-chauhan-neel-at-neelc-dot-org}

| Nickname                                                                                                 | First Seen   | Guardonly   |   Eff. Family Members |
|:---------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [NeelTorRelay2](https://metrics.torproject.org/rs.html#details/6E21BB0F39095B207C45DBBD30A521F0CABBF6A7) | 2023-03-11   | Yes         |                     1 |
| [NeelTorRelay1](https://metrics.torproject.org/rs.html#details/97011FAE9F14C820BEB31C467DEA11E6BFCCA0E1) | 2023-03-11   | Yes         |                     1 |
| [NeelTorRelay4](https://metrics.torproject.org/rs.html#details/66BCB27A28C3C98987C2F5A87E3F80282BE1DB32) | 2023-05-03   | Yes         |                     1 |
| [NeelTorRelay3](https://metrics.torproject.org/rs.html#details/BA3B3FBB7F23A9580A94DE811F1F2017CEFF52E1) | 2023-05-03   | Yes         |                     1 |
| [OnionPS17](https://metrics.torproject.org/rs.html#details/09A308A13D6EF30FD737D8A396F6B712C28EA61C)     | 2023-06-29   | No          |                    24 |
| [OnionPS24](https://metrics.torproject.org/rs.html#details/1693D7F30503F9F357D9422FA946D17D3386E93D)     | 2023-06-29   | No          |                    24 |
| [OnionPS4](https://metrics.torproject.org/rs.html#details/22AE701D9740661F64E4C8FE8D19CFD38D349202)      | 2023-06-29   | No          |                    24 |
| [OnionPS14](https://metrics.torproject.org/rs.html#details/2C5DFD7958B2F81F1B7E93B50153A92C62BD7F8E)     | 2023-06-29   | No          |                    24 |
| [OnionPS12](https://metrics.torproject.org/rs.html#details/2C6920D1022EB5F8DF8C0F71DC51C2F3BE982FD9)     | 2023-06-29   | No          |                    24 |
| [OnionPS22](https://metrics.torproject.org/rs.html#details/36ABB2F8AB1C080BAA3921BC1B0E674109BF8706)     | 2023-06-29   | No          |                    24 |
| [OnionPS13](https://metrics.torproject.org/rs.html#details/3C129C537C71F1F0BC8EFA05FE3D7068A6038F63)     | 2023-06-29   | No          |                    24 |
| [OnionPS7](https://metrics.torproject.org/rs.html#details/56B278FFE6699A4CCE20870A6393FED31CC3BCBA)      | 2023-06-29   | No          |                    24 |
| [OnionPS8](https://metrics.torproject.org/rs.html#details/65DE820FD4DA7A2F6EF2990D267315C7B4F55CED)      | 2023-06-29   | No          |                    24 |
| [OnionPS9](https://metrics.torproject.org/rs.html#details/80A493171F6EFD126A0E0CE5100EA2C6F412AD1B)      | 2023-06-29   | No          |                    24 |
| [OnionPS10](https://metrics.torproject.org/rs.html#details/85017491DADD5D39B8B7EFAE0B1CB72519106804)     | 2023-06-29   | No          |                    24 |
| [OnionPS2](https://metrics.torproject.org/rs.html#details/981D406945FAA29856CB4C0EE321C1B38AEB56EF)      | 2023-06-29   | No          |                    24 |
| [OnionPS21](https://metrics.torproject.org/rs.html#details/98911566DC054B5BE3A36EBD81CE370423A6EBFF)     | 2023-06-29   | No          |                    24 |
| [OnionPS3](https://metrics.torproject.org/rs.html#details/9C954B8DB0C8BCC4446D49B2ABBAB59B584178EF)      | 2023-06-29   | No          |                    24 |
| [OnionPS18](https://metrics.torproject.org/rs.html#details/9FB95310FBB98FE412E7199C806F1363E2EE2882)     | 2023-06-29   | No          |                    24 |
| [OnionPS6](https://metrics.torproject.org/rs.html#details/A259941BD2E86302E46AB07B09480DA45716D224)      | 2023-06-29   | No          |                    24 |
| [OnionPS20](https://metrics.torproject.org/rs.html#details/A525410BF80FFBB1F6CE89988455B905C4821C2E)     | 2023-06-29   | No          |                    24 |
| [OnionPS11](https://metrics.torproject.org/rs.html#details/B2BC20B6642EA1CD3A9F8DAB6A4605900DE35638)     | 2023-06-29   | No          |                    24 |
| [OnionPS19](https://metrics.torproject.org/rs.html#details/BA5C8ADBEC8641B628ED263F4F6354115E4DE9A2)     | 2023-06-29   | No          |                    24 |
| [OnionPS1](https://metrics.torproject.org/rs.html#details/C4CCF8C235695A30035A8125ECE007B521394C07)      | 2023-06-29   | No          |                    24 |
| [OnionPS15](https://metrics.torproject.org/rs.html#details/DCC1375E8C02C28CA18F284DF1480BCA5C55286C)     | 2023-06-29   | No          |                    24 |
| [OnionPS16](https://metrics.torproject.org/rs.html#details/DF71925FF5241C6442F3FA4BDE2AE203FACCC457)     | 2023-06-29   | No          |                    24 |
| [OnionPS23](https://metrics.torproject.org/rs.html#details/E3B140819EBF6DEE4EE25504E67A3757EFC9E5B7)     | 2023-06-29   | No          |                    24 |
| [OnionPS5](https://metrics.torproject.org/rs.html#details/E8B186C9B6D4D033B7BDC364A2CD6DE34A40ABD6)      | 2023-06-29   | No          |                    24 |


## Fingerprint List of Guard-only Relays in E2E Groups

66BCB27A28C3C98987C2F5A87E3F80282BE1DB32,6E21BB0F39095B207C45DBBD30A521F0CABBF6A7,97011FAE9F14C820BEB31C467DEA11E6BFCCA0E1,BA3B3FBB7F23A9580A94DE811F1F2017CEFF52E1