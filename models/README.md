
# AI Models for Mosquito Acoustic Analysis

A curated catalog of machine learning and deep learning models for mosquito acoustic detection, species identification, representation learning, domain generalization, and behavioural analysis.

## Contents

- [1. Model Overview](#1-model-overview)
- [2. Mosquito Detection](#2-mosquito-detection)
- [3. Species and Sex Classification](#3-species-and-sex-classification)
- [4. Representation Learning](#4-representation-learning)
- [5. Domain Generalization](#5-domain-generalization)
- [6. Uncertainty and Reliability](#6-uncertainty-and-reliability)
- [7. Behavioural Recognition](#7-behavioural-recognition)
- [8. Evaluation Guidelines](#8-evaluation-guidelines)
- [9. Contributing](#9-contributing)

## 1. Model Overview

The catalog covers models directly evaluated on mosquito acoustic or wingbeat-sensing data.

Models are organized by their primary research tasks rather than neural network architecture alone.

| Model / Study | Year | Primary Task | Method | Source |
|---|---|---|---|---|
| Mukundarajan et al. | 2017 | Species identification | Frequency-based statistical classification | [Paper](https://doi.org/10.7554/eLife.27854) |
| Kiskin et al. | 2018/2020 | Mosquito detection | Wavelet-conditioned CNN | [Paper](https://doi.org/10.1007/s00521-018-3626-7) |
| Fernandes et al. | 2021 | Aedes aegypti detection | Spectrogram CNN / Ensemble | [Paper](https://doi.org/10.1016/j.compbiomed.2020.104152) |
| HumBugDB models | 2021 | Detection / Classification | Bayesian neural networks and related pipelines | [Code](https://github.com/HumBug-Mosquito/HumBugDB) |
| MozzBNN | — | Mosquito detection | Bayesian CNN | [Code](https://github.com/HumBug-Mosquito/MozzBNN) |
| WbNet | 2022 | Species classification | ResNet-18 + Self-attention | [Paper](https://doi.org/10.1038/s41598-022-14372-x) · [Code](https://github.com/xutong30/WbNet-ResNet-Attention) |
| MosquitoSong+ | 2024 | Species / Sex classification | Noise-augmented 1D CNN | [Paper](https://doi.org/10.1371/journal.pone.0310121) · [Code](https://github.com/akaraspt/mosquitosongp) |
| BioDCASE CD-MSC baseline | 2026 | Cross-domain species classification | MTRCNN | [Challenge](https://biodcase.github.io/challenge2026/task5) · [Code](https://github.com/Yuanbo2020/CD-MSC) |

**Notes**

- The year refers to the publication year where available.
- Kiskin et al. was first published online in 2018 and appeared in the 2020 journal volume.
- HumBugDB and MozzBNN are related resources; they should not be counted as independent published algorithms without checking their underlying methods.
- Missing code links do not necessarily mean that no implementation exists.
- Performance results from different datasets or validation protocols are not directly comparable.

## 2. Mosquito Detection

**Task:** Identify mosquito-generated acoustic signals in recordings containing background noise and other sound sources.

### 2.1 Wavelet-conditioned CNN

**Reference:** Kiskin et al. (2018/2020)

**Paper:** [Bioacoustic detection with wavelet-conditioned convolutional neural networks](https://doi.org/10.1007/s00521-018-3626-7)

- **Input:** Wavelet representations of acoustic recordings
- **Method:** Convolutional neural network
- **Task:** Mosquito presence detection
- **Contribution:** Comparison of learned acoustic features against conventional handcrafted representations
- **Limitation:** Results depend on available recordings and the evaluated detection conditions

### 2.2 CNN-based Aedes aegypti Detection

**Reference:** Fernandes et al. (2021)

**Paper:** [Detecting Aedes aegypti mosquitoes through audio classification with convolutional neural networks](https://doi.org/10.1016/j.compbiomed.2020.104152)

- **Input:** Spectrograms derived from wingbeat recordings
- **Method:** Binary CNN, multiclass CNN, ensemble of binary classifiers
- **Task:** Identification of Aedes aegypti
- **Contribution:** Comparison of different CNN-based detection strategies
- **Limitation:** Reported performance should be interpreted within the study's original evaluation conditions

### 2.3 HumBug Bayesian Acoustic Detection

**Resources:**

- [HumBugDB](https://github.com/HumBug-Mosquito/HumBugDB)
- [MozzBNN](https://github.com/HumBug-Mosquito/MozzBNN)

The HumBug project provides mosquito acoustic detection and classification resources, including Bayesian neural-network-based methods.

Relevant tasks include:

- Mosquito event detection
- Species classification
- Processing large collections of field recordings
- Identifying candidate mosquito-containing segments

The repositories provide code and usage information. Dataset access and reproduction requirements should be checked against the original documentation.

## 3. Species and Sex Classification

**Task:** Assign mosquito acoustic recordings to species, sex, or other validated taxonomic categories.

### 3.1 Frequency-based Statistical Classification

**Reference:** Mukundarajan et al. (2017)

**Paper:** [Using mobile phones as acoustic sensors for high-throughput mosquito surveillance](https://doi.org/10.7554/eLife.27854)

- **Input:** Smartphone-recorded wingbeat signals
- **Method:** Frequency-distribution-based statistical classification
- **Task:** Mosquito species identification
- **Contribution:** Demonstrated low-cost acoustic sensing and species identification using mobile phones
- **Dataset:** [Dryad](https://doi.org/10.5061/dryad.98d7s)

### 3.2 WbNet — ResNet with Attention

**Reference:** Wei et al. (2022)

**Paper:** [A ResNet attention model for classifying mosquitoes from wing-beating sounds](https://doi.org/10.1038/s41598-022-14372-x)

**Code:** [WbNet-ResNet-Attention](https://github.com/xutong30/WbNet-ResNet-Attention)

- **Input:** Mel-spectrograms
- **Architecture:** ResNet-18 with self-attention
- **Task:** Six-species classification
- **Datasets:** WINGBEATS and ABUZZ
- **Reported accuracy:** 89.9% on WINGBEATS and 98.9% on ABUZZ
- **Limitation:** The reported values correspond to the study's evaluation protocols and should not be treated as cross-domain benchmark results

### 3.3 MosquitoSong+

**Reference:** Supratak et al. (2024)

**Paper:** [MosquitoSong+: A noise-robust deep learning model for mosquito classification from wingbeat sounds](https://doi.org/10.1371/journal.pone.0310121)

**Code:** [mosquitosongp](https://github.com/akaraspt/mosquitosongp)

- **Input:** Raw wingbeat audio
- **Architecture:** Modified 1D convolutional neural network
- **Task:** Species and sex classification
- **Techniques:** Environmental noise augmentation and wingbeat amplitude variation
- **Reported result:** 93.3% species-and-sex classification accuracy in the paper's noise-overlay evaluation
- **Limitation:** Performance under simulated background-noise conditions does not establish generalization to independent real-world deployments

## 4. Representation Learning

This category focuses on methods that learn reusable acoustic representations rather than relying exclusively on handcrafted features.

### Relevant approaches

- Transfer learning from pretrained audio models
- Self-supervised acoustic representation learning
- Contrastive learning
- Few-shot adaptation
- Active learning for acoustic annotation

### Mosquito-specific evidence

The WbNet study includes transfer learning with ResNet models. However, its main contribution is supervised species classification, rather than a general-purpose mosquito acoustic foundation model.

[WbNet paper](https://doi.org/10.1038/s41598-022-14372-x)

### Research opportunities

Important directions include:

1. Evaluating pretrained audio representations on mosquito recordings.
2. Comparing frozen embeddings against end-to-end fine-tuning.
3. Testing generalization across recording devices and environments.
4. Investigating whether embeddings encode species-related, environmental, or acquisition-domain information.
5. Evaluating label efficiency under independent target-domain testing.

Models developed only for other animal taxa should be listed separately as candidate transferable models until mosquito-specific validation is available.

## 5. Domain Generalization

**Task:** Maintain reliable mosquito acoustic classification when acquisition conditions change.

Relevant domain shifts include:

- Recording device
- Location and environmental context
- Laboratory versus field acquisition
- Recording session
- Species–domain combinations

### 5.1 BioDCASE 2026 CD-MSC Baseline

**Paper:** [BioDCASE 2026 Challenge Baseline](https://arxiv.org/abs/2603.20118)

**Challenge:** [Cross-Domain Mosquito Species Classification](https://biodcase.github.io/challenge2026/task5)

**Code:** [CD-MSC](https://github.com/Yuanbo2020/CD-MSC)

**Dataset:** [Zenodo](https://doi.org/10.5281/zenodo.20478577)

- **Task:** Closed-set mosquito species classification under domain shift
- **Species:** 9
- **Domains:** 5
- **Architecture:** Multi-temporal Resolution CNN (MTRCNN)
- **Input:** 64-bin log-mel spectrograms
- **Sampling rate:** 8 kHz
- **Outputs:** Species classification and auxiliary domain classification
- **Released resources:** Training scripts, evaluation scripts, configurations and checkpoints

The official development-split baseline reports:

| Checkpoint | BA Seen | BA Unseen |
|---|---:|---:|
| Best validation | 0.8806 ± 0.0108 | 0.1751 ± 0.0197 |
| Final | 0.8822 ± 0.0097 | 0.1704 ± 0.0180 |

These values refer to the challenge's reported development test split, not an independently established universal performance level.

**Important:** The task's "unseen domain" includes species–domain combinations absent from training, even when the domain itself occurs in other training species.

### Suggested evaluation dimensions

- Seen-domain performance
- Unseen-domain performance
- Species-balanced accuracy
- Domain shift gap
- Per-species recall
- Class imbalance
- Training/test recording independence

## 6. Uncertainty and Reliability

Reliable acoustic monitoring requires more than accurate hard-label predictions.

Relevant topics include:

- Bayesian neural networks
- Predictive probability calibration
- Classification confidence
- Out-of-distribution detection
- Selective classification
- False-positive and false-negative analysis

### Mosquito-specific resources

**HumBug / MozzBNN**

[Repository](https://github.com/HumBug-Mosquito/MozzBNN)

Provides a Bayesian convolutional neural network pipeline for mosquito acoustic prediction.

### Evaluation considerations

Recommended metrics include:

- Precision and recall
- False positives per recording hour
- Negative log-likelihood
- Brier score
- Expected calibration error
- Performance under domain shift
- Risk–coverage curves for selective prediction

A Bayesian architecture alone does not guarantee reliable uncertainty estimates. Probability calibration and error detection must be evaluated empirically.

## 7. Behavioural Recognition

**Task:** Identify mosquito behavioural states from validated acoustic observations.

Potential research targets include:

- Flight activity and flight bouts
- Mating interactions
- Harmonic convergence
- Behaviour-associated wingbeat modulation

### Evidence status

Acoustic correlates of mosquito reproductive behaviour and flight dynamics have been studied. However, a biological association between a sound feature and a behaviour does not establish reliable automated behavioural classification.

This catalog does not currently designate a model as a validated, general-purpose mosquito behavioural classifier.

### Minimum requirements for model inclusion

A behavioural model should document:

1. The target behavioural state.
2. Independent behavioural annotations.
3. Acoustic recording conditions.
4. Evaluation across independent individuals or sessions.
5. Performance against suitable baselines.
6. Known confounding factors and deployment limitations.

## 8. Evaluation Guidelines

Model performance should always be interpreted in relation to its evaluation protocol.

| Evaluation level | Recommended protocol |
|---|---|
| Within-dataset | Clearly documented train/test split |
| Recording-level | Separate recording sessions |
| Individual-level | Separate individual mosquitoes |
| Device-level | Hold out recording devices |
| Location-level | Hold out acquisition sites |
| Domain generalization | Hold out acquisition domains or species–domain combinations |
| Field validation | Evaluate on independent operational recordings |

### Reporting checklist

When contributing a model, report:

- Dataset version
- Recording modality
- Species and sex coverage
- Input representation
- Preprocessing
- Model architecture
- Training/validation/test protocol
- Primary evaluation metrics
- Code and checkpoint availability
- Hardware and computation requirements, when available
- Known limitations

**Do not compare model accuracy across unrelated datasets or incompatible splits as if they were leaderboard results.**

## 9. Contributing

Contributions of published models, verified implementations, and corrections are welcome.

Please see [CONTRIBUTING.md](../CONTRIBUTING.md).
