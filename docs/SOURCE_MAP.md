# Consolidation provenance

All nine source notebooks are retained. Code-cell hashes are equal before and after migration; headings and generated notebook outputs are handled separately. Original commits and Git blob identifiers are recorded in [SOURCE_MAP.json](SOURCE_MAP.json).

| Original repository and path | Current notebook | Code-cell SHA-256 |
| --- | --- | --- |
| `ISLR-Landmarks-using-BiLSTM-with-Attention-Mechanism: src/landmarks_Extraction.ipynb` | [01_extract_landmarks.ipynb](../experiments/01_bilstm_attention/notebooks/01_extract_landmarks.ipynb) | `53ad62fc7819180725a2e422a0e483d2c80e7eff2f84ae3e24a192ea5d02f692` |
| `ISLR-Landmarks-using-BiLSTM-with-Attention-Mechanism: src/training_100 Classes.ipynb` | [02_train_100_classes.ipynb](../experiments/01_bilstm_attention/notebooks/02_train_100_classes.ipynb) | `4e6ed54b8cb0cbf4e334becac9c768eca70c0e9892cf08d9f9cb2d44a264f9a6` |
| `ISLR-Landmarks-using-BiLSTM-with-Attention-Mechanism: src/training_300 Classes.ipynb` | [03_train_300_classes.ipynb](../experiments/01_bilstm_attention/notebooks/03_train_300_classes.ipynb) | `f067a22acde7451e32bd21aa315d5a3cc2934c972d9bcdb2d149c700a8d7c4fc` |
| `MSE-GCN-Paper-Methodology: src/landmarks extraction.ipynb` | [01_extract_landmarks.ipynb](../experiments/02_mse_gcn/notebooks/01_extract_landmarks.ipynb) | `da08e737e6f94354a4b44d58ce6a4d5d164ab8fad5e3b8145f648635ae812bed` |
| `MSE-GCN-Paper-Methodology: src/mse-gcn-67-3500k.ipynb` | [02_train_mse_gcn.ipynb](../experiments/02_mse_gcn/notebooks/02_train_mse_gcn.ipynb) | `f8304067255284ee35a489017ff174440f8a0ccbdc2d519ef4cd9604c7da3cd0` |
| `TT-STGCN-for-Sign-Language-Recognition: src/landmarks extraction.ipynb` | [01_extract_landmarks.ipynb](../experiments/03_tt_stgcn/notebooks/01_extract_landmarks.ipynb) | `da08e737e6f94354a4b44d58ce6a4d5d164ab8fad5e3b8145f648635ae812bed` |
| `TT-STGCN-for-Sign-Language-Recognition: src/tt-stgcn-for-300 (1).ipynb` | [02_train_tt_stgcn.ipynb](../experiments/03_tt_stgcn/notebooks/02_train_tt_stgcn.ipynb) | `b658ef54c289feeb77fa8f6ecc920869af1355c37a7740ff7be53156516b4bf0` |
| `Efficient-TT-STGCN-for-Sign-Language-Recognition: notebooks/01_extract_landmarks.ipynb` | [01_extract_landmarks.ipynb](../experiments/04_efficient_tt_stgcn/notebooks/01_extract_landmarks.ipynb) | `da08e737e6f94354a4b44d58ce6a4d5d164ab8fad5e3b8145f648635ae812bed` |
| `Efficient-TT-STGCN-for-Sign-Language-Recognition: notebooks/02_train_lightweight_ttstgcn.ipynb` | [02_train_efficient_tt_stgcn.ipynb](../experiments/04_efficient_tt_stgcn/notebooks/02_train_efficient_tt_stgcn.ipynb) | `71700f84f451beec1d7ac1ac7440cd899792c67fd967fd1fe64c2d5265b3df52` |

Original source histories and GitHub metadata still require separate backups before deleting a source repository. This source map links to retained local notebooks, so navigation does not depend on the old repositories remaining online.
