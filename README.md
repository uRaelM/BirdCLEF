# BirdCLEF 2026 Starter

This repository now uses a notebook-first workflow, following the style of `/home/rafael/Documentos/Faculdade/Sistemas Apoio a Decisão/audio/main.ipynb`.

## Files

- `main.ipynb`: download, inspect, train, and run a BirdCLEF 2026 multilabel SED baseline in notebook form.
- `requirements.txt`: Python dependencies for the notebook workflow.

## Quick Start

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
```

Then open `main.ipynb` and run the cells in order.

## Notes

- The notebook downloads the competition data with `kagglehub`.
- It summarizes `train.csv`, `taxonomy.csv`, `train_soundscapes_labels.csv`, and `sample_submission.csv` when available.
- It trains a local multilabel baseline on `train_soundscapes` using 5-second windows, `mel spectrogram`, and a PyTorch model inspired by the Kaggle EfficientNet-B0 SED logic.
- It also includes a submission-generation step for `test_soundscapes`.
- This is still a compact baseline, but it is now aligned with the competition task instead of a simple `train_audio` clip classifier.
