# 🏆 Mosquito Acoustic Benchmarks

A curated index of **published benchmarks**, reusable datasets, and evaluation guidance for mosquito acoustic AI. A public dataset is **not automatically an official benchmark**; compare model scores only when their data splits and evaluation rules are compatible.

## Established benchmarks

| Benchmark | Year | Task | Scale | Official evaluation | Resources |
|---|---|---|---|---|---|
| **BioDCASE CD-MSC (Task 5)** | 2026 | Cross-domain mosquito species classification | 9 species · 5 domains · 271,380 clips (development data) | **BA_unseen** (primary); domain shift gap, **DSG** (secondary) | [Challenge](https://biodcase.github.io/challenge2026/task5) · [Development data](https://zenodo.org/records/19095788) · [Evaluation data](https://zenodo.org/records/20478577) · [Baseline code](https://github.com/Yuanbo2020/CD-MSC) |

*CD-MSC defines “unseen-domain” at the **species–domain combination** level: a domain may be represented during training for other species. The official challenge uses balanced accuracy on unseen-domain samples for ranking; DSG = |BA_unseen − BA_seen|.*

## Other datasets used for evaluation

| Dataset | Modality | Common tasks | Note |
|---|---|---|---|
| WINGBEATS / MosquitoSound | Optical wingbeat sensing | Species classification | Related releases; check provenance and split independence |
| HumBug Zooniverse | Microphone audio | Mosquito presence / detection | Overlapping clips and crowd-sourced annotations |
| HumBugDB | Microphone audio | Detection and species classification | Strong variation in species, location and recording device |

These are **dataset resources**, not additional official benchmarks in this registry. See the [Dataset Catalog](../datasets/README.md) for authoritative source links, licenses and metadata.

## Evaluation essentials

- **Splits:** Prefer independent recording/session/individual splits; use held-out devices or sites for deployment claims.
- **Classification:** Report balanced accuracy, macro-F1 and per-species confusion; include per-domain results when relevant.
- **Detection:** Report precision/recall, event-level metrics and false positives per recording hour for continuous monitoring.
- **Reliability:** Assess calibration and unknown-condition performance where the task warrants it.
- **Reproducibility:** Document dataset version, grouping keys, preprocessing, official vs custom split, seeds and metric implementation.

Read the [Evaluation Guidelines](evaluation-guidelines.md) for detailed recommendations. Machine-readable entries are in [benchmark-registry.csv](benchmark-registry.csv).

## Contributing

Submit a published benchmark or a correction via pull request with its **official task page, citation, data/split definition, evaluation metrics, code and license**. Clearly label custom protocols rather than presenting them as organizer-approved benchmarks. See [CONTRIBUTING](../CONTRIBUTING.md).

[← Back to main repository](../README.md)
