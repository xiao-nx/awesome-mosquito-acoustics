# Mosquito Acoustic Dataset Catalog

A curated registry of open mosquito acoustic and optical wingbeat resources for machine learning, acoustic biology, and field monitoring. **Catalog version: 0.1 (11 November 2026).**

> **Important:** optical wingbeat time series are not airborne microphone recordings. Audio clips, optical segments, label votes, and total durations are different units; do not compare dataset sizes directly or assume datasets are independent.

## Datasets

| Dataset | Year | Modality | Scale | Primary uses | Details |
|---|---|---|---|---|---|
| WINGBEATS / MosquitoSound | Source 2017; archive 2026 | Optical | 279,566 segments; 6 species | Species classification | [Card](cards/wingbeats-mosquitosound.md) |
| Vasconcelos et al. | 2020 | Microphone | 3 reported taxonomic groups | Recognition, acoustic features | [Card](cards/vasconcelos-2020.md) |
| HumBug Zooniverse | 2020 | Microphone | 80,101 overlapping 2 s clips; 195,434 annotations | Mosquito event detection | [Card](cards/humbug-zooniverse.md) |
| HumBugDB | 2021 | Microphone | 71,286 s labelled mosquito audio; 36 species/complexes (species-labelled subset) | Detection, classification | [Card](cards/humbugdb.md) |
| BioDCASE CD-MSC | 2026 | Acoustic | 271,380 development clips; 60.66 h; 9 species; 5 domains | Cross-domain classification | [Card](cards/biodcase-cd-msc-2026.md) |
| Augustin et al. | 2026 | Acoustic traits | 15 recorded species in analysis | Biological/environmental wingbeat effects | [Card](cards/augustin-2026.md) |

## Browse by task

- **Detection:** HumBug Zooniverse, HumBugDB
- **Species classification:** WINGBEATS/MosquitoSound, Vasconcelos et al., HumBugDB, BioDCASE CD-MSC
- **Cross-domain generalization:** BioDCASE CD-MSC; HumBugDB can support custom analyses with carefully defined splits
- **Wingbeat biology and environmental variation:** Augustin et al.; Vasconcelos et al.

## How to choose a dataset

1. Specify your measurement modality: optical wingbeat sensing vs airborne acoustics.
2. Confirm the prediction unit: raw recording, overlapping clip, independent event, or biological individual.
3. Check metadata and grouping variables (individual/session/device/site) before splitting.
4. Prefer grouped and external evaluation for real-world generalization claims.
5. Inspect dataset rights before copying or redistributing recordings; public download does not automatically imply a reusable license.
6. Check overlaps or derivatives before combining resources (especially WINGBEATS/MosquitoSound and HumBug-related resources).

## Metadata schema

The canonical machine-readable index is [`datasets.csv`](datasets.csv). Missing values mean *not confirmed in this catalog*, not necessarily absent from the underlying dataset. For each dataset, its card tracks scope, data access, annotation units, limitations, and sources.

## Curation rules

- Prefer publisher, official project, and original archive records.
- Report provenance and release/version information separately from publication year.
- Do not represent annotation votes as unique sound files.
- Avoid comparing models evaluated on different splits directly.
- Mark unchecked license details as **license check required** rather than assuming a blanket open-data license.
- This repository indexes data; it does not redistribute original audio.

## Sources and official links

- [MosquitoSound archive description](https://www.timeseriesclassification.com/description.php?Dataset=MosquitoSound) · [Zenodo release](https://doi.org/10.5281/zenodo.18681520
        
        
        
        )
- [Vasconcelos et al. data](https://doi.org/10.6084/m9.figshare.11902125
        
        
        
        ) · [paper](https://doi.org/10.1038/s41597-020-00725-6
        
        
        
        )
- [HumBug Zooniverse project](https://github.com/HumBug-Mosquito/ZooniverseData) · [paper](https://doi.org/10.1109/ICASSP40776.2020.9053141
        
        
        
        )
- [HumBugDB Zenodo](https://doi.org/10.5281/zenodo.4904800
        
        
        
        ) · [official code](https://github.com/HumBug-Mosquito/HumBugDB)
- [BioDCASE CD-MSC Zenodo v2](https://doi.org/10.5281/zenodo.20478577
        
        
        
        ) · [challenge](https://biodcase.github.io/challenge2026/task5) · [baseline](https://github.com/Yuanbo2020/CD-MSC)
- [Augustin et al. research data](https://doi.org/10.6084/m9.figshare.30230581
        
        
        
        ) · [paper](https://doi.org/10.1371/journal.pone.0343060
        
        
        
        )

## Contributing

Please supply the official data URL, publication, dataset version, modality, annotation unit, validated quantities, licensing information, and any known provenance overlap. Propose updates via pull requests.

