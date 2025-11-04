# Efficient TT-STGCN for Sign Language Recognition

This repository contains an efficient and lightweight **Temporal Transformer Spatio-Temporal Graph Convolutional Network (TT-STGCN)** for **Sign Language Recognition (SLR)** using skeletal landmarks.
It combines transformer-based temporal modeling with adaptive graph convolution for highly efficient recognition while maintaining strong accuracy.

---

## 🚀 Highlights

* **Dual-Stream Architecture:** Joint and Bone feature streams with late fusion.
* **Lightweight Design:** Only **~0.25M parameters**, ideal for real-time applications.
* **High Accuracy:** Achieves **69.8% Top-1 accuracy** on the **NSLT-300** benchmark.
* **Training Optimizations:**

  * Label Smoothing Cross-Entropy
  * Mixup Augmentation
  * Warmup + Cosine Learning Rate Scheduler
  * Early Stopping & Gradient Clipping
  * Test-Time Augmentation (TTA)
* **Dataset Agnostic:** Works with pose-based datasets like **WLASL**, **NSLT**, or custom Mediapipe landmark data.

---

## 🧠 Landmark Extraction

The **`extraction_pipeline.ipynb`** (and its underlying script) uses **MediaPipe Holistic** to extract **65 landmarks** per frame as proposed in the **MSE-GCN** methodology:

* **23 Pose landmarks** (face & body)
* **21 Left-hand landmarks**
* **21 Right-hand landmarks**

Each frame is processed to produce two complementary data streams:

* **Joint Stream:**
  Captures 2D coordinates and relative positions of each joint to a central node (mid-shoulder reference).
* **Bone Stream:**
  Encodes geometric relations as **bone length** and **bone angle**, providing richer motion dynamics.

> These features are stored as NumPy arrays (`.npz` files) and directly used by the TT-STGCN model for training and evaluation.

---

## 📁 Project Structure

```
Efficient-TT-STGCN-for-Sign-Language-Recognition/
│
├── src/
│   ├── lightweight-ttstgcn-300.ipynb     # Full training pipeline for NSLT-300
│   ├── landmarks-extraction.ipynb        # Landmark extraction pipeline using MediaPipe
│
├── .gitignore
├── requirements.txt
└── README.md
```

---

## ⚙️ Installation

```bash
git clone https://github.com/Muhammad-Huzifa/Efficient-TT-STGCN-for-Sign-Language-Recognition.git
cd Efficient-TT-STGCN-for-Sign-Language-Recognition
pip install -r requirements.txt
```

---

## 🧩 Applications

* Continuous Sign Language Recognition (CSLR)
* Gesture / Action Recognition
* Pose-based Human Motion Understanding
* Low-latency sign interpretation systems

---

## 📊 Performance Summary

| Dataset  | # Classes | Parameters | Top-1 Accuracy |
| -------- | --------- | ---------- | -------------- |
| NSLT-300 | 300       | ~0.25M     | **69.8%**      |

---

## 👨‍🔬 Author

**Muhammad Huzaifa**
Sign Language Recognition Researcher | Deep Learning Engineer
📬 **[mhuzaifa3202@gmail.com](mailto:mhuzaifa3202@gmail.com)**

---

## 🧾 Citation (if used in research)

If this work helps your research or project, please consider citing:

```
@misc{huzaifa2025ttstgcn,
  author = {Muhammad Huzaifa},
  title = {Efficient TT-STGCN for Sign Language Recognition},
  year = {2025},
  url = {https://github.com/Muhammad-Huzifa/Efficient-TT-STGCN-for-Sign-Language-Recognition}
}
```

---

✨ *Designed for efficiency, optimized for Sign Language Recognition.*
