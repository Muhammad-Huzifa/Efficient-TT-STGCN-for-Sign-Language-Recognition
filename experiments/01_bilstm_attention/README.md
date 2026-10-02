# BiLSTM with Attention

Study stage 1 in the public sign-language recognition collection. Original source repository: `ISLR-Landmarks-using-BiLSTM-with-Attention-Mechanism`; snapshot commit: `0adb04466a0969fd3bec32f23fc28427ecfd96bc`.

| Order | Notebook |
| --- | --- |
| 1 | [01_extract_landmarks.ipynb](notebooks/01_extract_landmarks.ipynb) |
| 2 | [02_train_100_classes.ipynb](notebooks/02_train_100_classes.ipynb) |
| 3 | [03_train_300_classes.ipynb](notebooks/03_train_300_classes.ipynb) |

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
python -m pip install -r experiments/01_bilstm_attention/requirements.txt
jupyter lab
```

## Inputs and execution

Combined landmark NPZ; configure its exact schema and class split in the notebook.

Run extraction first after setting its video, annotation, and output paths. Then configure training input paths, choose the class subset, and use a fresh kernel for the intended experiment. Read the [feature-format guide](../../docs/DATASETS.md). Several original training notebooks contain multiple configurations; select the intended blocks before running them.

Model and training source cells are unchanged. Only headings, paths in documentation, cleared outputs, and file organization were added. Dataset extraction, full dependency installation, GPU training, and checkpoint inference were not performed during consolidation.
