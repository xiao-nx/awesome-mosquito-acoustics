# 🦟 Awesome Mosquito Acoustics

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated, community-maintained collection of **research papers, open datasets, AI models, benchmarks, and tools** for mosquito acoustic sensing and analysis.

Mosquito acoustics connects wingbeat biology, sensing technologies, machine learning, and field monitoring. This repository helps researchers **discover resources, compare study designs, and identify reproducible methods**. It is a research resource catalog—not a repository of third-party audio files, model weights, or copyrighted papers.

**Status:** early-stage resource catalog (v0.1). Entries are added after checking their primary sources. Some sections are intentionally empty while curation is underway.

## Contents

- [Publications](publications/README.md) — research articles, reviews, and references
- [Datasets](datasets/README.md) — datasets, annotations, provenance, and dataset cards
- [AI Models](models/README.md) — detection, classification, representation learning, domain shift, and uncertainty
- [Benchmarks](benchmarks/README.md) — published benchmark tasks and evaluation guidelines
- [Acoustic Biology](acoustic-biology/README.md) — wingbeat signatures, behaviour, environmental effects
- [Tools & Hardware](tools/README.md) — acquisition, annotation, processing, and deployment tools
- [Contributing](CONTRIBUTING.md) — submit a resource or correction

## Scope

| Included | Outside this repository's scope |
| --- | --- |
| Mosquito acoustic and optical wingbeat datasets, clearly distinguished by sensing modality | Rehosting datasets without redistribution permission |
| Published acoustic detection/classification methods and links to official implementations | Full training projects and large model checkpoints |
| Behaviour-related mosquito acoustic biology and direct empirical evidence | Treating acoustic detection counts as validated mosquito abundance |
| Published benchmark descriptions and transparent evaluation recommendations | Claims of comparable model accuracy across incompatible datasets/splits |
| Links to relevant external methodological projects | Full ecological-inference model development (separate project) |

## Explore the resources

### 📚 Publications

Browse papers by topic (acoustic biology, sensing, ML/DL, behavioural acoustics, domain generalization, and field monitoring) in the [publication catalog](publications/README.md). The machine-readable index is [`publications/papers.csv`](publications/papers.csv) and bibliographic entries can be stored in [`publications/references.bib`](publications/references.bib).

### 🗃️ Datasets

Browse the [dataset catalog](datasets/README.md), with one source-checked record per dataset/release and optional detailed cards. We distinguish **microphone-recorded airborne sound** from **optical wingbeat measurements** and document any known overlap between dataset releases.

### 🤖 AI Models

Browse [model methods by task](models/README.md):

- [Detection](models/detection.md)
- [Species and sex classification](models/classification.md)
- [Representation learning](models/representation-learning.md)
- [Cross-domain generalization](models/domain-generalization.md)
- [Uncertainty and calibration](models/uncertainty.md)

A model's reported performance must always be accompanied by its dataset, split, metric, and source.

### 🎯 Benchmarks

See [benchmark registry](benchmarks/README.md) and [evaluation guidelines](benchmarks/evaluation-guidelines.md) for recording/session separation, cross-device tests, class imbalance, and leakage-aware evaluation.

### 🦟 Acoustic Biology

See [acoustic biology](acoustic-biology/README.md) for biological interpretation of wingbeat signals and the distinction between observed associations and independently validated behavioural prediction.

### 🔧 Tools & Hardware

See [tools](tools/README.md) for recording hardware, annotation software, signal processing, and open-source implementations.

## Resource quality principles

1. **Source first:** link primary papers, official repositories, and original dataset access pages.
2. **Verify claims:** do not infer licenses, datasets, code availability, or validation procedures.
3. **Preserve provenance:** identify dataset versions, possible overlap, original labels, and recording modality.
4. **Report evaluation context:** performance numbers are meaningless without dataset, split, and metric.
5. **Separate evidence levels:** distinguish direct mosquito studies, methods validated in other taxa, and future proposals.
6. **Respect third-party rights:** link external materials rather than redistributing files without permission.

## Contributing

Suggestions, corrections, and new resources are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) or open an issue using the resource templates. Every submitted entry should have a verifiable primary source.

## Related projects

- **Acoustic Ecological Inference:** a separate, planned methods/code repository for statistical inference from imperfect acoustic observations. A verified link will be added when it becomes available.

## Citation and license

To cite this catalog, see [`CITATION.cff`](CITATION.cff). Cite **original dataset and model creators** directly whenever using their resources. Original text and repository-maintained code are offered under the [MIT License](LICENSE); upstream resources retain their own licenses and rights.

## Maintainers

Maintained by community contributors. To request a correction, use [GitHub Issues](../../issues).

<!-- MAINTAINER SETUP: Add the workflow badge after the repository URL is known. -->
