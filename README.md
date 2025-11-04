# Efficient TT-STGCN for Sign Language Recognition

This repository contains an efficient and lightweight **Temporal Transformer Spatio-Temporal Graph Convolutional Network (TT-STGCN)** for **Sign Language Recognition (SLR)** using skeletal landmarks. The model combines transformer-based temporal modeling with adaptive graph convolution, achieving high accuracy with minimal computational cost.

---

## 🧩 Key Features

* **Dual-Stream Fusion:** Joint and Bone features integrated.
* **Extremely Lightweight:** ~300K parameters only.
* **Modern Training Tricks:**

  * Label Smoothing Cross Entropy
  * Mixup Data Augmentation
  * Warmup + Cosine Learning Rate Scheduler
  * Early Stopping and Gradient Clipping
  * Test-Time Augmentation (TTA)
* **Dataset Agnostic:** Works with any pose-based dataset (e.g., WLASL, NSLT).

---

## 📁 Project Structure

```
Efficient-TT-STGCN-for-Sign-Language-Recognition/
│
├── src/
│   ├── train_pipeline.ipynb         # Full training pipeline
│   ├── extraction_pipeline.ipynb    # Landmark extraction notebook
│  
│   
│
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
* Gesture and Action Recognition
* Pose-based Human Motion Understanding

---



## 👨‍🔬 Author

**Muhammad Huzaifa**
Sign Language Recognition Researcher | Deep Learning Engineer
📬 Contact: mhuzaifa3202@gmail.com

---
