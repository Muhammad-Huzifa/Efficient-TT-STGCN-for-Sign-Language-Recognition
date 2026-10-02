# MSE-GCN Learning Implementation

Study stage 2 in the public sign-language recognition collection. Original source repository: `MSE-GCN-Paper-Methodology`; snapshot commit: `a0a433898ab126d70ebaf6d76e7f1040d7e8204f`.

| Order | Notebook |
| --- | --- |
| 1 | [01_extract_landmarks.ipynb](notebooks/01_extract_landmarks.ipynb) |
| 2 | [02_train_mse_gcn.ipynb](notebooks/02_train_mse_gcn.ipynb) |

## Environment

From the repository root, use Python 3.11 in this experiment's own virtual environment:

```bash
python -m venv .venv
```

| Terminal | Activate the environment |
| --- | --- |
| Windows Command Prompt | `.venv\Scripts\activate.bat` |
| Windows PowerShell | `.\.venv\Scripts\Activate.ps1` |
| Windows Git Bash | `source .venv/Scripts/activate` |
| Linux/macOS | `source .venv/bin/activate` |

```bash
python -m pip install -r experiments/02_mse_gcn/requirements.txt
jupyter lab
```

## Inputs and execution

Combined MSE_GCN_combined_features.npz and the configured NSLT split.

Run extraction first after setting its video, annotation, and output paths. Then configure training input paths, choose the class subset, and use a fresh kernel for the intended experiment. Read the [feature-format guide](../../docs/DATASETS.md). Several original training notebooks contain multiple configurations; select the intended blocks before running them.

Model and training source cells are unchanged. Only headings, paths in documentation, cleared outputs, and file organization were added. Dataset extraction, full dependency installation, GPU training, and checkpoint inference were not performed during consolidation.
