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

RiceVision Lab is a curated workspace exploring automated rice variety classification using modern computer-vision techniques. This project was created by me and my team, which analyzes two well-known rice datasets and compares six powerful CNN architectures to understand how models behave on both **single-grain** and **multi-grain** images.

---

## 🎯 Project Goals
- Explore how different CNN architectures perform on single-grain vs multi-grain images  
- Understand the impact of augmentation on model generalization  
- Visualize attention patterns using **Grad-CAM**  
- Provide a clean and reusable workflow for other ML learners

---

## 📁 Datasets Used

### **1. Aruzz Dataset (20 varieties - single grain images)**  
A large-scale rice dataset featuring high-quality single-grain images.  
👉 [Mendeley - Aruzz](https://data.mendeley.com/datasets/3mn9843tz2/1)

### **2. BD Rice Dataset (8 categories - multiple grains per image)**  
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

This repository is intentionally kept clean and lightweight. To help learners focus on the **core workflow understanding**, only **demonstration** is included:

### ✔ ** Website Showcase**  

- Open the 🌾 [Rice Vision](https://rice-vision.streamlit.app/) web application in your browser.
  
- Select the Grain Type from the sidebar:
  - Single Grain (Aruzz) → for single rice grain images
  - Multi Grain (BDRice) → for multi-grain images
- Choose a model architecture:
  - EfficientNet-V2-S
  - DenseNet-201
  - ResNeXt50-32×4d
- Upload one or more rice images using the Upload image(s) option.
  - Supported formats: .jpg, .png, .jpeg
- For each uploaded image, the application shows:
  - Image name and preview
  - Predicted rice variety
  - Confidence score
  - Top 3 predictions displayed as confidence bars
- A low-confidence warning is displayed if the prediction confidence is below the threshold.
- Enable Grad-CAM (optional) to visualize image regions influencing the prediction.
- Multiple images are processed sequentially for batch evaluation.


### ✔ **Visualizations Included**
The repository includes all essential visual outputs generated during the experiments, providing a clear understanding of model behavior:

- **Training & Validation Accuracy/Loss Curves**  
- **Confusion Matrices**  
- **ROC-AUC & Precision–Recall Curves**  
- **Grad-CAM Heatmaps** (Aruzz & BDRice)
- **Both Dataset Sample Image's**

These visuals highlight learning patterns, model stability, and the specific grain features each model focuses on - making the entire workflow transparent and easy to interpret.

---


## 🏆 Highlight Findings (From the Experiments)

- **EfficientNetV2-S** achieved the highest performance across both datasets  
- Reached **99.95% accuracy** after augmentation  
- DenseNet201 and NASNet-A-Large also performed extremely well  
- Grad-CAM confirmed meaningful feature focus (grain edges, texture patterns)  
- Augmentation significantly improved generalization, especially for BD Rice

| Dataset ↓ / Model →  | ResNeXt50 | DenseNet201 | EfficientNet-V2-S | NASNet-Large | GhostNet   | Xception |
| -------------------- | --------- | ----------- | ----------------- | ------------ | ---------- | -------- |
| **Aruzz Original**   | 🟡 Good   | 🟡 Good     | 🟢 Best           | 🟠 Average   | 🔴 Weak    | 🟡 Good  |
| **Aruzz Augmented**  | 🟢 Best   | 🟢 Best     | 🟢 Best           | 🟡 Good      | 🟠 Average | 🟢 Best  |
| **BDRice Original**  | 🟡 Good   | 🟡 Good     | 🟢 Best           | 🟠 Average   | 🔴 Weak    | 🟡 Good  |
| **BDRice Augmented** | 🟢 Best   | 🟢 Best     | 🟢 Best           | 🟡 Good      | 🟠 Average | 🟢 Best  |


---

## 📦 Other Resources
To ensure the repository remains lightweight and easy to demonstrate, training notebooks, trained model checkpoints (`.pth`), and the full PDF report are intentionally omitted.

📬 You can request them at: [contact me](mailto:heyneeddev@gmail.com)

## 🚀 Getting Started

Clone the repo:
```bash
git clone https://github.com/Shourav-Deb/Rice-Vision
cd Rice-Vision
```
---
