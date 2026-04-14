**Online Retail Customer Intelligence System**

## 📌 Project Overview
This project demonstrates an **end-to-end Machine Learning workflow** using a real-world **Online Retail transactional dataset**.  
The same dataset is used to implement:

- ✅ **Unsupervised Learning** (Customer Segmentation)


The project focuses on extracting **business insights** and predicting **high-value customers**

---

## 📊 Dataset Information
- **Dataset Name:** Online Retail II (UCI)
- **Source:** Kaggle  
- **Dataset Link:** https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci

### Key Columns
- `Invoice`
- `StockCode`
- `Description`
- `Quantity`
- `InvoiceDate`
- `Price`
- `Customer ID`
- `Country`

---

## 🎯 Project Objectives
- Understand customer purchasing behavior
- Segment customers based on spendings using unsupervised learning
- Predict high-value customers using supervised learning


---

## 🔄 Project Workflow
Data Loading  
↓  
Exploratory Data Analysis (EDA)  
↓  
Data Cleaning & Preprocessing  
↓  
Feature Engineering (RFM Analysis)  
↓  
Unsupervised Learning (Clustering)  

---

## 🧪 Methodology

### 1️⃣ Data Loading
- Loaded dataset using Pandas
- Initial inspection using `.head()`, `.info()`, and `.describe()`

---

### 2️⃣ Exploratory Data Analysis (EDA)
- Missing value analysis
- Quantity and unit price distribution
- Country-wise sales analysis
- Time-based (monthly) sales trends
- Identification of outliers and returns

---

### 3️⃣ Data Cleaning
- Removed missing `CustomerID`
- Removed negative quantities (product returns)
- Removed zero or negative prices
- Created `TotalPrice = Quantity × UnitPrice`
- Removed duplicate records

---

### 4️⃣ Feature Engineering – RFM Analysis
Created customer-level features:
- **Recency:** Days since last purchase
- **Frequency:** Number of invoices per customer
- **Monetary:** Total spending per customer

---

### 5️⃣ Unsupervised Learning – Customer Segmentation
- Algorithm used: **KMeans Clustering**
- Optimal number of clusters selected using:
  - Elbow Method

#### Customer Segments Identified
| Segment | Description |
|------|------------|
| High-Value Customers | Frequent, recent, high spenders |
| Regular Customers | Moderate engagement and spending |
| At-Risk Customers | Infrequent purchases, low spending |


---

## 🗂️ Project Structure
```
AI-Driven Online Retail Customer Intelligence System/
│
├── notebooks/
│   └── Customer_Segmentation_and_RFM.ipynb
│
├── README.md
└── requirements.txt
```

---

## 🛠️ Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- Jupyter Notebook

---

## 📚 Key Learnings
- Converting transactional data into ML-ready features
- Applying unsupervised learning for customer segmentation
- Creating supervised learning labels from business insights

**Dashboard Preview**

![Dashboard Preview](https://github.com/mahir863/Online-Retail-System/blob/main/retail_sales_data.png)
---

