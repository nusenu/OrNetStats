---
datatable: true
---


# Tor Relay Operators in End-to-End (E2E) Correlation Position

Tor network data as of: **2023-06-25 11:00 UTC**

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


## ContactInfo: email:abuse-node49 posteo.de url:hydra-family.git (16) {#emailabuse-node49posteode-urlhydra-familygit}

| Nickname                                                                                            | First Seen   | Guardonly   |   Eff. Family Members |
|:----------------------------------------------------------------------------------------------------|:-------------|:------------|----------------------:|
| [Hydra94a](https://metrics.torproject.org/rs.html#details/61866162CCDFE651B0D76AA57ECA90B9CC7C80DD) | 2022-09-03   | Yes         |                    17 |
| [Hydra93a](https://metrics.torproject.org/rs.html#details/5D575ADD108DDBBF17E78AD8CB267D6C1F338206) | 2022-09-03   | Yes         |                    17 |
| [Hydra90a](https://metrics.torproject.org/rs.html#details/21328917A9379E6B8ABCB49A0DBE3AAE885CFC15) | 2022-11-02   | Yes         |                     4 |
| [Hydra91a](https://metrics.torproject.org/rs.html#details/AEC8D545DDEDC0311FA7F9F9A885D674D1F1C2FF) | 2022-07-10   | Yes         |                    17 |
| [Hydra71a](https://metrics.torproject.org/rs.html#details/9F95C68AACB67E6258EC7A6BA9406C227ABAD3F0) | 2021-09-19   | Yes         |                    16 |
| [Hydra72a](https://metrics.torproject.org/rs.html#details/FB79B2BE707F272FBFE1584F44A3FA5156F7F1CF) | 2021-09-19   | Yes         |                    16 |
| [Hydra73a](https://metrics.torproject.org/rs.html#details/391F278B2B55548B97410ADFBD055D079D798E04) | 2021-09-19   | Yes         |                    16 |
| [Hydra16](https://metrics.torproject.org/rs.html#details/1DFE397493D0791DE63F2D6EA5AB6EBCB7B9871A)  | 2020-06-09   | Yes         |                    16 |
| [Hydra18](https://metrics.torproject.org/rs.html#details/3AD29FE1241B73595F99BA2C6D830AF0B6874043)  | 2020-06-30   | Yes         |                    16 |
| [Hydra46](https://metrics.torproject.org/rs.html#details/3F14EF80BCA7D3679491EB37C98ECFB786F644AE)  | 2021-03-06   | Yes         |                    16 |
| [Hydra20](https://metrics.torproject.org/rs.html#details/86E479266EBB982E204009532ED460628689E5B5)  | 2020-10-07   | Yes         |                    16 |
| [Hydra11](https://metrics.torproject.org/rs.html#details/D9D2DBEAC776215B33E99D4EBFFE8FBA5C100DB7)  | 2021-01-13   | Yes         |                    16 |
| [Hydra17](https://metrics.torproject.org/rs.html#details/E3DAF067B028450B31CF5CE118F2F9AC53146ABD)  | 2020-06-09   | Yes         |                    16 |
| [Hydra19](https://metrics.torproject.org/rs.html#details/E465AD166798A3CD0A4866FA2A8BB5ADD157FBD5)  | 2020-06-30   | Yes         |                    16 |
| [Hydra1](https://metrics.torproject.org/rs.html#details/FF7C2604EFEE8B5898FDE1145A4CA35C8E5E5607)   | 2021-01-13   | Yes         |                    16 |
| [Hydra75](https://metrics.torproject.org/rs.html#details/63928D370B929EBDA54EF2ABDD4A63082085BF61)  | 2021-09-22   | No          |                    16 |


## Fingerprint List of Guard-only Relays in E2E Groups

1DFE397493D0791DE63F2D6EA5AB6EBCB7B9871A,21328917A9379E6B8ABCB49A0DBE3AAE885CFC15,391F278B2B55548B97410ADFBD055D079D798E04,3AD29FE1241B73595F99BA2C6D830AF0B6874043,3F14EF80BCA7D3679491EB37C98ECFB786F644AE,5D575ADD108DDBBF17E78AD8CB267D6C1F338206,61866162CCDFE651B0D76AA57ECA90B9CC7C80DD,86E479266EBB982E204009532ED460628689E5B5,9F95C68AACB67E6258EC7A6BA9406C227ABAD3F0,AEC8D545DDEDC0311FA7F9F9A885D674D1F1C2FF,D9D2DBEAC776215B33E99D4EBFFE8FBA5C100DB7,E3DAF067B028450B31CF5CE118F2F9AC53146ABD,E465AD166798A3CD0A4866FA2A8BB5ADD157FBD5,FB79B2BE707F272FBFE1584F44A3FA5156F7F1CF,FF7C2604EFEE8B5898FDE1145A4CA35C8E5E5607