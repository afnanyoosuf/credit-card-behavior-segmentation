%%writefile /content/README.md

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
project/
├── data/
│   ├── raw/                        
│   └── processed/                  
├── notebooks/
│   └── project_analysis.ipynb      
├── src/
│   ├── preprocessing.py            
│   ├── feature_engineering.py      
│   ├── clustering.py               
│   ├── evaluation.py               
│   └── pipeline.py                 
├── outputs/
│   ├── models/                     
│   ├── clusters/                   
│   └── reports/                    
├── requirements.txt
├── README.md
└── main.py

---

## Tasks Completed
- Task 1 - Exploratory Data Analysis
- Task 2 - Data Preprocessing
- Task 3 - Feature Engineering
- Task 4 - Clustering (KMeans + Hierarchical)
- Task 5 - Cluster Evaluation
- Task 6 - Cluster Interpretation
- Bonus  - Power BI Dashboard

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

## Bonus — Power BI Dashboard
A Power BI dashboard was created to explore cluster insights visually.

### Dashboard Contains
- KPI Cards showing customer count per cluster
- Pie Chart showing cluster distribution
- Bar Chart showing average balance per cluster
- Bar Chart showing average purchases per cluster
- Scatter Plot showing cash advance vs purchases
- Bar Chart showing credit limit per cluster
- Bar Chart showing full payment rate per cluster
- Interactive Slicer to filter by cluster label

### Dashboard File
- CreditCardClusterDashboard.pbix

### Key Dashboard Insights
- High Value Customers have highest credit limit and full payment rate
- Cash Advance Users have highest cash advance and lowest purchases
- Active Purchasers show highest purchase amounts
- Inactive Users show low activity across all metrics

---

## How to Run

### Install requirements
pip install -r requirements.txt

### Run the project
python main.py

---

## Deliverables
- Complete project folder with structured code
- Documented notebook with analysis
- dataset_with_clusters.csv
- CreditCardClusterDashboard.pbix (Bonus)

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
