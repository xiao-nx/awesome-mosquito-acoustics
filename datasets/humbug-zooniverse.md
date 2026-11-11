# HumBug Zooniverse

**Dataset ID:** `humbugzooniverse2020`  
**Year:** 2020  
**Modality:** airborne audio microphone  
**Environment:** four collection groups  
**Main tasks:** mosquito detection

## Description

Crowd-sourced mosquito presence annotations covering 80,101 overlapping 2-second clips (~22 hours unique audio) and 195,434 volunteer classifications. Annotations are votes rather than unique recordings, with `yes`, `no`, `not_sure` categories. The project provides a processed non-overlapping 1-second version and recommends it for modelling. Annotation disagreement, label aggregation, clip overlap, class imbalance, and related HumBug recording provenance require care.

## Catalog metadata

- **Sample count:** 80101
- **Duration:** ~22 unique audio hours (overlapping windows)
- **Species:** Not applicable / not verified
- **Annotations:** 195434 crowd annotations; yes/no/not_sure
- **Data format / metadata:** overlapping 2 s clips; recommended non-overlap 1 s
- **Known limitations:** Annotator disagreements; overlapping clips; possible related HumBug recordings
- **License status:** license check at source. Inspect the chosen dataset version and the original repository before redistribution.

## Access and citations

- [Data / official archive](https://github.com/HumBug-Mosquito/ZooniverseData)
- [Paper / source](https://doi.org/10.1109/ICASSP40776.2020.9053141)
- [Associated code](https://github.com/HumBug-Mosquito/ZooniverseData)

## Reuse checklist

- [ ] Verify archive version and download access
- [ ] Verify data license / attribution requirements
- [ ] Inspect sample-level and biological-unit identifiers
- [ ] Check overlap with other resources
- [ ] Use grouped evaluation when the necessary metadata exists
