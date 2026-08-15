# 🌆 Urban Change Detection using Sentinel-2

This project uses **Google Earth Engine** and **Machine Learning** to detect urban expansion between 2021 and 2025 using Sentinel-2 satellite imagery. The study area is located in **Chhattisgarh, India** (near 22.07°N, 82.14°E).

---

## 📌 Overview

Urbanization is rapidly changing land use patterns. This project analyzes multi-temporal Sentinel-2 imagery to identify areas that have undergone significant change — specifically, the expansion of built-up areas. We use spectral indices like **NDVI**, **NDBI**, and **NDWI**, and apply **Random Forest**, **SVM**, and **CNN** models to classify change vs. no-change pixels.

---

## ✨ Features

- 🌍 **Study Area:** 22.065°N – 22.095°N, 82.125°E – 82.155°E
- 🛰️ **Data:** Sentinel-2 Surface Reflectance (COPERNICUS/S2_SR_HARMONIZED)
- 📊 **Indices:** NDVI, NDBI, NDWI
- 🤖 **Models:** Random Forest, Support Vector Machine, Convolutional Neural Network
- 📈 **Change Detection:** NDBI difference (2025 – 2021) threshold-based labeling
- 🗺️ **Visualization:** Interactive maps using `geemap`, RGB composites, and change maps

---

 Acknowledgements
Google Earth Engine for providing free access to satellite data.

Open-source libraries that made this analysis possible.

## 🗂️ Repository Structure

📁 sentinel2-urban-change/
├── 📄 C_RF.ipynb # Main Jupyter Notebook (Google Colab)
├── 📄 README.md # Project description
├── 📄 requirements.txt # Python dependencies
├── 📄 .gitignore # Files to ignore


---

## 🚀 Getting Started

### Prerequisites
- A **Google Earth Engine** account ([sign up here](https://earthengine.google.com/))
- Google Colab or local Jupyter environment

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/sumi29910/sentinel2-urban-change.git
   cd sentinel2-urban-change

  pip install -r requirements.txt

  Authenticate Earth Engine

The notebook will prompt you to authenticate with Earth Engine.

Follow the link, sign in, and copy the authorization code back to Colab.

📊 How to Run
Open the notebook in Google Colab:
https://colab.research.google.com/assets/colab-badge.svg

Run all cells sequentially.

The notebook will:

Load Sentinel-2 imagery

Compute spectral indices

Extract training samples

Train classifiers

Generate change detection maps

🛠️ Technologies Used
Google Earth Engine — Remote sensing data & processing

geemap — Interactive mapping

Scikit-learn — ML models

TensorFlow — CNN implementation
