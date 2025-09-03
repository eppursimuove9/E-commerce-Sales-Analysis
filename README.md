# 📈 E-Commerce Analysis & Customer Segmentation with Machine Learning

![K-Means Clustering Elbow Method](Assets/kmeans-clustering.png)
![Product Segmentation Visualization](Assets/product-segmentation.png)
![UK Profit Visualization](Assets/uk-profit-visualization.png)

## 🚀 Live Interactive Dashboard

Explore the data and key insights through the interactive dashboard built with Plotly.

**[➡️ View Live Dashboard](https://78a5a393-d942-4685-9c26-e318f671f8e9.plotly.app/)**

---

## 📝 Project Overview

This repository contains an end-to-end data analysis for a **UK-based online retailer** specializing in gifts. Using a full year of transactional data, this project transforms raw data into actionable business intelligence through rigorous exploratory analysis, **Machine Learning** modeling, and the creation of **interactive dashboards**.

The objective is to uncover hidden patterns in customer behavior and product dynamics to answer critical business questions:
- What are our true sales trends and how does seasonality affect us?
- How can we classify thousands of products into manageable, strategic groups?
- Who are our most valuable customers and how can we target them more effectively?

This analysis provides a solid framework for data-driven decision-making to optimize inventory, personalize marketing campaigns, and drive strategic growth.

---

## 🛠️ Tech Stack

- **Language:** Python
- **Data Analysis:** Pandas, NumPy, SciPy
- **Machine Learning:** Scikit-learn (K-Means)
- **Data Visualization:** Plotly, Matplotlib, Seaborn
- **Development Environment:** Google Colab, Jupyter Notebook

---

## 📂 Repository Structure

This is the structure of the project repository:

```
├── assets/
│   ├── kmeans-clustering.png
│   ├── product-segmentation.png
│   └── uk-profit-visualization.png
├── README.md
├── ecommerce-analysis.ipynb
├── requirements.txt
```

- **`assets/`**: Contains visual resources, such as screenshots of the generated charts.
- **`ecommerce-analysis.ipynb`**: The Google Colab notebook that contains all the Python code, detailed analysis, and visualizations.
- **`requirements.txt`**: A list of all necessary Python dependencies.
- *Note: The dataset is automatically downloaded from Google Drive when running the notebook.*

---

## 📊 How to Run the Project

This project is configured for a seamless experience directly in Google Colab.

### **Step 1: Open the Notebook in Google Colab**

Click the button below to open the notebook directly in your browser. No local installation is required!

**[![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/eppursimuove9/E-commerce-Sales-Analysis/blob/main/ecommerce_analysis.ipynb)**

### **Step 2: Run the Project**

Simply run the notebook cells in order. The first cell will handle everything:
1.  **It will install all necessary libraries.**
2.  **It will automatically download the `Online-Retail.xlsx` dataset** from Google Drive.

The subsequent cells will perform the complete analysis, train the clustering model, and generate interactive dashboards. Some charts will be displayed directly within the notebook. Additionally, the scripts will generate **7 standalone HTML dashboards**. To view these, you must **download them from the Colab file explorer and open them on your local machine.**

---

## 🧠 Analysis Methodology

The project follows a structured data science workflow to ensure robust and reliable results.

1.  **Data Cleaning and Preprocessing:** Handled null values, removed duplicate and canceled transactions, and created new features like `TotalPrice` to enrich the analysis.
2.  **Exploratory Data Analysis (EDA):** Investigated sales trends over time to identify seasonality, analyzed geographical differences in order sizes, and identified data anomalies like the most returned products.
3.  **Machine Learning Modeling (Clustering):** Used the **K-Means** algorithm to segment the product catalog. The optimal number of clusters (k=4) was determined using the Elbow Method to ensure a statistically significant segmentation.
4.  **Dashboard Generation:** Created multiple interactive dashboards with Plotly to present the findings, focusing on global sales performance and strategic customer KPIs (RFM, Market Basket Analysis).

---

## 📈 Key Findings & Business Insights

### **Business Insights**
- ** Strong Seasonality:** Sales show a **massive peak in the fourth quarter (Q4)**, confirming the gift-oriented nature of the business and the critical importance of the holiday season for inventory and marketing planning.
- ** Dual Business Model (B2C & B2B):** International orders are **statistically larger** than domestic ones. This reveals a significant wholesale (B2B) business line that requires a differentiated strategy.
- ** Operational Anomalies:** The most returned item, "Manual," is not a physical product, pointing to an internal administrative process that could be optimized.

### **Strategic Product Segmentation**
The K-Means model revealed four clear and actionable product segments:

- **🏆 Core Products:** The backbone of the business. Low-price items with very high sales volume and purchase frequency. **Strategy:** Always keep in stock and feature prominently on the homepage.
- **💎 Niche / Premium:** Luxury items. High-price, low-volume, and infrequently purchased. **Strategy:** Target marketing to specific customer segments and consider a just-in-time inventory model.
- **✨ Rising Stars:** Products with potential. Moderately priced with steady sales volume. **Strategy:** Monitor closely and boost with promotions to turn them into future "Core Products."
- **📦 Bulk Bestsellers:** The foundation of the B2B business. Low-price items sold in massive volumes. **Strategy:** Manage through a dedicated B2B channel and optimize logistics for large orders.
