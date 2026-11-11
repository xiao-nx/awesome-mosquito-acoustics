# Representation Learning and Transfer Learning

[← Model Catalog](README.md)

**Scope.** Learned embeddings, pretrained audio encoders, self-supervised approaches, few-shot adaptation, and representation robustness. **Separate mosquito-validated methods from prospective transfers from other taxa.**

## Mosquito-specific evidence

| Study | Approach | Evidence status | Resources |
|---|---|---|---|
| Wei et al. (2022), WbNet study | Transfer learning explored for ResNet-based wingbeat classification | Evaluated on mosquito wingbeat datasets; predominantly supervised species-recognition study | [Paper](https://doi.org/10.1038/s41598-022-14372-x) · [Code](https://github.com/xutong30/WbNet-ResNet-Attention) |
| Hou et al. (2026), DR-BioL | Contrastive learning and species-conditional distribution alignment | Mosquito-specific domain-robust representation learning; assess exact reported protocol | [Preprint](https://arxiv.org/abs/2510.00346) · [Data record](https://zenodo.org/records/17287037) |

## Candidate general bioacoustic/audio encoders (not mosquito-validated by inclusion here)

These are **research directions**, not catalogued mosquito-specific benchmark winners:

- Self-supervised acoustic pretraining on unlabeled mosquito audio.
- Frozen pretrained embeddings compared with fine-tuning on mosquito labels.
- Contrastive objectives that avoid learning device/site shortcuts.
- Few-shot evaluation on previously unseen mosquito species or recording domains.

If adding AVES, BirdNET, general-purpose audio foundation models, or models pretrained on other taxa, state the **actual mosquito evaluation paper and dataset**, or label them *candidate transfer only*.

## Standard representation-learning evaluation

- Linear probe versus fine-tuned classifier versus supervised scratch baseline.
- Label-efficiency curves (number of independently annotated recordings/individuals).
- Held-out session, device, site and species–domain combinations.
- Ablations for augmentation, domain-balanced sampling and metadata leakage.
- Embedding sensitivity to species, sex, temperature, device and background noise.

## Avoiding misleading claims

A cluster of acoustic embeddings does not automatically correspond to a biological behaviour. Verify biological states using independent video or experimental labels. Contrastive learning alone does not guarantee invariance to acquisition domains.
