# Prediction Uncertainty, Calibration and Reliability

[← Model Catalog](README.md)

**Scope.** Mosquito acoustic models that expose useful measures of predictive reliability, plus recommended evaluation for calibrated probabilities and uncertain deployments.

## Mosquito-specific implementation

### MozzBNN / HumBug

- **Architecture family:** Bayesian convolutional neural network.
- **Task:** Mosquito candidate detection; related pipeline for species classification.
- **Code:** [HumBug-Mosquito/MozzBNN](https://github.com/HumBug-Mosquito/MozzBNN).
- **Output:** Candidate `start_time`, `stop_time`, `probability`, `predictive_entropy`, `mutual_information` (and species labels for the relevant prediction pathway).
- **Reproducibility:** Pin the checkpoint and code version; the official repository identifies the 2021 publication checkpoint separately from later model versions.

## What uncertainty outputs can and cannot show

- **Probability:** Model score; not automatically a calibrated probability of true species presence.
- **Predictive entropy:** Uncertainty in the predictive distribution.
- **Mutual information:** A possible indicator of model-parameter uncertainty in Bayesian predictive settings, dependent on estimation method.
- **Calibration:** Whether predicted probabilities agree with observed frequencies under a specified evaluation distribution.
- **OOD detection:** Whether the model can flag unfamiliar inputs; requires its own independently labelled evaluation.

**Caution:** Predictive uncertainty does not replace measurement of acoustic detectability or independent ecological calibration.

## Recommended assessment

| Evaluation target | Suggested metrics / plots |
|---|---|
| Detection error | Event-level precision and recall; false positives per audio hour |
| Species-class probabilities | Brier score; NLL; reliability diagrams; classwise calibration |
| Domain shift | Domain-stratified calibration and error rates |
| Selective prediction | Risk–coverage curves; accuracy at retained fraction |
| Unknown species / sounds | OOD AUROC/AUPRC under a documented unknown set |
| Statistical reliability | Confidence intervals across independent recording groups and seeds |

## Reporting requirements

Specify calibration-set source, probability aggregation (window/event/recording), choice of threshold and whether test data influenced selection. A lower predictive entropy is not evidence of correct identification without an empirical comparison.

## Further reading

For ecological inference from AI-generated detections and its different uncertainty sources, refer to the separate `acoustic-ecological-inference` project when its public URL is available.
