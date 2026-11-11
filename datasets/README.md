# Mosquito Acoustic Dataset Catalog

A curated registry of open mosquito acoustic and optical wingbeat resources for machine learning, acoustic biology, and field monitoring. **Catalog version: 0.1 (11 November 2026).**

> **Important:** optical wingbeat time series are not airborne microphone recordings. Audio clips, optical segments, label votes, and total durations are different units; do not compare dataset sizes directly or assume datasets are independent.

## Datasets

| Dataset | Year | Modality | Scale | Primary uses | Details |
|---|---|---|---|---|---|
| WINGBEATS / MosquitoSound | 2017 | Optical | 279,566 segments; 6 species | Species classification | [Card](wingbeats-mosquitosound.md) |
| Vasconcelos et al. | 2020 | Microphone | 3 reported taxonomic groups | Recognition, acoustic features | [Card](vasconcelos-2020.md) |
| HumBug Zooniverse | 2020 | Microphone | 80,101 overlapping 2 s clips; 195,434 annotations | Mosquito event detection | [Card](humbug-zooniverse.md) |
| HumBugDB | 2021 | Microphone | 71,286 s labelled mosquito audio; 36 species/complexes (species-labelled subset) | Detection, classification | [Card](humbugdb.md) |
| BioDCASE CD-MSC | 2026 | Acoustic | 271,380 development clips; 60.66 h; 9 species; 5 domains | Cross-domain classification | [Card](biodcase-cd-msc-2026.md) |
| Augustin et al. | 2026 | Acoustic traits | 15 recorded species in analysis | Biological/environmental wingbeat effects | [Card](augustin-2026.md) |

## Browse by task

- **Detection:** HumBug Zooniverse, HumBugDB
- **Species classification:** WINGBEATS/MosquitoSound, Vasconcelos et al., HumBugDB, BioDCASE CD-MSC
- **Cross-domain generalization:** BioDCASE CD-MSC; HumBugDB can support custom analyses with carefully defined splits
- **Wingbeat biology and environmental variation:** Augustin et al.; Vasconcelos et al.

## Contributing

Please supply the official data URL, publication, dataset version, modality, annotation unit, validated quantities, licensing information, and any known provenance overlap. Propose updates via pull requests.
