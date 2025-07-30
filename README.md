# 🧠 Brain Tumor Segmentation with K-Means Clustering

> Unsupervised brain MRI segmentation using Python, OpenCV, and K-Means Clustering.  
> Clean, fast, and doesn’t need labeled data.

---

## 📌 Overview

This project segments brain tumors from MRI images using **K-Means Clustering**—a simple but powerful unsupervised learning algorithm. It's ideal for quick medical image segmentation tasks without deep learning.

---

## 🧪 Demo

| Original Image | Segmented Tumor |
|----------------|------------------|
| ![Input](results/input_sample.png) | ![Output](results/output_sample.png) |

---

## 🚀 Features

- ✅ Preprocessing (grayscale, denoising)
- ✅ K-Means clustering from `sklearn`
- ✅ Tumor region isolation
- ✅ Contour & mask overlay
- 🔜 Evaluation metrics (Dice/Jaccard)
- 🔜 Web/GUI interface

---

## 🧠 How It Works

1. Convert MRI scan to grayscale and normalize
2. Flatten and feed pixel data to **K-Means** (`k=2` or `k=3`)
3. Assign each cluster a label
4. Isolate the cluster likely to represent the tumor
5. Overlay tumor mask on original image

---
📦 Dependencies

numpy
opencv-python
scikit-learn
matplotlib
jupyter

📈 Possible Improvements

    📊 Add metrics (if ground truth available)

    🎨 Interactive GUI or web tool

    🔁 Try advanced clustering (DBSCAN, Spectral)

    🧠 Compare with deep learning methods later

    📜 License

MIT License — Free to use and modify
👨‍💻 Author

Lahiru Pramuditha
🔗 Portfolio | ✉️ lahirupramuditha0000@gmail.com | 🐙 GitHub




