# Mosquito Acoustic Detection

[← Model Catalog](README.md)

**Scope.** Models that distinguish mosquito-generated sound from background audio, including event detection in continuous recordings. Detection is distinct from species classification: a model may detect a mosquito without identifying its species.

## Published studies and implementations

| Study / system | Method | Target | Data / evaluation notes | Resources |
|---|---|---|---|---|
| Kiskin et al. (2018 online; journal volume 2020) | Wavelet-conditioned CNN | Bioacoustic mosquito detection | Verify original dataset and train/test grouping before comparing scores | [Paper](https://doi.org/10.1007/s00521-018-3626-7) |
| Fernandes et al. (2021) | Spectrogram CNNs; binary, multiclass and ensemble approaches | *Aedes aegypti* sound identification | A target-species detection/classification task; not a general mosquito-vs-background benchmark | [Paper](https://doi.org/10.1016/j.compbiomed.2020.104152) |
| HumBug / MozzBNN (2021-era system) | Bayesian convolutional neural network | Locate mosquito-containing windows in audio | Includes uncertainty outputs and a species-prediction pathway; model versions differ | [Code](https://github.com/HumBug-Mosquito/MozzBNN) · [HumBugDB](https://github.com/HumBug-Mosquito/HumBugDB) |

## MozzBNN: implementation notes

The released `predict.py` pipeline outputs mosquito candidate intervals with start/stop times, probability, predictive entropy and mutual information. `predict_species.py` performs species prediction. The repository documents *different model checkpoints for different published/software versions*; cite and record the exact checkpoint when reproducing results.

- **Evidence status:** Public mosquito-specific implementation.
- **Code availability:** Public repository.
- **Weights:** Repository documents models under `Code/models/`; check the selected version before use.
- **Independent field evaluation:** Do not assume established solely from the existence of field audio.

## Recommended evaluation

- Event-level precision, recall and F1, with an explicit event-matching tolerance.
- False-positive events **per recording hour**, including mosquito-free soundscapes.
- Sensitivity stratified by device, distance, noise, species and recording site.
- Separation of recording sessions / individuals between training and test when IDs exist.
- Event merging rules and threshold selection fixed before test evaluation.
- Calibration and uncertainty assessment when probability outputs are used operationally.

## Caveats

Positive sliding windows are **not** independent mosquito encounters. A single flight can trigger multiple overlapping windows. Detection papers and classification papers should not be ranked together.

## Contribute a detection model

Supply the paper, dataset and modality, exact event definition, split protocol, evaluation unit, tested negative soundscapes, code and weights links (if available), and licence. See [Contributing](../CONTRIBUTING.md).
