# AI Model Catalog

[← Awesome Mosquito Acoustics](../README.md)

A curated index of **published mosquito acoustic and optical-wingbeat AI models**, their research tasks, original evidence, open implementations and evaluation limitations. Models are indexed by **task**, not ranked by accuracy across incompatible datasets.

## Browse by task

| Category | Content |
|---|---|
| [Detection](detection.md) | Mosquito-vs-background and acoustic event localization |
| [Classification](classification.md) | Species, genus and sex prediction |
| [Representation Learning](representation-learning.md) | Transfer learning and mosquito-validated robust representations |
| [Domain Generalization](domain-generalization.md) | Transfer between devices, environments and species–domain combinations |
| [Uncertainty & Reliability](uncertainty.md) | Bayesian outputs, probability calibration and selective prediction |
| [Behavioural Recognition](behavioural-recognition.md) | Behavioural state models and evidence requirements |

## Model index

The structured [models.csv](models.csv) is the main machine-readable index; each record has a stable `model_id` and links to original sources. Empty fields mean **not verified or not supplied**, never confirmed absence.

| Model / system | Main task | Year | Public code | Details |
|---|---|---:|---|---|
| Frequency-based classification — Mukundarajan et al. | Species identification | 2017 | Not verified | [Classification](classification.md) |
| Wavelet-conditioned CNN — Kiskin et al. | Detection | 2018/2020 | Not verified | [Detection](detection.md) |
| CNN approaches — Fernandes et al. | *Aedes aegypti* identification | 2021 | Not verified | [Detection](detection.md) |
| HumBug / MozzBNN | Detection and species prediction | 2021-era | [GitHub](https://github.com/HumBug-Mosquito/MozzBNN) | [Uncertainty](uncertainty.md) |
| WbNet | Species classification | 2022 | [GitHub](https://github.com/xutong30/WbNet-ResNet-Attention) | [Classification](classification.md) |
| MosquitoSong+ | Species and sex classification | 2024 | [GitHub](https://github.com/akaraspt/mosquitosongp) | [Classification](classification.md) |
| DR-BioL | Cross-domain representations | 2026 | Not verified | [Domain Generalization](domain-generalization.md) |
| BioDCASE CD-MSC MTRCNN baseline | Cross-domain classification | 2026 | [GitHub](https://github.com/Yuanbo2020/CD-MSC) | [Domain Generalization](domain-generalization.md) |

## Interpretation rules

- **Species recognition is not mosquito detection**: different targets, negative examples and evaluation units.
- **Optical wingbeat measurements and airborne microphone audio are distinct sensing modalities.**
- Accuracy in one paper is **not** directly comparable to accuracy in another dataset or split.
- Software repositories may contain **multiple model versions**; pin the original checkpoint for reproducibility.
- An architecture with Bayesian layers does not automatically demonstrate calibrated uncertainty.
- Behavioural associations are not automatically validated behavioural recognition models.

## Submit a model

Please provide paper/DOI, task and species coverage, signal modality, input preprocessing, data split, numerical metric and evaluation unit, source code, weights, licence and limitations. See [CONTRIBUTING.md](../CONTRIBUTING.md).

## Evidence and verification

This catalog is an initial curated release. Entries use original publications and publicly documented project repositories. Repository availability is not a claim that instructions have been executed or results reproduced. Publication/repository URLs and key model descriptions were checked in November 2026; incomplete fields are explicitly left blank in CSV. Performance is omitted from the cross-study overview to avoid misleading comparisons.
