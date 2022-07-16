---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2022-07-16 09:00 UTC**

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


## ContactInfo: info@fileditch.com (4) {#infofileditchcom}

| Nickname                                                                                                   | First Seen   | Guardonly   |   Eff. Family Members |
|:-----------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [FileDitchRelay0](https://metrics.torproject.org/rs.html#details/1D58C94057CFA3A875208BD699B2CA262E7C7C1C) | 2022-07-01   | Yes         |                     3 |
| [FileDitchExit1](https://metrics.torproject.org/rs.html#details/667741676DD35F168C1858232928AA26564A2EC6)  | 2022-07-07   | No          |                     1 |
| [FileDitchExit2](https://metrics.torproject.org/rs.html#details/C92DE921C34ACB1C1B4EA7D2C1ECF4A0ACD2CA00)  | 2022-06-09   | No          |                     3 |
| [FileDitchExit0](https://metrics.torproject.org/rs.html#details/ED13907E3BD2901D6DFB2036805640EA3A33D97A)  | 2022-06-09   | No          |                     3 |

## ContactInfo: url:relayon.org proof:uri-rsa abuse:abuse relayon (88) {#urlrelayonorg-proofuri-rsa-abuseabuserelayon}

| Nickname                                                                                               | First Seen   | Guardonly   |   Eff. Family Members |
|:-------------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [relayon1143](https://metrics.torproject.org/rs.html#details/F5F8497B39C1022BCA786012390E1FDA55AB73EC) | 2022-07-05   | Yes         |                     1 |
| [relayon1142](https://metrics.torproject.org/rs.html#details/64BB15B6295E3A44594F438CD0E674E7C4E60BA1) | 2022-07-05   | Yes         |                     1 |
| [relayon1149](https://metrics.torproject.org/rs.html#details/059851E41076E47C8B391292BF0E73BE1600FBCD) | 2022-06-30   | No          |                   127 |
| [relayon1153](https://metrics.torproject.org/rs.html#details/066CD2C493E4DF7300B2731EAF7E317433262591) | 2022-06-30   | No          |                   127 |
| [relayon0159](https://metrics.torproject.org/rs.html#details/07A2ADB079E1440927020D23B47B4358CCA585A8) | 2022-07-10   | No          |                   127 |
| [relayon0154](https://metrics.torproject.org/rs.html#details/0ADDA48046EFCD0EDFD28F2461BC27B755932D95) | 2022-07-10   | No          |                   127 |
| [relayon1179](https://metrics.torproject.org/rs.html#details/0CA3677DCF4314403CE148859EE5553F9ADFD66E) | 2022-06-30   | No          |                   127 |
| [relayon1128](https://metrics.torproject.org/rs.html#details/0D5AA7C0C53B65EBE9CE3A4093CBAF2319C45271) | 2022-06-30   | No          |                   127 |
| [relayon1133](https://metrics.torproject.org/rs.html#details/0E4616DEC4D8DCB0D54E15EE9DCB13A55D57F7F7) | 2022-06-30   | No          |                   127 |
| [relayon1143](https://metrics.torproject.org/rs.html#details/0EA1D72D5925E999A93866FFCD16950D430DE267) | 2022-06-30   | No          |                   127 |
| [relayon0187](https://metrics.torproject.org/rs.html#details/0EC0515743B4C2883F908C528774A6E12E613B85) | 2022-07-10   | No          |                   127 |
| [relayon0128](https://metrics.torproject.org/rs.html#details/16A2165A0B0FD4BF24A337373378863E3A7633A2) | 2022-07-10   | No          |                   127 |
| [relayon0181](https://metrics.torproject.org/rs.html#details/174490E075B23EF126BB145EF81FA932FA345D1D) | 2022-07-10   | No          |                   127 |
| [relayon1158](https://metrics.torproject.org/rs.html#details/1928A32C989AF166EBC762FE2D8E257D265ACBA7) | 2022-06-30   | No          |                   127 |
| [relayon0191](https://metrics.torproject.org/rs.html#details/201FF736CF3406134B2A62FE59C80F1480458811) | 2022-07-10   | No          |                   127 |
| [relayon1147](https://metrics.torproject.org/rs.html#details/20A1B55784057884DB8B6D90026864EDE14542F5) | 2022-06-30   | No          |                   127 |
| [relayon0158](https://metrics.torproject.org/rs.html#details/21666A25FFB89D74B5F9577D6FA8BB7EA7CC77B2) | 2022-07-10   | No          |                   127 |
| [relayon0145](https://metrics.torproject.org/rs.html#details/22552EC1CEA14A6B418FA9E8479EDEFB079535F1) | 2022-07-10   | No          |                   127 |
| [relayon0163](https://metrics.torproject.org/rs.html#details/26C57F06BDECFF9968F65805CD9ECC9036B02AA9) | 2022-07-10   | No          |                   127 |
| [relayon0142](https://metrics.torproject.org/rs.html#details/27A145F2EC4528E702B0BEFB229FBFA96A0C7BA6) | 2022-07-10   | No          |                   127 |
| [relayon0129](https://metrics.torproject.org/rs.html#details/293F149DD1971492E31779AA12CCE7C545BF5088) | 2022-07-10   | No          |                   127 |
| [relayon1139](https://metrics.torproject.org/rs.html#details/2B810AA81A036E01FFC74A6931DBB583169BB7FE) | 2022-06-30   | No          |                   127 |
| [relayon0141](https://metrics.torproject.org/rs.html#details/2E9030B90B0599BB20E4332DAA88D8858C8DDD7F) | 2022-07-10   | No          |                   127 |
| [relayon0138](https://metrics.torproject.org/rs.html#details/331CEE19F311204CB732FF8DB5694C4DF32F3B26) | 2022-07-10   | No          |                   127 |
| [relayon0169](https://metrics.torproject.org/rs.html#details/36D8A00885BCBFEB17312607C0877BFFD9330CF0) | 2022-07-10   | No          |                   127 |
| [relayon0186](https://metrics.torproject.org/rs.html#details/3A7B07485E2F4DC45FB57761CAC59FA2C556AAFE) | 2022-07-10   | No          |                   127 |
| [relayon0148](https://metrics.torproject.org/rs.html#details/3C363C8B45D21ED2C656A0ED73B947F5469C5199) | 2022-07-10   | No          |                   127 |
| [relayon1150](https://metrics.torproject.org/rs.html#details/3DB5EEE6865B1F1CCEDE2F75DCB8F9A6D987BDE3) | 2022-06-30   | No          |                   127 |
| [relayon0139](https://metrics.torproject.org/rs.html#details/3FBBE55B719D0B8547E7EB75F014393E3736AED4) | 2022-07-10   | No          |                   127 |
| [relayon0131](https://metrics.torproject.org/rs.html#details/42CFF0CAAF7EB5E86B358DB047DCFE53B64856EB) | 2022-07-10   | No          |                   127 |
| [relayon0174](https://metrics.torproject.org/rs.html#details/4329C619B7EA274A6A9F610DD22863C7E1634756) | 2022-07-10   | No          |                   127 |
| [relayon0171](https://metrics.torproject.org/rs.html#details/48020D412674B13B083B9FF0A61222D121C67868) | 2022-07-10   | No          |                   127 |
| [relayon0182](https://metrics.torproject.org/rs.html#details/4C830D0B56E49ECBFCB114542600A1725DB1A1E7) | 2022-07-10   | No          |                   127 |
| [relayon1138](https://metrics.torproject.org/rs.html#details/4CEEB0CE90FF70CB54CEE37EAFCE176661231512) | 2022-06-30   | No          |                   127 |
| [relayon1129](https://metrics.torproject.org/rs.html#details/4E09798074474CCF51F1D6B46141C1506587020B) | 2022-06-30   | No          |                   127 |
| [relayon0179](https://metrics.torproject.org/rs.html#details/4F56DE76CDC2A296B6D637949207F904E5A20C21) | 2022-07-10   | No          |                   127 |
| [relayon0153](https://metrics.torproject.org/rs.html#details/54ACB278AA2ABD96F9150AB72B08A8A8B1E4A659) | 2022-07-10   | No          |                   127 |
| [relayon0161](https://metrics.torproject.org/rs.html#details/57D0CA93B069DCCC2C34BED2BDCBC71AF8C89D3F) | 2022-07-10   | No          |                   127 |
| [relayon0165](https://metrics.torproject.org/rs.html#details/5EF9F7FAEC180D0548F4C33F450D70CDE25AAC81) | 2022-07-10   | No          |                   127 |
| [relayon0147](https://metrics.torproject.org/rs.html#details/6854BE1FF67606E28B6A500C25BE3CFCE4F53DD0) | 2022-07-10   | No          |                   127 |
| [relayon1152](https://metrics.torproject.org/rs.html#details/6FC1F0A868B41BC5F79832547D4D1CF868171A31) | 2022-06-30   | No          |                   127 |
| [relayon0130](https://metrics.torproject.org/rs.html#details/71F7BD26BBF6EAF711B71A7685815E00809EF261) | 2022-07-10   | No          |                   127 |
| [relayon0185](https://metrics.torproject.org/rs.html#details/72CDE7793F029523509484439A35A05810301D0E) | 2022-07-10   | No          |                   127 |
| [relayon1169](https://metrics.torproject.org/rs.html#details/78C30768B05DA11CD764E229C237B50471319CFE) | 2022-06-30   | No          |                   127 |
| [relayon0156](https://metrics.torproject.org/rs.html#details/7C34BB94624DD1194CAD0083ACB9251AEBE3BF8C) | 2022-07-10   | No          |                   127 |
| [relayon0135](https://metrics.torproject.org/rs.html#details/7CC686289752FDA026E8B22246EDE0979D1B7B04) | 2022-07-10   | No          |                   127 |
| [relayon1181](https://metrics.torproject.org/rs.html#details/8132DD2EFA6D048CB9D050C78453F5C8D8CCAF65) | 2022-06-30   | No          |                   127 |
| [relayon0144](https://metrics.torproject.org/rs.html#details/872D0A0DEBE914EC3C3E3105B7A8CC157662FA68) | 2022-07-10   | No          |                   127 |
| [relayon0188](https://metrics.torproject.org/rs.html#details/8ABB1CE0BEACFF2C9F8B53B4C286614E52E57381) | 2022-07-10   | No          |                   127 |
| [relayon1154](https://metrics.torproject.org/rs.html#details/8F52E0177AD35F590C5B83960AA11ED00F72629A) | 2022-06-30   | No          |                   127 |
| [relayon0146](https://metrics.torproject.org/rs.html#details/914B3AB3FCF39CEBE15FFF743C0AC1614591E966) | 2022-07-10   | No          |                   127 |
| [relayon1166](https://metrics.torproject.org/rs.html#details/928F3A31CE726451DAD32316DE91D5FB6F8C10D5) | 2022-06-30   | No          |                   127 |
| [relayon0164](https://metrics.torproject.org/rs.html#details/92B1634A7D1C35DDCEB34E0FC1229602D0AEDFB4) | 2022-07-10   | No          |                   127 |
| [relayon0189](https://metrics.torproject.org/rs.html#details/970A8832BAECDCCF5FBAD492F8D65C3C084B6F11) | 2022-07-10   | No          |                   127 |
| [relayon0184](https://metrics.torproject.org/rs.html#details/993D31DDD72EFF8C3FBC5A4899DF85E062E4E0CA) | 2022-07-10   | No          |                   127 |
| [relayon1178](https://metrics.torproject.org/rs.html#details/9AABDF5A8E5D546663A91788ECFD9C484740D761) | 2022-06-30   | No          |                   127 |
| [relayon0190](https://metrics.torproject.org/rs.html#details/9BAD1607C3A2328FBF26BC45AF46A7F8153D2BCC) | 2022-07-10   | No          |                   127 |
| [relayon1189](https://metrics.torproject.org/rs.html#details/A1981F6980AC1AF9756940660267C01D11E15B02) | 2022-06-30   | No          |                   127 |
| [relayon0168](https://metrics.torproject.org/rs.html#details/A4FE9A1F6A7EB6A002A1F3DFA313A43390E22C6F) | 2022-07-10   | No          |                   127 |
| [relayon0143](https://metrics.torproject.org/rs.html#details/B23F3E3D66658CCBD83AAA977093E4B652B834A4) | 2022-07-10   | No          |                   127 |
| [relayon0162](https://metrics.torproject.org/rs.html#details/B4C4989666384C40914197A767E1D1D299E73676) | 2022-07-10   | No          |                   127 |
| [relayon0167](https://metrics.torproject.org/rs.html#details/B60B94FC0FD8DF6F2D9C611F77FC7EF66646A45C) | 2022-07-10   | No          |                   127 |
| [relayon0133](https://metrics.torproject.org/rs.html#details/B6BAB95C30B2A1FF75B80B5E2B0895B97FF87D2F) | 2022-07-10   | No          |                   127 |
| [relayon0152](https://metrics.torproject.org/rs.html#details/B9DA7E83EEA60B91D7B18A272F38B5F6AC7D33C7) | 2022-07-10   | No          |                   127 |
| [relayon1155](https://metrics.torproject.org/rs.html#details/BAB161E1E3319F005568E27029681ED537AF3406) | 2022-06-30   | No          |                   127 |
| [relayon0173](https://metrics.torproject.org/rs.html#details/BC489671E2D42AD4C5FD289B389FE8401A28FDE0) | 2022-07-10   | No          |                   127 |
| [relayon1131](https://metrics.torproject.org/rs.html#details/C264CF7C05E8CC6DC7D22D0392D1311B1F7F5E25) | 2022-06-30   | No          |                   127 |
| [relayon0172](https://metrics.torproject.org/rs.html#details/C6B47E1F0D3C75F36FA00CF63ABABB984DD13A1A) | 2022-07-10   | No          |                   127 |
| [relayon0183](https://metrics.torproject.org/rs.html#details/CE6511968ACAA43402638D66A2FAC5F32F9A45C4) | 2022-07-10   | No          |                   127 |
| [relayon1140](https://metrics.torproject.org/rs.html#details/CF0F49C017ED14EFD54E953F428AE3508A7ED85A) | 2022-06-30   | No          |                   127 |
| [relayon0178](https://metrics.torproject.org/rs.html#details/D1C45FAAD766E810EDA2401335CC8EBDE8EA8526) | 2022-07-10   | No          |                   127 |
| [relayon1141](https://metrics.torproject.org/rs.html#details/D1D5D6A5AF1B94F4FB3371034B11FF72CB40A83F) | 2022-06-30   | No          |                   127 |
| [relayon0155](https://metrics.torproject.org/rs.html#details/D4CFB23D6880135B8BF20C820E59C34029153432) | 2022-07-10   | No          |                   127 |
| [relayon1135](https://metrics.torproject.org/rs.html#details/D604C7BF901191E59D791EF8758D19EE8E8C9A70) | 2022-06-30   | No          |                   127 |
| [relayon1134](https://metrics.torproject.org/rs.html#details/DA22C0B589959ADD14D16606B9A2A512CED61C4F) | 2022-06-30   | No          |                   127 |
| [relayon1137](https://metrics.torproject.org/rs.html#details/DB16C773A0E87530FD4FC6D5D81FFB6D6EB2E5D0) | 2022-06-30   | No          |                   127 |
| [relayon0149](https://metrics.torproject.org/rs.html#details/DC44E351DF9681D6999A1E59D83077D4047FEDF5) | 2022-07-10   | No          |                   127 |
| [relayon0136](https://metrics.torproject.org/rs.html#details/DEAFF8BA64CC7898AFC5D94A1BCFA87FFFCF5657) | 2022-07-10   | No          |                   127 |
| [relayon0157](https://metrics.torproject.org/rs.html#details/E53683EDF846E6D27C6685FA481935FB16339526) | 2022-07-10   | No          |                   127 |
| [relayon0151](https://metrics.torproject.org/rs.html#details/EA6BD20181D488A83B25541275B374F5BA1AA45A) | 2022-07-10   | No          |                   127 |
| [relayon1159](https://metrics.torproject.org/rs.html#details/EC677ABD5F31FCAFC4CAA9865487DA14E2D15755) | 2022-06-30   | No          |                   127 |
| [relayon0180](https://metrics.torproject.org/rs.html#details/EF3CD6C1223940763ADD5D1A703D8D22809BFEAC) | 2022-07-10   | No          |                   127 |
| [relayon0175](https://metrics.torproject.org/rs.html#details/F03267E78461E198C7A8D3E825146895B19BFD1A) | 2022-07-10   | No          |                   127 |
| [relayon0160](https://metrics.torproject.org/rs.html#details/F1C28FCABCC61193B61E651B3210D4739B837F3C) | 2022-07-10   | No          |                   127 |
| [relayon0140](https://metrics.torproject.org/rs.html#details/F211A7031A14FB0DA13D467F6C1B98FDC3F2A559) | 2022-07-10   | No          |                   127 |
| [relayon1184](https://metrics.torproject.org/rs.html#details/F586F0E989416C210211A74640E1D9FAC0C74264) | 2022-06-30   | No          |                   127 |
| [relayon0137](https://metrics.torproject.org/rs.html#details/F9408C144B36D78A47BABB0BB53DFF671D23BE51) | 2022-07-10   | No          |                   127 |
| [relayon0170](https://metrics.torproject.org/rs.html#details/FF450F683B7BE494703B90827DB2DBD05B624471) | 2022-07-10   | No          |                   127 |


## Fingerprint List of Guard-only Relays in E2E Groups

1D58C94057CFA3A875208BD699B2CA262E7C7C1C,64BB15B6295E3A44594F438CD0E674E7C4E60BA1,F5F8497B39C1022BCA786012390E1FDA55AB73EC