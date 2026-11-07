# hri-vision references

| Requirement | Sources |
|---|---|
| People in frame / VIS-004 Camera privacy | Butler et al. 2015; Rueben et al. 2018 (see hri-core) |
| Deployment context | Regulation (EU) 2024/1689, Art. 5(1)(f) |
| VIS-001 Capture conditions | Li & Deng 2020 |
| VIS-002 Validity and uncertainty of inference | Barrett et al. 2019 (see hri-core); Li & Deng 2020 |
| VIS-003 Fairness | Buolamwini & Gebru 2018 |

## Notes

- Barrett et al. (2019) show that emotional states cannot be reliably read from facial
  configurations alone; treat any visual inference of internal state as an estimate.
- Li & Deng (2020) identify illumination, head pose and identity bias as key problems for facial
  expression recognition outside the lab.
- Buolamwini & Gebru (2018) found error rates up to 34.7% for darker-skinned women versus 0.8%
  for lighter-skinned men in commercial gender classifiers: subgroup evaluation is necessary.
- The EU AI Act prohibits AI systems that infer emotions in workplaces and education institutions,
  except for medical or safety reasons. Check the primary text and Commission guidelines for scope.

## Full references

- Buolamwini, J., & Gebru, T. (2018). Gender shades: Intersectional accuracy disparities in commercial gender classification. *Proceedings of the 1st Conference on Fairness, Accountability and Transparency*, PMLR 81, 77–91. https://proceedings.mlr.press/v81/buolamwini18a.html
- Butler, D. J., Huang, J., Roesner, F., & Cakmak, M. (2015). The privacy-utility tradeoff for remotely teleoperated robots. *HRI 2015*, 27–34. https://doi.org/10.1145/2696454.2696484
- Li, S., & Deng, W. (2020). Deep facial expression recognition: A survey. *IEEE Transactions on Affective Computing*. https://doi.org/10.1109/TAFFC.2020.2981446
- Regulation (EU) 2024/1689 of the European Parliament and of the Council (Artificial Intelligence Act), Article 5(1)(f). *Official Journal of the European Union*. https://eur-lex.europa.eu/eli/reg/2024/1689/oj
