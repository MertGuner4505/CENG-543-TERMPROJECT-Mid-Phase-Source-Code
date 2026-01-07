
---

## Execution Environment

This project was developed and evaluated using **Google Colab**.

- **Training phase**: GPU (unconstrained, cloud-scale)
- **Evaluation phase**: CPU-only, single core, memory-limited (edge simulation)

All Colab-specific setup (e.g., Google Drive mounting) is handled **inside the
notebooks**, not in `project_core.py`.

---

## Running the Experiments (Colab)

1. Open either experiment notebook:
   - `MiniBERT_Experiment.ipynb`
   - `TinyBERT_Experiment.ipynb`

2. Run the first cell to mount Google Drive:
   ```python
   from google.colab import drive
   drive.mount('/content/drive')
