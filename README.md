<h1 align="center">🌾 Rice-Vision 🌾</h1>
<p align="center">A Deep Learning Playground for Fine-Grained Rice Variety Classification</p>

<p align="center">
  <img src="https://img.shields.io/badge/Deep%20Learning-PyTorch-blue?style=flat-square"/>
  <img src="https://img.shields.io/badge/Models-6%20CNN%20Architectures-purple?style=flat-square"/>
  <img src="https://img.shields.io/badge/GradCAM-Enabled-orange?style=flat-square"/>
</p>

<p align="center">
  <img src="https://i.pinimg.com/736x/f3/64/7a/f3647ab910a201ec5a429481b1ac825a.jpg" alt="Web Development Showcase Banner" width="1200">
</p>

RiceVision Lab is a curated workspace exploring automated rice variety classification using modern computer-vision techniques. This project analyzes two well-known rice datasets and compares six powerful CNN architectures to understand how models behave on both **single-grain** and **multi-grain** images.

The repo includes structured training notebooks, performance graphs, Grad-CAM heatmaps, and a clean template for anyone who wants to explore fine-grained classification research.

---

## 🎯 Project Goals
- Explore how different CNN architectures perform on single-grain vs multi-grain images  
- Understand the impact of augmentation on model generalization  
- Visualize attention patterns using **Grad-CAM**  
- Provide a clean and reusable workflow for other ML learners

---

## 📁 Datasets Used

### **1. Aruzz Dataset (20 varieties — single grain images)**  
A large-scale rice dataset featuring high-quality single-grain images.  
👉 [Mendeley - Aruzz](https://data.mendeley.com/datasets/3mn9843tz2/1)

### **2. BD Rice Dataset (8 categories — multiple grains per image)**  
Images captured from mixed environments with visible clusters of rice grains.  
👉 [Mendeley - BD Rice](https://data.mendeley.com/datasets/y4gywztksm/1)
  

Both datasets were used in **original** and **augmented** forms for performance comparison.


## 🧠 Models Used (6 CNN Architectures)

This project evaluates six modern and diverse architectures:

- **ResNeXt50**
- **DenseNet201**
- **GhostNet**
- **EfficientNetV2-S**
- **NASNet-A-Large**
- **Xception**

Each model was trained using a unified PyTorch pipeline with identical hyperparameters for a fair comparison.

## 📓 Repository Contents

This repository is intentionally kept clean and lightweight. To help learners focus on the **core training workflow**, only **one notebook** is included:

### ✔ **Aruzz (Augmented) Notebook – Template Version**  
A polished, easy-to-follow training template covering the full pipeline — preprocessing, augmentation, model training, evaluation, and Grad-CAM visualization. Learners can easily adapt this notebook for both the Aruzz and BDRice datasets, or extend it with new models.

### ✔ **Visualizations Included**
The repository includes all essential visual outputs generated during the experiments, providing a clear understanding of model behavior:

- **Training & Validation Accuracy/Loss Curves**  
- **Confusion Matrices**  
- **ROC-AUC & Precision–Recall Curves**  
- **Grad-CAM Heatmaps** (Aruzz & BDRice)

These visuals highlight learning patterns, model stability, and the specific grain features each model focuses on — making the entire workflow transparent and easy to interpret.

---
> 📌 *The original Aruzz notebook and all BDRice notebooks (original & augmented) are not included.* Their workflows are identical to the template provided. This encourages hands-on experimentation rather than uploading repetitive files.
---


## 🏆 Highlight Findings (From the Experiments)

- **EfficientNetV2-S** achieved the highest performance across both datasets  
- Reached **99.95% accuracy** after augmentation  
- DenseNet201 and NASNet-A-Large also performed extremely well  
- Grad-CAM confirmed meaningful feature focus (grain edges, texture patterns)  
- Augmentation significantly improved generalization, especially for BD Rice

---

## 📦 Trained Models & Full Research Report  
To keep the repository light and accessible, trained model files (`.pth`) and the complete PDF report are not included here.

📬 You can request them at: [contact me](mailto:heyneeddev@gmail.com)

## 🚀 Getting Started

Clone the repo:
```bash
git clone https://github.com/Shourav-Deb/Rice-Vision
cd Rice-Vision
```
---
