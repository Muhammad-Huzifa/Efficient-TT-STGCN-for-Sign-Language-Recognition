# Efficient TT-STGCN

Study stage 4 in the public sign-language recognition collection. Original source repository: `Efficient-TT-STGCN-for-Sign-Language-Recognition`; snapshot commit: `ced7644f57a7e334dbb730f0e84b10c647fed2ff`.

| Order | Notebook |
| --- | --- |
| 1 | [01_extract_landmarks.ipynb](notebooks/01_extract_landmarks.ipynb) |
| 2 | [02_train_efficient_tt_stgcn.ipynb](notebooks/02_train_efficient_tt_stgcn.ipynb) |

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
python -m pip install -r experiments/04_efficient_tt_stgcn/requirements.txt
jupyter lab
```

## Inputs and execution

Individual joint/bone feature archives with the configured 300-class split.

Run extraction first after setting its video, annotation, and output paths. Then configure training input paths, choose the class subset, and use a fresh kernel for the intended experiment. Read the [feature-format guide](../../docs/DATASETS.md). Several original training notebooks contain multiple configurations; select the intended blocks before running them.

Model and training source cells are unchanged. Only headings, paths in documentation, cleared outputs, and file organization were added. Dataset extraction, full dependency installation, GPU training, and checkpoint inference were not performed during consolidation.
