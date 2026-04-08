# Customer Segmentation using RFM Analysis & K-Means Clustering

This repository presents a comprehensive customer segmentation analysis based on retail transaction data. Using RFM (Recency, Frequency, Monetary) features and K-Means clustering, customers are grouped into meaningful segments to support data-driven marketing strategies.

The project includes a fully documented Jupyter Notebook and a structured analytical report.

---

## Project Overview

**Goal**  
Segment customers based on purchasing behavior using RFM analysis and unsupervised learning.

**Techniques**
- Data cleaning and preprocessing of real-world transactional data  
- Feature engineering using the RFM model  
- Clustering using K-Means  
- Evaluation using Silhouette Score and Davies-Bouldin Index  
- Interpretation of clusters and derivation of marketing strategies  

**Language**
- The notebook and report are written in **German**  

---

## Report (Important)

This project includes a detailed analytical report (in German) documenting the full workflow.

**Contents**
- Problem definition and business context  
- Dataset description (UCI Online Retail dataset)  
- Data preprocessing and cleaning methodology  
- Exploratory Data Analysis (EDA)  
- RFM feature engineering  
- Clustering approach and model selection  
- Evaluation of clustering results  
- Interpretation of customer segments  
- Marketing strategy derivation  
- Critical discussion and conclusions  

---

## Team Contribution

**Egehan Kilic**
- Data preprocessing and cleaning  
- Cluster interpretation  
- Marketing strategy derivation  
- Report writing  

**Ahmet Topal**
- Data preparation  
- Exploratory Data Analysis (EDA)  
- Visualization  
- Report structuring  

**Enis Cobanoglu**
- Clustering methodology selection  
- K-Means implementation  
- Model evaluation  
- Contribution to report and presentation  

---

## Dataset

**Source:** UCI Machine Learning Repository  
**Dataset:** Online Retail  

- ~540,000 transactions  
- ~4,300 customers after preprocessing  
- Real-world retail dataset  

---

## Methodology

### Data Preprocessing
- Removal of missing `CustomerID` values  
- Exclusion of cancellations (`InvoiceNo` starting with "C")  
- Filtering invalid values (`Quantity <= 0`, `UnitPrice <= 0`)  
- Creation of revenue feature (`Quantity × UnitPrice`)  

### Feature Engineering (RFM)
- **Recency:** Days since last purchase  
- **Frequency:** Number of transactions  
- **Monetary:** Total spending per customer  

### Clustering
- Algorithm: **K-Means**  
- Feature scaling using **StandardScaler**  
- Fixed random state for reproducibility  

---

## Evaluation

Clustering performance is evaluated using:

- **Silhouette Score** (cluster separation)  
- **Davies-Bouldin Index** (cluster compactness)  

---

## Key Results

The clustering reveals distinct customer segments such as:

- High-value loyal customers  
- Frequent low-spending customers  
- Inactive or churn-risk customers  
- High-spending but infrequent customers  

These segments can be used to support targeted marketing strategies.

---

## Features

- End-to-end data cleaning pipeline  
- RFM-based customer segmentation  
- K-Means clustering implementation  
- Quantitative evaluation of clustering quality  
- Business-oriented interpretation of results  
- Full analytical report in German  

---

## Setup

Clone the repository:
```bash
git clone https://github.com/egehank1/rfm-customer-segmentation.git
cd rfm-customer-segmentation
```

Install dependencies:
```bash
pip install pandas numpy scikit-learn matplotlib
```

Run the notebook:
```bash
jupyter notebook
```

---

## Requirements

```text
pandas==2.2.2
numpy==1.26.4
scikit-learn==1.4.2
matplotlib==3.8.4
```

---

## Future Improvements

- Explore alternative clustering algorithms (e.g., DBSCAN, Hierarchical Clustering)  
- Apply dimensionality reduction (e.g., PCA)  
- Incorporate temporal customer behavior analysis  
- Extend evaluation with additional metrics  

---

## License

This project is intended for academic purposes.
