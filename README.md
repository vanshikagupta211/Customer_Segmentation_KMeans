# 🛍️ Customer Segmentation using K-Means Clustering
### **By Vanshika Gupta**

---

## 🔍 Project Overview

This project focuses on **customer segmentation using K-Means clustering**, enhanced with **PCA (Principal Component Analysis)** for dimensionality reduction and **interactive Tableau dashboards** for business insights.

The objective is to segment customers based on **demographics and spending behavior** to help businesses:
- Identify high-value customers
- Understand customer behavior patterns
- Enable targeted marketing and retention strategies

---

## 📂 Dataset Source

This project uses a publicly available Kaggle dataset as the raw data source and a processed dataset generated during analysis.

🔹 Raw Dataset (Original Source)

The original dataset was sourced from Kaggle:

🔗 **Customer Segmentation Dataset**  
https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python

Raw dataset contains:
  - Customer demographics
  - Income levels
  - Spending behavior

🔹 Processed Dataset (Used for Dashboard & Modeling)

A cleaned and feature-engineered version of the dataset was created during the analysis and is included in this repository:

📄 **Processed Dataset:**  
[Data/customer_segments.csv](Data/customer_segments.csv)

This processed dataset contains:
  - Cluster labels (K-Means output)
  - Segment names
  - PCA components (PC1, PC2)
  - Ready-to-use structure for Tableau dashboards

---

## 🧠 Business Problem

Businesses often struggle to:
- Identify profitable customer groups
- Understand spending behavior vs income
- Design targeted marketing strategies

This project solves that by:
- Grouping customers into meaningful segments
- Visualizing patterns through dashboards
- Providing actionable insights for decision-makers

---

## 🔧 Tools & Technologies
- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)
- K-Means Clustering
- PCA (Principal Component Analysis)
- Tableau Desktop / Tableau Reader

---

## 📌 Methodology

### **Data Preparation**
- Loaded and inspected customer demographic and spending data
- Handled data quality issues and validated data types
- Selected key numerical features for clustering:
  - Age
  - Annual Income
  - Spending Score
- Standardized features using **StandardScaler** to ensure equal contribution to distance calculations

---

### **Exploratory Data Analysis (EDA)**
- Analyzed feature distributions and relationships
- Visualized correlations and patterns among income, age, and spending behavior
- Identified natural customer group tendencies prior to modeling

---

### **Optimal Cluster Selection**
- Applied the **Elbow Method (WCSS)** to identify potential cluster counts
- Evaluated cluster quality using the **Silhouette Score**
- Compared multiple `k` values to balance cluster separation and interpretability

---

### **K-Means Clustering**
- Trained **K-Means model** with optimal cluster count
- Assigned cluster labels to each customer
- Validated clustering results using:
  - **Silhouette Score**
  - Cluster size distribution
  - Cluster profiling metrics

---

### **Cluster Profiling & Interpretation**
- Calculated average **Age, Income, and Spending Score** per cluster
- Assigned **business-friendly segment names** based on customer behavior
- Interpreted each cluster from a marketing and business perspective

---

### **PCA (Principal Component Analysis)**
- Reduced multi-dimensional feature space to **2 principal components**
- Visualized cluster separation in a 2D PCA space
- Verified cluster compactness and separation visually

---

### **Visualization & Analysis**
- Built **interactive Tableau dashboards** using model output
- Implemented:
  - Filters (Segment, Gender, Income range)
  - Parameters and dashboard actions
  - Reset functionality for enhanced usability
- Designed dashboards for both:
  - **Executive overview**
  - **Customer behavior deep-dive analysis**

---

## 📊 Visualization & Dashboarding (Tableau)

This project includes **two professionally designed Tableau dashboards** built for executive-level storytelling and deep analytical exploration.

### 🔹 Dashboard 1: Customer Segmentation Overview
- High-level distribution of customer segments
- Segment-wise and gender-wise customer breakdown
- Interactive donut charts with dynamic labels
- KPI-style customer counts
- Global dashboard filters for:
  - Segment
  - Gender
  - Income range
  - Spending score

### 🔹 Dashboard 2: Customer Behavior Deep Dive
- Income vs Spending scatter plot with cluster coloring
- PCA-based 2D cluster separation with reference lines
- Advanced tooltips displaying:
  - Gender
  - Age
  - Income
  - Spending score
  - Segment name
- Interactive filtering using **dashboard actions**
- Parameter-driven views for flexible data exploration

### 🔹 Advanced Tableau Features Implemented
- **Parameters** for dynamic dimension switching
- **Calculated fields** for:
  - Segment labeling
  - Dynamic titles
  - Tooltip customization
- **Dashboard actions** (click-to-filter behavior)
- **Reset Filters button** using parameter actions
- Consistent color palette and professional layout design
- Tiled dashboard layout optimized for portfolio viewing

These dashboards are designed to simulate **real-world business intelligence applications**, enabling stakeholders to explore customer behavior interactively and derive actionable insights.

---

## 📊 Tableau Dashboard Preview

### **Customer Segmentation Overview**
![Overview](Images/customer_segmentation_overview.png)

### **Customer Behavior Deep Dive**
![Deep Dive](Images/customer_behavior_deep_dive.png)

### **PCA Cluster Separation (2D)**
![PCA](Images/pca_cluster_2d.png)

---

## 📌 Key Insights
- **Premium High Spenders** generate the highest revenue
- **Young Budget High Spenders** show strong engagement despite lower income
- **High income does not always high spending**
- **Potential Loyalists** represent strong upsell opportunities
- PCA confirms **well-separated clusters** validating the K-Means model

---

## 📝 Conclusion

This project demonstrates an end-to-end customer segmentation workflow combining:

- Machine Learning
- Dimensionality reduction
- Business intelligence dashboards

It highlights how data-driven insights can directly support strategic business decisions.

---

## 📈 How to Run the Project

### Python Analysis

Install dependencies:

```
pip install -r requirements.txt
```

## Open the Jupyter Notebook:

[Notebook/Customer Segmentation.ipynb](Notebook/Customer%20Segmentation.ipynb)

## Tableau Dashboard

Download the Tableau dashboard file:  
[Dashboard/Customer Segmentation Analysis – K-Means Clustering.twbx](Dashboard/Customer%20Segmentation%20Analysis%20–%20K-Means%20Clustering.twbx)

Open this file using **Tableau Desktop** or **Tableau Reader**.

---

## 📂 Folder Structure

```
Customer_Segmentation_KMeans/
│
├── Dashboard/
│ └── Customer Segmentation Analysis – K-Means Clustering.twbx
│
├── Data/
│ └── customer_segments.csv
│
├── Images/
│ ├── customer_segmentation_overview.png
│ ├── customer_behavior_deep_dive.png
│ └── pca_cluster_2d.png
│
├── Notebook/
│ └── Customer_Segmentation.ipynb
│
├── README.md
└── requirements.txt
```

👩‍💻 Author

Vanshika Gupta

Data Scientist | Machine Learning | Python | Tableau


