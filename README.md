
# Credit Card Customer Segmentation
## Unsupervised Machine Learning Project

---

## Project Overview
This project applies unsupervised machine learning techniques
to segment credit card customers into meaningful groups based
on their spending behavior and financial patterns.

---

## Dataset
- **Name:** CC_GENERAL.csv
- **Source:** Credit Card Customer Dataset
- **Size:** 8,950 customers, 18 features
- **Domain:** Banking and Finance

---

## Project Structure
```
project/
├── data/
│   ├── raw/                        ← Original dataset
│   └── processed/                  ← Cleaned dataset
├── notebooks/
│   └── project_analysis.ipynb      ← Main analysis notebook
├── src/
│   ├── preprocessing.py            ← Data cleaning functions
│   ├── feature_engineering.py      ← Feature creation functions
│   ├── clustering.py               ← Clustering algorithms
│   ├── evaluation.py               ← Evaluation metrics
│   └── pipeline.py                 ← Full pipeline
├── outputs/
│   ├── models/                     ← Saved models
│   ├── clusters/                   ← Final dataset with labels
│   └── reports/                    ← All plots and graphs
├── requirements.txt
├── README.md
└── main.py
```

---

## Tasks Completed
- Task 1 - Exploratory Data Analysis
- Task 2 - Data Preprocessing
- Task 3 - Feature Engineering
- Task 4 - Clustering (KMeans + Hierarchical)
- Task 5 - Cluster Evaluation
- Task 6 - Cluster Interpretation

---

## Algorithms Used
- **KMeans Clustering**
- **Hierarchical Clustering (Agglomerative)**

---

## Cluster Results

| Cluster | Label | Description |
|---|---|---|
| 0 | Inactive Users | Rarely use card, low balance |
| 1 | Active Purchasers | High purchases, pay regularly |
| 2 | Cash Advance Users | High cash advance, financially stressed |
| 3 | High Value Customers | High limit, pay in full |

---

## Evaluation Results
- KMeans outperformed Hierarchical Clustering
- Evaluated using Silhouette Score and Davies-Bouldin Index

---

## How to Run

### Install requirements
```
pip install -r requirements.txt
```

### Run the project
```
python main.py
```

---

## Deliverables
- Complete project folder with structured code
- Documented notebook with analysis
- dataset_with_clusters.csv

---

## Requirements
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- scipy
- jupyter
- kneed
- joblib
