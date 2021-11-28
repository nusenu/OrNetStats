---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2021-11-28 16:00 UTC**

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


## ContactInfo: ContactInfo email:abuse stormycloud.org url:storm (20) {#contactinfo-emailabusestormycloudorg-urlstorm}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/FE0016D9350B7AA5A7DAE6D463DD8F0EC1228F7D) | 2021-10-21   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/0AE98603DEDD519D0EFF2A66162B9529ECD9D694) | 2021-10-18   | Yes         |                     1 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/5886B4AD841347BBC4448346BAD7641BE716E71F) | 2021-10-21   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/E4E7D68A7B066E48E9D47FDB289184E3DEAC9673) | 2021-10-19   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/2A772EBF36CE63BD643674C4E3914D9A55F40140) | 2021-10-19   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/2F5F3C95B273490BF2626E0CD7F0F045C4CFF90D) | 2021-10-18   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/C6BDE87671B6594AF2A66964CAD519844503B793) | 2021-11-01   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/D043A4CB9B1B7A8E225B4E113289CAC0B0F0A683) | 2021-11-09   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/D8C495D5A0B10D5E2E58004FE633084EBF732C21) | 2021-10-18   | Yes         |                     1 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/854FE47BF85F4F6A0297DE5405F26891BB600246) | 2021-11-09   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/2F10EF06BA3712840C4FB986ED0E9AFEC1A0C74E) | 2021-11-01   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/6E914A73D403856F78A7413647681BF7B7FD5B4F) | 2021-11-01   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/6FFBF52ACB71934CC5754DB3A8880E85E2781F0D) | 2021-11-01   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/B7A30CCCEB768AED08A8E2BBF3327CC12091D5B5) | 2021-11-01   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/74838E434B0CF36CC2399BAE07C204D1BD14C14F) | 2021-10-19   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/F3F863A2121E54CF5C455E9CAECD114DA46FAD5D) | 2021-11-01   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/1D0CCED2128CAA9B9D8C3D71A08F192BBA91120C) | 2021-11-01   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/6CEB64F6C655B7394A7A2C6175D17FAC3387D79B) | 2021-11-01   | Yes         |                    18 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/69093E6A0A39704E69042AA8928148FFAFE15BCB) | 2021-10-22   | No          |                     2 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/76AE930782A3EA62AB5C0D72C6C72EF291D37B4E) | 2021-10-22   | No          |                     2 |


## Fingerprint List of Guard-only Relays in E2E Groups

0AE98603DEDD519D0EFF2A66162B9529ECD9D694,1D0CCED2128CAA9B9D8C3D71A08F192BBA91120C,2A772EBF36CE63BD643674C4E3914D9A55F40140,2F10EF06BA3712840C4FB986ED0E9AFEC1A0C74E,2F5F3C95B273490BF2626E0CD7F0F045C4CFF90D,433A112B7530B795980B389270962EDDB943D028,5886B4AD841347BBC4448346BAD7641BE716E71F,6CEB64F6C655B7394A7A2C6175D17FAC3387D79B,6E914A73D403856F78A7413647681BF7B7FD5B4F,6FFBF52ACB71934CC5754DB3A8880E85E2781F0D,74838E434B0CF36CC2399BAE07C204D1BD14C14F,78F8AB7B2CE34A90599753068C0589F09E0307BD,854FE47BF85F4F6A0297DE5405F26891BB600246,B7A30CCCEB768AED08A8E2BBF3327CC12091D5B5,C6BDE87671B6594AF2A66964CAD519844503B793,D043A4CB9B1B7A8E225B4E113289CAC0B0F0A683,D8C495D5A0B10D5E2E58004FE633084EBF732C21,E4E7D68A7B066E48E9D47FDB289184E3DEAC9673,F3F863A2121E54CF5C455E9CAECD114DA46FAD5D,FE0016D9350B7AA5A7DAE6D463DD8F0EC1228F7D