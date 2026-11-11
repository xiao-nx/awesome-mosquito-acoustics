# Behavioural Acoustic Recognition

[← Model Catalog](README.md)

**Scope.** Algorithms that predict independently validated mosquito behavioural states from acoustic recordings, rather than inferring behaviour solely from species labels or wingbeat correlations.

## Current catalog status

**No general-purpose, independently validated mosquito behavioural classifier is designated in this initial release.** This is a conservative cataloguing decision, not a claim that no relevant research exists.

Well-studied mosquito acoustic phenomena such as flight tones, mating interactions and harmonic convergence supply candidate features and biological hypotheses; they are **not by themselves evidence of successful automated state recognition**.

## Candidate target labels

| Behaviour / measurement | Potential acoustic evidence | Validation needed |
|---|---|---|
| Flight activity / flight bouts | Flight-associated acoustic events and temporal structure | Synchronized video or independently verified flight behaviour |
| Courtship / mating interactions | Harmonic convergence and coupled frequency modulation | Recorded interactions with behavioural annotations |
| Host-seeking | Flight and stimulus-response dynamics | Controlled host-cue experiment with observed behaviour |
| Oviposition-search behaviour | Flight near oviposition sites | Independent experimental / video state labels |
| Resting | Often absence of flight tones | Direct observation; silence alone is **not** a resting label |

## Minimum evidence standard for adding a model

1. A precisely defined behavioural label and annotation protocol.
2. Independent video, tracking or experimental labels aligned with audio.
3. A transparent description of species, sex, temperature and acquisition conditions.
4. Test recordings and individuals independent from training, where possible.
5. Reported class counts, confusion matrix and uncertainty or confidence intervals.
6. Baselines that test whether context/device/temperature alone explains predictions.

## Proposed benchmark design (not an existing public benchmark)

A useful future dataset would pair continuous microphone audio with synchronized video, known mosquito identities or cohorts, environmental sensors, and behavioural annotations. Grouped splits should hold out individuals/sessions and, when possible, conditions or devices.

## How to contribute

Open an issue with a peer-reviewed paper or documented public model, its behaviour-label definitions, data and independent validation. Do not classify a species-recognition model as a behavioural classifier without behavioural evaluation.
