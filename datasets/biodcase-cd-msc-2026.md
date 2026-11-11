# BioDCASE 2026 CD-MSC

**Dataset ID:** `biodcase2026`  
**Year:** 2026  
**Modality:** mosquito acoustic recordings  
**Environment:** 5 acquisition domains  
**Main tasks:** cross-domain species classification

## Description

Official 2026 cross-domain mosquito species classification benchmark. Development release: 271,380 clips (218,388.40 s = 60.66 h), nine species, five domains. Domain distribution D1=4,065; D2=784; D3=679; D4=200; D5=265,652, so the dataset is highly imbalanced. Development filenames encode species and domain IDs; the released evaluation filenames are anonymized. The official evaluation set is not a training/validation set. Metrics include balanced accuracy on unseen-domain samples (primary) and the domain shift gap. Follow the organizers' specific split and leakage precautions.

## Catalog metadata

- **Sample count:** 271380
- **Duration:** 60.66 development audio hours
- **Species:** 9
- **Annotations:** species and domain IDs (development)
- **Data format / metadata:** WAV clips; official split metadata
- **Known limitations:** D5=265652/271380 clips; evaluation set restricted to evaluation use
- **License status:** license check selected Zenodo version. Inspect the chosen dataset version and the original repository before redistribution.

## Access and citations

- [Data / official archive](https://doi.org/10.5281/zenodo.20478577)
- [Paper / source](https://arxiv.org/abs/2603.20118)
- [Associated code](https://github.com/Yuanbo2020/CD-MSC)

## Reuse checklist

- [ ] Verify archive version and download access
- [ ] Verify data license / attribution requirements
- [ ] Inspect sample-level and biological-unit identifiers
- [ ] Check overlap with other resources
- [ ] Use grouped evaluation when the necessary metadata exists
