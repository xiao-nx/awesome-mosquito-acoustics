# Cross-Domain Generalization and Robustness

[← Model Catalog](README.md)

**Scope.** Mosquito acoustic recognition under changes in device, recording environment, location, recording session and species–domain pairing.

## Published resources

| Resource | Year | Approach | Domain protocol | Links |
|---|---|---|---|---|
| DR-BioL — Hou et al. | 2026 (preprint posted 2025) | Contrastive learning + species-conditional distribution alignment | Multiple mosquito acquisition domains; evaluate against the paper's actual splits | [Paper](https://arxiv.org/abs/2510.00346) · [Data](https://zenodo.org/records/17287037) |
| BioDCASE CD-MSC baseline | 2026 | Multi-temporal Resolution CNN (MTRCNN) | Seen vs unseen **species–domain combinations** | [Challenge code](https://github.com/Yuanbo2020/CD-MSC) · [Paper](https://arxiv.org/abs/2603.20118) |
| MosquitoSong+ | 2024 | Environmental-noise augmentation / amplitude variation | Robustness to constructed noise mixtures, **not automatically held-out devices/sites** | [Paper](https://doi.org/10.1371/journal.pone.0310121) · [Code](https://github.com/akaraspt/mosquitosongp) |

## BioDCASE CD-MSC (2026)

The [official code repository](https://github.com/Yuanbo2020/CD-MSC) documents **9 species, 5 domains, 271,380 clips**, and a released MTRCNN pipeline using 8 kHz audio and 64-bin log-mel features. It provides configs, split IDs, evaluation scripts and checkpoints.

For the repository's **10-seed best-checkpoint development-test summary**:

| Metric | Mean ± SD |
|---|---:|
| Seen-domain balanced accuracy | 0.8793 ± 0.0101 |
| Unseen-domain balanced accuracy | 0.1854 ± 0.0140 |
| Domain shift gap (absolute difference) | 0.6939 ± 0.0186 |

Source: the official README's `outputs/multi_seed_summary/best_model_eval/summary_stats.json` description. **Do not confuse this with final challenge evaluation results or with a particular individual seed.**

The official task defines unseen cases in relation to species–domain combinations, not necessarily wholly new physical domains. Read the protocol before interpreting the metric.

## Standard evaluation protocol

1. Define domain identifiers and their relationship to species labels.
2. Avoid clips from the same parent recording appearing across splits.
3. Report label and domain distribution for each split.
4. Report within-domain and cross-domain performance separately.
5. Include simple audio-only, metadata-only and audio-plus-metadata baselines where metadata are relevant and available.
6. Test counterfactual or shuffled metadata when shortcut learning is suspected.
7. Report per-class recall and across-seed uncertainty, not just overall accuracy.

## Limitations to document

Confounding between species and device/site, unequal domain sizes, missing combinations, recording-session leakage, and label-taxonomy differences can all distort conclusions about generalization.
