# Contributing to Awesome Mosquito Acoustics

Thank you for helping improve this research catalog. We welcome **new resources, corrections, source links, and metadata improvements**.

## What can I contribute?

- A peer-reviewed paper or clearly labeled preprint about mosquito acoustic biology, sensing, recognition, or monitoring.
- A publicly documented mosquito acoustic or optical wingbeat dataset.
- A published AI model, official implementation, or pretrained weights with an accessible source.
- A published benchmark or a correction to evaluation descriptions.
- A publicly available recording, annotation, or signal-processing tool relevant to mosquito acoustics.

## Before submitting

1. Search for an existing entry to avoid duplicates.
2. Find the **primary source** (DOI, official dataset URL, or author-maintained repository).
3. Verify the dataset version, exact modality, study task, license, and availability. Use `unknown` rather than guessing.
4. Distinguish **published**, **preprint**, and **proposal**; distinguish **direct mosquito evidence** from broader bioacoustic evidence.
5. Do not upload copyrighted PDFs, restricted audio, or model weights unless you are authorized to redistribute them.

## How to contribute

**Easiest:** open a New Paper, New Dataset, or New Model issue using a template. Provide source URLs and a short explanation of relevance.

**Pull request:** update the appropriate CSV registry or Markdown catalog; link the new entry to a primary source, and ensure no duplicate IDs. If adding a detailed dataset card, create `datasets/cards/<dataset-id>.md` and link it from the catalog. Run `python scripts/validate_resources.py` before submitting.

## Registry conventions

- Use unique, lowercase, hyphenated IDs (for example, `example-dataset-2026`).
- Use a consistent year and make the release version explicit in notes when important.
- Prefer DOI URLs (`https://doi.org/...`) when available.
- Place multiple tags in a single CSV field using semicolons (`;`), properly quoted if needed.
- Leave unknown values blank or use `unknown`, never fabricate specifics.
- Report numeric performance only with a source, metric, evaluation split, and dataset.
- Do not claim that a model is reproducible solely because its paper is available.

## Review criteria

Contributors and maintainers may request more detail before merging if provenance, permissions, relevance, or evaluation conditions are unclear. Corrections to existing resources are especially valuable.

## Community standards

Please follow the [Code of Conduct](CODE_OF_CONDUCT.md).
