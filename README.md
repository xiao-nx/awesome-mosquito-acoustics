
# 🦟 Awesome Mosquito Acoustics

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
![Status](https://img.shields.io/badge/Status-Early%20Stage-yellow)

A curated, community-maintained collection of **research papers, open datasets, AI models, benchmarks, and tools** for mosquito acoustic sensing and analysis.

Mosquito acoustics connects wingbeat biology, sensing technologies, machine learning, and field monitoring. This repository helps researchers **discover resources, compare study designs, and identify reproducible methods**.

**Status:** early-stage resource catalog (v0.1). Entries are added after checking their primary sources. Some sections are intentionally empty while curation is underway.

## Explore Resources

<table>
<tr>
<td width="50%" valign="top">

### 🗃️ [Datasets](datasets/README.md)

Open acoustic and optical wingbeat datasets, annotations, metadata, and dataset cards.

</td>
<td width="50%" valign="top">

### 🤖 [AI Models](models/README.md)

Mosquito detection, species classification, representation learning, and domain generalization.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🎯 [Benchmarks](benchmarks/README.md)

Published benchmark tasks, evaluation protocols, and reproducibility guidelines.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📚 [Publications](publications/README.md)

Curated research papers, reviews, and bibliographic references.

</td>
<td width="50%" valign="top">

### 🔧 [Tools & Hardware](tools/README.md)

Recording devices, acoustic annotation software, signal processing, and open-source tools.

</td>
</tr>
</table>

### 🦟 [Acoustic Biology](acoustic-biology/README.md)

Wingbeat characteristics, acoustic communication, mosquito behaviour, and environmental effects.

</td>
<td width="50%" valign="top">

---

## Resource Collections

### 📚 Publications

Explore the [Publications Catalog](publications/README.md), organized by research topic:

- Mosquito acoustic biology and wingbeat characteristics
- Acoustic sensing technologies
- Machine learning and deep learning
- Behavioural acoustics
- Domain generalization and robustness
- Field monitoring and surveillance
- Reviews and perspectives

**Resources:**
- [Publication Catalog](publications/README.md)
- [Machine-readable Paper Index](publications/papers.csv)
- [BibTeX References](publications/references.bib)

### 🗃️ Datasets

Explore the [Datasets Catalog](datasets/README.md), containing publicly available mosquito acoustic and wingbeat datasets.

Each dataset entry aims to document:

- Species coverage and sample size
- Recording modality and environment
- Annotation types and metadata
- Dataset provenance and version
- Available download links and licenses
- Known limitations and evaluation protocols

We distinguish **microphone-recorded airborne sound** from **optical wingbeat measurements** and document known overlap between dataset releases.

**Resources:**
- [Dataset Catalog](datasets/README.md)
- [Dataset Index](datasets/datasets.csv)

### 🤖 AI Models

Browse published AI methods by task:

- [Mosquito Detection](models/detection.md)
- [Species and Sex Classification](models/classification.md)
- [Representation Learning](models/representation-learning.md)
- [Cross-Domain Generalization](models/domain-generalization.md)
- [Uncertainty and Calibration](models/uncertainty.md)

Where available, entries include the original publication, official code, pretrained weights, datasets, and evaluation results.

**Note:** Reported model performance must be interpreted in the context of the dataset, evaluation split, and performance metric.

### 🎯 Benchmarks

Explore published benchmarks and recommended evaluation practices.

Topics include:

- Random versus group-aware data splits
- Recording- and session-level separation
- Cross-device and cross-location evaluation
- Species–domain imbalance
- Data leakage and shortcut learning
- Robustness and uncertainty assessment

**Resources:**
- [Benchmark Registry](benchmarks/README.md)
- [Evaluation Guidelines](benchmarks/evaluation-guidelines.md)


### 🔧 Tools & Hardware

Explore [Tools & Hardware](tools/README.md) for resources related to:

- Smartphone and microphone recording
- Optical wingbeat sensing
- Audio annotation and visualization
- Acoustic signal processing
- Open-source monitoring systems
- Field data collection

General-purpose tools are distinguished from systems specifically validated for mosquito acoustic research.

### 🦟 Acoustic Biology

Explore the [Acoustic Biology](acoustic-biology/README.md) collection.

Topics include:

- Wingbeat frequency and harmonic structure
- Species- and sex-associated variation
- Acoustic communication and mating behaviour
- Flight-associated acoustic activity
- Temperature and physiological effects

The collection distinguishes observed biological associations from independently validated behavioural prediction.

---

## Related Projects

**Acoustic Ecological Inference**

A separate, planned research repository focusing on statistical inference from imperfect acoustic observations, including ecological observation models, uncertainty propagation, identifiability, and calibration.

---

## Contributing

Contributions from the research community are welcome!
