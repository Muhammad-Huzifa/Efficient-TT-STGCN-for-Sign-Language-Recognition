# Dataset and feature formats

The public experiments use WLASL videos and NSLT class-subset annotations. Resources: [official WLASL project](https://dxli94.github.io/WLASL/) and [the resized dataset referenced by the source notebooks](https://www.kaggle.com/datasets/sttaseen/wlasl2000-resized).

| Experiment | Training input | Configuration notes |
| --- | --- | --- |
| BiLSTM | Combined landmark NPZ | Extraction names `Full_Landmarks_300_553_3D.npz`; training refers to `Landmarks_300_553_3D.npz`. Point both to your actual output. The name alone does not establish the tensor shape. |
| MSE-GCN | `MSE_GCN_combined_features.npz` | Use the extractor's combining step and verify the loader's schema. |
| TT-STGCN | Individual feature NPZ directory | Keep joint/bone ordering aligned with its dataset class; choose the intended 100/300-class blocks. |
| Efficient TT-STGCN | Individual joint/bone feature archives | Use the exact configured split and feature representation. |

The graph extractors represent 65 pose/hand joints and position/relative-position plus bone features. A BiLSTM landmark archive needs the preprocessing expected by its own loader. Do not substitute a differently encoded NPZ without checking shapes, channels, joint order, class labels, and split membership.

Original Windows and Kaggle paths remain in source configuration cells. Set extraction video/JSON/output paths first, then the training feature/split/checkpoint paths. The models, hyperparameters, and source code were preserved during consolidation; no universal data loader is claimed.

Dataset videos, trained checkpoints, and complete feature archives are not bundled. Install one experiment's environment at a time. MediaPipe uses the legacy Holistic-compatible release; the requirements files are proposed environments, not installation-tested GPU locks.
