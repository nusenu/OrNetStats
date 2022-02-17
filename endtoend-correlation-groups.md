---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-02-17 18:00 UTC**

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


## ContactInfo: tor at xtom dot com (6) {#toratxtomdotcom}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [XTOMAMS](https://metrics.torproject.org/rs.html#details/A41A8317A5BD4DD10BE9925277DB332395F50F17)     | 2021-12-07   | Yes         |                     1 |
| [XTOMLON](https://metrics.torproject.org/rs.html#details/5ABC7AAFA86CA890242DE79582125B18C3B0E541)     | 2021-12-03   | Yes         |                     1 |
| [XTOMDUS](https://metrics.torproject.org/rs.html#details/955F15325D6F3E3350EA8A70EB5C49C5BF95C5A0)     | 2021-12-03   | Yes         |                     1 |
| [XTOMFRA](https://metrics.torproject.org/rs.html#details/AB12F88E52C439769EDB592B89AA36D8AF5A1C0C)     | 2021-12-07   | Yes         |                     1 |
| [XTOMSJC](https://metrics.torproject.org/rs.html#details/280F26E75C5ED7C292DD5AC5A9695C47B7784DC8)     | 2021-12-09   | Yes         |                     1 |
| [XTOMLONEXIT](https://metrics.torproject.org/rs.html#details/9331E29298E40EB28A01C780E73954CD73237F50) | 2022-02-03   | No          |                     1 |

## ContactInfo: admin dot tor-operator at firemail dot tech pgp:70 (5) {#admin-dot-tor-operator-at-firemail-dot-tech-pgp70}

| Nickname                                                                                             | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Zinc](https://metrics.torproject.org/rs.html#details/01F73DBD9B56C31E3D3AAEB95F8CF1DEB7D9A72F)      | 2020-04-13   | Yes         |                     4 |
| [Oxygen](https://metrics.torproject.org/rs.html#details/B29E6646E11E5E6EAFE7DDE5AD3C3FE966B49E4E)    | 2022-01-11   | Yes         |                     5 |
| [Plutonium](https://metrics.torproject.org/rs.html#details/6859D71E3E1323F959F9E0559E83A9088C462684) | 2021-12-09   | No          |                     4 |
| [Hydrogen](https://metrics.torproject.org/rs.html#details/702FD318AEED49702B5C16255ED5F595DA116516)  | 2020-10-01   | No          |                     5 |
| [Uranium](https://metrics.torproject.org/rs.html#details/90B818902D42800A5E5F31A2C0D9A2B0B31EAC5F)   | 2020-11-29   | No          |                     5 |

## ContactInfo: ContactInfo email:abuse stormycloud.org url:storm (24) {#contactinfo-emailabusestormycloudorg-urlstorm}

| Nickname                                                                                                  | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/19B53DE3B97AEE85A90D44F0F06C1AE69FF62237) | 2022-02-01   | Yes         |                    22 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/F8555980E41FF5D0E2379126DAD74C56FF32DD66) | 2022-02-01   | Yes         |                    22 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/00B211F85E145B50890633CA9CB6B18262E51CD7) | 2022-01-24   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/037A9B1EF680151D1977B52CFFA948819B2F867A) | 2022-01-23   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/0A5EE342140AF65850A0D1CCEF0ECB3223AFA24F) | 2022-02-09   | No          |                    22 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/166443CA1BE8020A9479B117E7ADB061CF8F7852) | 2022-01-25   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/2BC1779CF325C5E4A6C0A5F958E458ED104CCEA7) | 2022-01-25   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/3AD93704B1EFFA79F2BF09CAB7ADCC334D0BEF7A) | 2022-01-24   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/3EF489E1F8EDA383286769CBF90E3CB18B0F71CF) | 2022-01-24   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/4B0BC0CD47B93EB98CB2D624C634143F5BD62BF6) | 2022-02-09   | No          |                    22 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/6EA904BE17DB5CF37EB9416ECB73C24A7FED057E) | 2022-01-23   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/76B3B62839BC59822FC09C0E80435DD0524083D3) | 2022-01-24   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/7E7737831BEEB5EE423F37E127112F1E3C5419CF) | 2022-01-24   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/85422BC1612840FA70EB70ECCD9F66D0D397719B) | 2022-01-25   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/8F32C089CD71D6FB1012FD6EC1EC0438A57F32C5) | 2022-01-25   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/8FFA62DEB796D18DA8CAA9A95E0B1F60CDDDCB50) | 2022-01-23   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/A00FAA3F0F84F8B118D337660FF0AA4E3E32AE5A) | 2022-01-25   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/A88CE4546B3165A03E4099260B93294BE750532A) | 2022-01-25   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/BC7ACE7298DF5BC8FFCEA4CF0CB88C97902E4582) | 2022-01-25   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/D8773C1BAA890CDEF3B48B5EC5B6AA610735DCAB) | 2022-01-25   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/DDE988A745422A4BBFF0C1ABFD1777D74BFBC40E) | 2022-01-23   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/EDD507B5CAAAABFB0F343CF621A202F93CB57CE4) | 2022-01-23   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/EFF54875CFED77DDB6260A1A4AD2B0608E3807A1) | 2022-01-24   | No          |                    26 |
| [StormyCloudInc](https://metrics.torproject.org/rs.html#details/F8BDA076BAA2452B7CD885B58863D956883605D6) | 2022-01-25   | No          |                    26 |


## Fingerprint List of Guard-only Relays in E2E Groups

280F26E75C5ED7C292DD5AC5A9695C47B7784DC8,5ABC7AAFA86CA890242DE79582125B18C3B0E541,955F15325D6F3E3350EA8A70EB5C49C5BF95C5A0,A41A8317A5BD4DD10BE9925277DB332395F50F17,AB12F88E52C439769EDB592B89AA36D8AF5A1C0C,01F73DBD9B56C31E3D3AAEB95F8CF1DEB7D9A72F,B29E6646E11E5E6EAFE7DDE5AD3C3FE966B49E4E,19B53DE3B97AEE85A90D44F0F06C1AE69FF62237,4E6515A5E941C1C5517FB2952972BEB458640BCF,A7348BE96DF5BD080A9BA6F87454706BFD75371A,F8555980E41FF5D0E2379126DAD74C56FF32DD66