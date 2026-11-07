# hri-audio references

| Requirement | Sources |
|---|---|
| AUD-001 Level limit | WHO & ITU 2022 (H.870) |
| AUD-002 No abrupt changes | Supports Principle I; no single source |
| AUD-003 Continuity | Supports Principle VI (see hri-core references) |
| AUD-004 Sync | ITU-R BT.1359 |
| AUD-005 State → sound mapping | Eerola et al. 2013; Juslin & Laukka 2004 |
| AUD-006 Acoustic context | Supports Principle II (see hri-core references) |

## Notes

- H.870 sets a weekly reference dose of 1.6 Pa²h for adults (≈ 80 dBA for 40 h/week) and
  0.51 Pa²h for children/sensitive users (≈ 75 dBA for 40 h/week). It targets personal audio
  devices; for loudspeakers, use it as a conservative reference.
- BT.1359 detectability thresholds (≈ 45 ms audio lead to 125 ms audio lag) were measured with
  speech/lip-sync material; other content may tolerate more or less.
- Eerola et al. measured *perceived* emotion: mode and tempo were the strongest cues, mostly
  additive. Perceived emotion is not the same as emotion *induced* in the listener
  (Juslin & Laukka 2004).

## Full references

- Eerola, T., Friberg, A., & Bresin, R. (2013). Emotional expression in music: Contribution, linearity, and additivity of primary musical cues. *Frontiers in Psychology, 4*, 487. https://doi.org/10.3389/fpsyg.2013.00487
- ITU-R (1998). *Recommendation BT.1359-1: Relative timing of sound and vision for broadcasting*. International Telecommunication Union.
- ITU-T (2022). *Recommendation H.870 (03/2022): Guidelines for safe listening devices/systems*. International Telecommunication Union. https://www.itu.int/rec/T-REC-H.870
- Juslin, P. N., & Laukka, P. (2004). Expression, perception, and induction of musical emotions: A review and a questionnaire study of everyday listening. *Journal of New Music Research, 33*(3), 217–238. https://doi.org/10.1080/0929821042000317813
