# BirdCLEF 2026 Starter

This repository now uses a notebook-first workflow, following the style of `/home/rafael/Documentos/Faculdade/Sistemas Apoio a Decisão/audio/main.ipynb`.

## Files

- `main.ipynb`: download, inspect, and train a first BirdCLEF 2026 baseline in notebook form.
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
- It summarizes `train.csv`, `taxonomy.csv`, and `train_soundscapes_labels.csv` when available.
- It trains a lightweight baseline on `train_audio` using 5-second windows and handcrafted audio features.
- This is an initiation scaffold, not a competition-ready soundscape submission pipeline.
