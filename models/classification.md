# Mosquito Species and Sex Classification

[← Model Catalog](README.md)

**Scope.** Models that infer mosquito species, genus or sex from optical wingbeat measurements or airborne audio. These modalities must be identified separately.

| Study / model | Year | Input / model | Task | Resources | Evidence notes |
|---|---|---|---|---|---|
| Mukundarajan et al. | 2017 | Smartphone audio; wingbeat-frequency statistical classification | Species identification | [Paper](https://doi.org/10.7554/eLife.27854) · [Data](https://doi.org/10.5061/dryad.98d7s) | Frequency distributions overlap; mobile sampling context matters |
| WbNet (Wei et al.) | 2022 | Mel spectrogram; ResNet-18 + self-attention | Species classification | [Paper](https://doi.org/10.1038/s41598-022-14372-x) · [Code](https://github.com/xutong30/WbNet-ResNet-Attention) | WINGBEATS and ABUZZ evaluations; no cross-study leaderboard comparison |
| MosquitoSong+ (Supratak et al.) | 2024 | Raw wingbeat audio; noise-augmented 1D CNN | Species and sex classification | [Paper](https://doi.org/10.1371/journal.pone.0310121) · [Code](https://github.com/akaraspt/mosquitosongp) | Laboratory wingbeats plus real recorded noise overlays; field transfer not thereby demonstrated |
| HumBug / MozzBNN | 2021-era | Bayesian CNN pipeline | Candidate event identification and species prediction | [Code](https://github.com/HumBug-Mosquito/MozzBNN) | Specify the checkpoint and dataset version |
| BioDCASE CD-MSC baseline | 2026 | Log-mel; MTRCNN | Nine-species cross-domain classification | [Code](https://github.com/Yuanbo2020/CD-MSC) · [Paper](https://arxiv.org/abs/2603.20118) | A specific benchmark protocol, not a universal accuracy claim |

## Model notes

### WbNet

- Published in *Scientific Reports* (2022).
- The paper reports model accuracy of approximately **89.9% on WINGBEATS** and **98.9% on ABUZZ** in its own experimental setups. **These values are not directly comparable** with other datasets or held-out-domain metrics.
- The study also explored transfer learning with ResNet architectures; WbNet itself is primarily a supervised classifier.

### MosquitoSong+

- The official repository provides a small reproduction dataset and instructions for obtaining trained classification models.
- The source recordings include four mosquito species and both sexes. Overlapping 300 ms training/evaluation excerpts are derived from wingbeat recordings; split independence must be checked when building new benchmarks.
- The repository states *academic and non-commercial use only* alongside an Apache-2.0 licence notice. **Check the licence applying to each separate data/code/model asset before redistribution.**

### Optical versus airborne audio

An optical sensor records wingbeat-induced changes in light; a microphone records acoustic pressure. Frequency information can be related, but input signals and deployment biases are not interchangeable.

## Evaluation checklist

1. Report species and sex coverage, label taxonomy and ambiguous labels.
2. Disclose recording modality, sampling rate and preprocessing.
3. Split by session/individual/device where possible; document any overlap.
4. Report macro-F1, per-species recall and balanced accuracy in addition to accuracy.
5. Report out-of-domain results separately from within-dataset testing.
6. Link code, weights, dataset and evaluation scripts separately.
