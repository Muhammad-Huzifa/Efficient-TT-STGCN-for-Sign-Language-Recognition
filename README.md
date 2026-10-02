# Efficient TT-STGCN

A notebook-based isolated sign-language recognition experiment using joint and bone features, adaptive graph layers, and lightweight temporal modeling.

## Notebook order

| Order | Notebook |
| --- | --- |
| 1 | [01_extract_landmarks.ipynb](notebooks/01_extract_landmarks.ipynb) |
| 2 | [02_train_lightweight_ttstgcn.ipynb](notebooks/02_train_lightweight_ttstgcn.ipynb) |

## Setup

Use Python 3.11 in a separate environment. Clone and open the project root:

```bash
git clone https://github.com/Muhammad-Huzifa/Efficient-TT-STGCN-for-Sign-Language-Recognition.git
cd Efficient-TT-STGCN-for-Sign-Language-Recognition
python -m venv .venv
```

| Terminal | Activation |
| --- | --- |
| Windows Command Prompt | `.venv\Scripts\activate.bat` |
| Windows PowerShell | `.\.venv\Scripts\Activate.ps1` |
| Windows Git Bash | `source .venv/Scripts/activate` |
| Linux/macOS | `source .venv/bin/activate` |

```bash
python -m pip install -r requirements.txt
jupyter lab
```

## Data and execution

Read [the dataset guide](docs/DATASETS.md) before running extraction or training. Dataset archives and model checkpoints are external resources. Kaggle experiment paths are retained and must match the resources attached to your runtime.

The notebooks target isolated sign classification. Continuous sign-language recognition, production deployment, and measured real-time performance are not established by these files.

## Structure

| Path | Purpose |
| --- | --- |
| `notebooks/` | Extraction and training notebooks |
| `requirements.txt` | Python dependencies |
| `docs/DATASETS.md` | Data, feature format, and runtime paths |
| `docs/RESULTS.md` | Reported results and reproduction status |
| `docs/STRUCTURE.md` | Original-to-current filename mapping |

MediaPipe is kept on its legacy Holistic-compatible 0.10.14 release. NumPy and its OpenCV distribution are aligned with that environment; full dependency installation has not been verified here. The original source does not constitute a locked GPU environment.

This pass checks notebook JSON, links, and source organization. Full extraction, model training, checkpoint inference, and reported benchmark figures have not been reproduced. See [results notes](docs/RESULTS.md).

Muhammad Huzifa — [GitHub](https://github.com/Muhammad-Huzifa)
