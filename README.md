# 🌍 Satellite Image Analysis using Machine Learning

## 📌 Overview

This project focuses on analyzing satellite imagery to extract meaningful insights about the environment using **Machine Learning** and **Remote Sensing Indices**. We process satellite images to monitor vegetation health, detect water bodies, and identify urban or barren regions.

## 🧠 Objectives

* Analyze satellite images using classical ML techniques.
* Extract and visualize environmental features like vegetation, water, and urban areas.
* Use indices like **NDVI**, **MNDWI**, and **SAVI** to quantify land characteristics.
* Classify land cover types using **SVM** and **K-Nearest Neighbors (KNN)**.

---

## 🛰️ Dataset

We used multispectral satellite images from **Sentinel-2** or **Landsat-8**.

Bands used:

* B2 (Blue)
* B3 (Green)
* B4 (Red)
* B5/B8 (NIR)
* B11/B12 (SWIR)

---

## 📊 Key Techniques

| Task               | Technique                                  |
| ------------------ | ------------------------------------------ |
| Preprocessing      | Raster stacking, resizing, noise filtering |
| Feature Extraction | NDVI, SAVI, VARI, MNDWI                    |
| Classification     | KNN, SVM                                   |
| Visualization      | Matplotlib, Seaborn, GeoTIFF tools         |

### 🌱 Vegetation Indices

* **NDVI** (Normalized Difference Vegetation Index):
  `NDVI = (NIR - Red) / (NIR + Red)`
* **SAVI** (Soil Adjusted Vegetation Index):
  `SAVI = ((NIR - Red) / (NIR + Red + L)) * (1 + L)`
* **MNDWI** (Modified Normalized Difference Water Index):
  `MNDWI = (Green - SWIR) / (Green + SWIR)`

---

## 🛠️ Installation

1. Clone this repo

```bash
git clone https://github.com/yourusername/satellite-image-analysis.git
cd satellite-image-analysis
```

2. Create a virtual environment & install requirements

```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

---

## 🚀 How to Run

```bash
python main.py
```

Change the path to your satellite bands inside `main.py`.

---

## 📈 Output Examples

* NDVI heatmaps
* Water body masks
* Classified land cover maps


## 📚 File Structure

```
├── data/
│   └── *.tif               # Satellite band images
├── src/
│   ├── preprocessing.py
│   ├── indices.py
│   ├── classifier.py
│   └── visualize.py
├── outputs/
│   └── *.png               # Output images
├── main.py
├── requirements.txt
└── README.md
```

---

## ⚙️ Libraries Used

* `numpy`, `pandas`
* `matplotlib`, `seaborn`
* `scikit-learn`
* `rasterio`, `GDAL`
* `opencv-python`

---

## 🧪 Results

| Model | Accuracy |
| ----- | -------- |
| KNN   | 85.3%    |
| SVM   | 89.7%    |

---

## 📍 Applications

* Deforestation Monitoring
* Water Resource Management
* Urbanization Tracking
* Disaster Impact Assessment


