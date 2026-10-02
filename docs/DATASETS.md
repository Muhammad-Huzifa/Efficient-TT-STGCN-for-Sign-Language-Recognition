# Dataset and feature guide

The notebooks use WLASL videos and `nslt_100.json` / `nslt_300.json` split annotations. Resources: [official WLASL project](https://dxli94.github.io/WLASL/) and [the resized dataset used by the original experiments](https://www.kaggle.com/datasets/sttaseen/wlasl2000-resized).

Start with the extraction notebook and inspect its video, annotation, and output paths. Then attach the generated features and split JSON to the training environment. Existing `/kaggle/input/...` and `/kaggle/working/...` paths are preserved as experiment settings; replace them with the actual attached dataset names or local paths before training.

The training notebook reads an individual-file `MSE_GCN_features_individual` directory. The shared extractor represents 65 pose/hand joints with position and relative-position channels, plus bone length/angle features. Keep this format aligned with the dataset class. A differently encoded landmark dataset needs an explicit conversion.

Videos, landmark archives, and trained checkpoints are not bundled. Existing inference sections may require a separately supplied checkpoint. This restructuring did not run extraction or GPU training.
