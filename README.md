# Heart Disease K-Means Clustering Analysis

## Project Overview

This project applies unsupervised machine learning (K-Means clustering) to analyze a heart disease dataset containing 920 patient records. The goal is to identify natural groupings of patients based on their cardiovascular health indicators.

**Kaggle Competition**: [K-Means Clustering for Heart Disease Analysis](https://www.kaggle.com/competitions/k-means-clustering-for-heart-disease-analysis/overview)

## Dataset

- **Size**: 920 patient records
- **Features**: 15 columns including clinical measurements and categorical health indicators
- **Source**: Combined data from Cleveland and VA Long Beach datasets

### Features Include:

- Demographic: age, sex
- Clinical measurements: blood pressure, cholesterol, heart rate
- Diagnostic indicators: chest pain type, ECG results, exercise-induced angina
- Test results: fasting blood sugar, ST depression, vessel fluoroscopy, thalassemia

## Project Structure

```
heart_disease_k_means_clustering/
├── heart_disease.csv              # Dataset
├── heart_disease_clustering.ipynb # Main analysis notebook
├── requirements.txt               # Python dependencies
└── README.md                      # This file
```

## Setup Instructions

### 1. Create Virtual Environment

**macOS/Linux:**

```bash
# Navigate to project directory
cd "/Users/david/Library/CloudStorage/OneDrive-Personal/Documents/CPP/Courses/Fall 2025/CS 4650/Final Project/heart_disease_k_means_clustering"

# Create virtual environment
python3 -m venv venv

# Activate virtual environment
source venv/bin/activate
```

**Windows:**

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment
venv\Scripts\activate
```

### 2. Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 3. Launch Jupyter Notebook

```bash
jupyter notebook heart_disease_clustering.ipynb
```

Or use VS Code's built-in Jupyter support.

### 4. Deactivate Virtual Environment (when done)

```bash
deactivate
```

## ML Pipeline

The analysis follows the complete machine learning cycle:

### Phase 1: Preprocessing & EDA

1. **Setup & Data Loading** - Import libraries and load dataset
2. **Initial Data Exploration** - Examine shape, data types, missing values
3. **Exploratory Data Analysis** - Visualize distributions and correlations
4. **Data Preprocessing** - Handle missing values, encode categoricals, scale features

### Phase 2: Training

5. **Determine Optimal K** - Use elbow method and silhouette analysis
6. **Train K-Means Model** - Fit model with optimal number of clusters

### Phase 3: Evaluation

7. **Cluster Evaluation** - Calculate metrics (Silhouette Score, Davies-Bouldin Index, Calinski-Harabasz Index) and visualize cluster quality

## Technologies Used

- **Python 3.8+**
- **Data Analysis**: pandas, numpy
- **Visualization**: matplotlib, seaborn
- **Machine Learning**: scikit-learn
- **Environment**: Jupyter Notebook

## Key Results

- **Optimal Clusters**: 6 distinct patient groups identified
- **Cluster Quality**: Evaluated using multiple metrics
  - Silhouette Score: Measures sample-to-cluster fit
  - Davies-Bouldin Index: Assesses cluster separation
  - Calinski-Harabasz Index: Evaluates cluster density and separation
- **Visualizations**: Comprehensive plots including cluster distributions, silhouette plots, and metric comparisons
- **Clinical Insights**: Clusters reveal patterns in chest pain types, ECG responses, and cardiovascular risk profiles

## Contributors

- [David Lam](https://github.com/davidgit3000)
- [Minh Nhat Doan](https://github.com/nhatminh23-03)
- [Huynh Pham](https://github.com/HuynhPham0302)
- [Thanh Pham](https://github.com/boyvtkg)

## Notes

This is the final project for CS 4650, Fall 2025.
