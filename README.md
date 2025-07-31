
This project applies **K-Means Clustering** on grayscale brain MRI images to perform **unsupervised segmentation**. The goal is to separate different brain regions and isolate potential tumor areas — all without any labeled data or deep learning.

---

## 🧪 What It Does

- Reads a brain MRI in grayscale
- Flattens the image for clustering
- Applies K-Means to segment pixels into clusters (e.g., tumor vs normal tissue)
- Visualizes the cluster result
- Saves the trained model for reuse

---

## 📂 Project Structure

.
├── test_images/ # Folder for input MRI images
├── brain_tumor_kmeans.sav # Saved KMeans model

---

## 📦 Requirements

- Python 3.8+
- OpenCV
- scikit-learn
- matplotlib
- joblib

Install all dependencies:
```bash
pip install -r requirements.txt

🚀 How to Run

python segment.py

This will:

    Read test_images/0 (239).jpg

    Cluster the image using K-Means

    Display the clustered result

    Save the model as brain_tumor_kmeans.sav

💾 Model Usage

To reuse the saved KMeans model:

import joblib
model = joblib.load('brain_tumor_kmeans.sav')
predicted_labels = model.predict(new_image_flattened)

🧠 Why K-Means?

K-Means is a classic unsupervised algorithm. It works well for image segmentation when:

    You have no labeled data

    You want quick clustering by pixel intensity

    You don't want the overhead of deep learning

This project uses only intensity, but can be extended with (x, y) coordinates and more features.
📈 Future Plans

    Add spatial features (x, y) to improve clustering

    Extract likely tumor cluster based on size or brightness

    Save output masks as image files

    Use morphological ops to refine tumor mask

    Try DBSCAN or Spectral Clustering for comparison

👨‍💻 Author

Lahiru Pramuditha
📫 lahirupramuditha0000@gmail.com
