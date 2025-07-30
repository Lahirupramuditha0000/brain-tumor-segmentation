# 🧠 Brain Tumor Segmentation with Mean Shift Clustering

> Unsupervised brain MRI segmentation using Python, OpenCV, and Mean Shift Clustering.  
> No labeled data. No deep learning. Just pure clustering wizardry.

---

## 📌 Overview

This project implements an **unsupervised approach** to detect and segment brain tumors from MRI scans using **Mean Shift Clustering**. It’s lightweight, interpretable, and doesn't require training on huge datasets.

---

## 🧪 Demo

| Original Image | Segmented Tumor |
|----------------|------------------|
| ![Input](results/input_sample.png) | ![Output](results/output_sample.png) |

---

## 🚀 Features

- ✅ Preprocessing (grayscale, smoothing, etc.)
- ✅ Mean Shift clustering from `sklearn`
- ✅ Tumor region extraction
- ✅ Visualization overlays
- 🔜 Dice/Jaccard Score (optional)
- 🔜 GUI or CLI pipeline

---

## 🧠 How It Works

1. Load brain MRI image
2. Preprocess: grayscale, noise reduction, normalization
3. Reshape image and apply **Mean Shift Clustering**
4. Extract cluster(s) representing tumor
5. Overlay and visualize segmented output

---

## 📂 Project Structure

