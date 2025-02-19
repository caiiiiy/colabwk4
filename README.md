# 🚀 Unsupervised Learning for Earth Observation Data

## 📌 Overview
This repository contains Jupyter Notebooks demonstrating **unsupervised learning techniques** applied to **Earth Observation (EO) data**. The main focus is on clustering algorithms such as **K-means** to classify **sea ice and leads** using **Sentinel-2 optical data** and **Sentinel-3 altimetry data**.

## 📂 Files in this Repository
- **`Chapter1_Unsupervised_Learning_Methods.ipynb`**  
  - Introduces **unsupervised learning methods**, specifically **K-means clustering**.
  - Covers classification of **sea ice vs. lead** using **Sentinel-2 and Sentinel-3 data**.

- **`colab1.ipynb`**  
  - This notebook performs **data processing, clustering, and visualization** using satellite data.
  - Uses **Google Colab** for execution, requiring **Google Drive access** for dataset storage.
  - Outputs **clustering results** with color-coded scatter plots and waveform alignments.

## 🛠️ How to Use the Notebooks
1. **Clone this repository**:
   ```bash
   git clone https://github.com/caiiiiy/colabwk4.git
   ```
2. **Install dependencies**:
   ```bash
   pip install rasterio netCDF4
   ```
3. **Open and run the notebooks**:
   - In **Google Colab**, upload the notebook and run the cells step by step.
   - In **Jupyter Notebook**, open locally and execute.

## 📊 Key Features
### 📌 Unsupervised Learning Concepts
- **K-means clustering**: Explained with practical implementation.
- **Cluster evaluation**: Using metrics to assess segmentation quality.
- **Satellite data processing**: Handling **Sentinel-2 and Sentinel-3** datasets.

### 🎨 Visualizations & Analysis
- **Scatter Plots of Clustered Data**:  
  - Different colors represent **clusters**.
  - Plots of (`sig_0` vs. `PP`), (`sig_0` vs. `SSD`), and (`PP` vs. `SSD`).
  
- **Waveform Alignment Using Cross-Correlation**:  
  - Aligns **10 equally spaced waveforms** using **cross-correlation**.
  - Helps identify common features across different clusters.

- **Histogram Analysis**:  
  - Echo distributions for **lead clusters** and **sea ice clusters**.
  - Reveals variability in **echo intensities**.

## 🔍 Annotations from [Issue #1](https://github.com/caiiiiy/colabwk4/issues/1)
The following insights were provided in the issue discussions:
- **Clustering Results**: Evaluated using both **Gaussian Mixture Model (GMM)** and **K-means**.
- **Feature Selection**: `sig_0`, `PP`, and `SSD` were used for classification.
- **Performance Comparison**: K-means provides **rigid segmentation**, while GMM captures **subtle variations**.
- **Recommended Improvements**:
  - Normalize spectral features for better cluster separation.
  - Optimize GMM covariance types for smoother clustering.
  - Validate clustering quality using **silhouette scores**.

## 🏆 References
- **GEOL0069 Jupyter book**. *[https://cpomucl.github.io/GEOL0069-AI4EO/intro.html]*.

## 🤝 Contributions
Feel free to:
- Open an **issue** for improvements.
- Submit a **pull request** for additional analyses or dataset extensions.

🚀
```
