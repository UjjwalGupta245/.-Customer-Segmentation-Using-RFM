# Customer Segmentation Using RFM

## Overview
This repository demonstrates the implementation of **Customer Segmentation** using the **RFM (Recency, Frequency, Monetary)** model and **K-Means clustering**. The analysis focuses on segmenting customers of an online retail store based on their purchasing behaviour, providing actionable insights to enhance customer engagement and marketing strategies.

---

## Table of Contents
- [Overview](#overview)
- [About RFM Analysis](#about-rfm-analysis)
- [Features of the Project](#features-of-the-project)
- [Dataset](#dataset)
- [Project Workflow](#project-workflow)
- [Insights and Findings](#insights-and-findings)

---

## About RFM Analysis
**RFM** is a technique used in marketing to evaluate and segment customers based on their purchasing behavior:

- **Recency (R):** How recently a customer made a purchase.
- **Frequency (F):** How often a customer makes purchases.
- **Monetary (M):** How much money a customer spends.

By assigning scores to each customer for R, F, and M metrics, we can create meaningful customer segments and design targeted strategies for each group.

---

## Features of the Project
1. **Data Cleaning:**
   - Removed duplicates and irrelevant data.
   - Handled missing values.
   - Filtered valid transactions (excluding cancellations and refunds).

2. **RFM Feature Engineering:**
   - Computed Recency, Frequency, and Monetary values for each customer.
   - Scored customers based on their RFM metrics.

3. **K-Means Clustering:**
   - Scaled data using `StandardScaler` for normalization.
   - Used the **Elbow Method** to determine the optimal number of clusters.
   - Applied K-Means clustering to segment customers.

4. **Data Visualization:**
   - Visualized RFM metrics and clusters using scatter plots, heatmaps, and bar charts.

5. **Insights Generation:**
   - Identified key customer segments such as "High-Value Customers" and "At-Risk Customers."

---

## Dataset
The dataset is from an online retail store, containing transactional data, including:
- **Customer ID**
- **Invoice Date**
- **Invoice Number**
- **Transaction Amount**

(Note: Actual data files are available in the `data/` directory. Ensure the dataset is clean before proceeding.)

---

## Project Workflow
1. **Data Cleaning**:
   - Handle missing values and filter relevant data.

2. **RFM Analysis**:
   - Compute Recency, Frequency, and Monetary values.
   - Score customers and create RFM segments.

3. **Scaling and Clustering**:
   - Scale the RFM data using `StandardScaler`.
   - Determine the optimal number of clusters using the **Elbow Method**.
   - Perform K-Means clustering.

4. **Visualization and Insights**:
   - Visualize clusters and generate actionable insights.

---

3. Follow the Jupyter notebooks in the `notebooks/` directory to reproduce the analysis:
   - `01_data_cleaning.ipynb`
   - `02_rfm_analysis.ipynb`
   - `03_clustering_kmeans.ipynb`
   - `04_visualization.ipynb`

---

## Insights and Findings
Through the analysis, the following customer segments were identified:

1. **High-Value Customers**: Recently purchased, frequent buyers, and high spenders.
2. **Loyal Customers**: Frequent buyers with moderate spending.
3. **At-Risk Customers**: Customers who haven't purchased recently and have low spending.
4. **Potential Loyalists**: Customers who recently purchased and spent a significant amount but have low frequency.

These insights can be used to:
- Target marketing campaigns.
- Design loyalty programs for high-value customers.
- Re-engage at-risk customers.

---

