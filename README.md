# Sign Language Recognition

A public research and learning collection for landmark-based isolated sign classification. Four existing experiments are organized from a BiLSTM baseline through graph models and temporal attention to a lightweight TT-STGCN variant.

## Study sequence

| Order | Experiment | Notebooks |
| --- | --- | --- |
| 1 | [BiLSTM with Attention](experiments/01_bilstm_attention/README.md) | 3 |
| 2 | [MSE-GCN Learning Implementation](experiments/02_mse_gcn/README.md) | 2 |
| 3 | [TT-STGCN](experiments/03_tt_stgcn/README.md) | 2 |
| 4 | [Efficient TT-STGCN](experiments/04_efficient_tt_stgcn/README.md) | 2 |

Each experiment includes its own extraction/training notebooks, dependencies, source snapshot, and dataset notes. The complete collection contains nine notebooks. This is a study order, not a claim that the experiments share one training pipeline or were published in this chronology.

## Get started

```bash
git clone https://github.com/Muhammad-Huzifa/Efficient-TT-STGCN-for-Sign-Language-Recognition.git
cd Efficient-TT-STGCN-for-Sign-Language-Recognition
```

Start with [BiLSTM](experiments/01_bilstm_attention/README.md), or select the experiment you want to reproduce. Use Python 3.11 and its environment commands. Read [the dataset guide](docs/DATASETS.md) before installing or running extraction.

## Structure

| Path | Purpose |
| --- | --- |
| `experiments/01_bilstm_attention/` | Landmark extraction and 100/300-class BiLSTM notebooks |
| `experiments/02_mse_gcn/` | Combined-feature graph-model experiment |
| `experiments/03_tt_stgcn/` | Joint/bone graph and temporal attention experiments |
| `experiments/04_efficient_tt_stgcn/` | Lightweight TT-STGCN experiment |
| `data/`, `outputs/` | Local input/output instructions |
| `scripts/` | Offline notebook checks |
| `docs/` | Feature formats, provenance, and results status |

## Verification

```bash
python scripts/check_notebooks.py --root experiments
```

All source model/training cells are preserved and their hashes recorded in [the source map](docs/SOURCE_MAP.md). JSON and Python syntax were checked. Full dependency installation, video extraction, GPU training, and real checkpoint inference were not run. Historical accuracy values are labeled explicitly in [results notes](docs/RESULTS.md).

General neural-network and detection lessons belong in the [Deep Learning collection](https://github.com/Muhammad-Huzifa/Neural-Networks-and-Deep-Learning-Using-Pytorch-and-Tensor-Flow); classical ML belongs in [Machine Learning](https://github.com/Muhammad-Huzifa/Machine_Learning).

Muhammad Huzifa — [GitHub](https://github.com/Muhammad-Huzifa)
