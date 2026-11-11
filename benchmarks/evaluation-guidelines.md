# Evaluation Guidelines for Mosquito Acoustic AI

Recommended practices for reproducible **detection, species/sex classification and cross-domain evaluation**. These are **community-facing recommendations**, not the official rules of every benchmark. When reproducing a challenge, follow its published protocol first.

## 1. Define the task and unit of prediction

| Task | Unit | Typical targets | Preferred reporting |
|---|---|---|---|
| Clip classification | Clip | Species, sex, presence/absence | Classwise metrics and confusion matrix |
| Event detection | Timestamped acoustic event | Mosquito flight sound | Event precision/recall/F1, temporal matching tolerance |
| Continuous monitoring | Recording hour / monitored interval | Detected acoustic activity | False positives/hour, recording effort, event definitions |
| Cross-domain classification | Clip grouped by acquisition context | Species under domain shift | Seen/unseen metrics and breakdown by species and domain |

**Do not equate clips, acoustic events and individual mosquitoes.** Overlapping windows can correspond to a single flight; event counts are not individual abundance estimates.

## 2. Splitting without leakage

| Split | Intended claim | What to check |
|---|---|---|
| Random clip | Familiar-data interpolation | No overlapping or duplicated source audio across sets |
| Recording/session held out | Transfer to new recordings/sessions | All windows from a parent recording stay together |
| Individual held out | Transfer to new mosquitoes | Individual identities are reliable and disjoint |
| Device held out | Cross-device generalization | Device and species labels are not perfectly confounded |
| Site/location held out | Geographic transfer | New site and acquisition conditions are described |
| Entire domain held out | New acquisition-domain transfer | No training samples from that domain |
| Species–domain combination held out | Unseen combinations | Domain may still occur for other species |

**Checklist:** Publish stable split manifests (where permitted), grouping identifiers, class counts and a species × domain contingency table. Prevent duplicates and overlapping clips from leaking across partitions. Fit normalization, learned features, calibrators and thresholds only on appropriate training/validation data. Keep the final test set untouched for model selection.

The **BioDCASE 2026 CD-MSC** official unseen-domain definition is based on an unseen **species–domain combination**, not necessarily a domain absent for every training species. See the [official task](https://biodcase.github.io/challenge2026/task5).

## 3. Report appropriate metrics

### Classification

- **Balanced accuracy** and **macro-F1** for imbalanced species groups.
- Per-class precision/recall and a confusion matrix (including support per class).
- Per-domain metrics and a seen–unseen gap for domain-shift studies.
- Multiple seeds or independent splits with variability estimates; make clear whether uncertainty is across seeds, clips or independent groups.

For CD-MSC, use the challenge's official `BA_unseen` and `DSG = |BA_unseen − BA_seen|` for comparisons with its ranking. Do not mix custom and official scores in one leaderboard.

### Detection

- Precision, recall, F1 and preferably precision–recall curves.
- For event detection: declare onset/offset tolerance, event merging rules and annotation conventions.
- For continuous recordings: **false-positive events per recording hour**, detection sensitivity at stated operating thresholds and effective recording effort.
- Report performance across noise levels, environments and sensor setups when available.

### Prediction reliability

- When probabilities are used downstream, report Brier score, negative log-likelihood and/or reliability diagrams.
- Evaluate calibration on held-out recording conditions; within-domain calibration does not establish out-of-domain reliability.
- For unknown species or environments, specify whether the task allows abstention/rejection; a closed-set benchmark does not automatically test open-set detection.

## 4. Evaluate domain confounding and shortcuts

Mosquito labels may correlate with **device, country, background sound, laboratory, collection protocol or time**. A classifier might exploit those shortcuts rather than transferable mosquito acoustics.

Recommended checks:

1. Show a **species × domain table**, including missing combinations and sample counts.
2. Compare a **biological-signal baseline** (e.g., interpretable wingbeat features) with stronger audio models when appropriate.
3. Where suitable metadata are available, train a **metadata-only diagnostic baseline** to assess predictive confounding; do not interpret its performance as evidence of causal shortcuts by itself.
4. Report performance separately across devices/sites and compare with within-domain testing.
5. Inspect possible preprocessing artifacts, correlated segments, duplicate clips and source provenance.
6. Do not claim generalization to species or domain types missing entirely from evaluation data.

Where individual, session or site IDs are unavailable, explicitly state that independence cannot be verified.

## 5. Minimum reporting checklist

- [ ] Dataset name, release/version, citation, license and retrieval URL.
- [ ] Modality, sampling rate, recording duration, species and sample distribution.
- [ ] Exact task, prediction unit and label definitions.
- [ ] Train/validation/test partition and grouping variables.
- [ ] Device/site/session/individual information, if available.
- [ ] Species × domain coverage and known confounding.
- [ ] Architecture, pretrained weights, input processing and training settings.
- [ ] Model selection method, thresholds and random seeds.
- [ ] Primary metric, metric code, classwise results and variability.
- [ ] Official vs modified benchmark protocol clearly distinguished.
- [ ] Code/configuration, split manifest and reproducible instructions, as licensing allows.
- [ ] Limitations of field transfer and biological/ecological interpretation.

## 6. How to submit benchmark resources

To propose a new entry in [benchmark-registry.csv](benchmark-registry.csv), provide an **official published task description**, dataset/version and access conditions, intended task, official split, primary/secondary metrics and a baseline or results source when available. For a useful dataset **without** a formal benchmark, suggest an entry in the [Dataset Catalog](../datasets/README.md) instead.

## Sources and scope

- [BioDCASE 2026 CD-MSC official task](https://biodcase.github.io/challenge2026/task5)
- [CD-MSC baseline repository](https://github.com/Yuanbo2020/CD-MSC)
- [CD-MSC baseline paper](https://arxiv.org/abs/2603.20118)

The guidelines above synthesize general evaluation principles; they are not presented as rules issued by the BioDCASE organizers.
