# 💳 Credit Card Lead Prediction — Bank Cross-Sell ML Model

![Python](https://img.shields.io/badge/Python-3.8+-blue?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?style=for-the-badge&logo=jupyter&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-green?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=for-the-badge)

---

## 📌 Project Overview

**Happy Customer Bank** is a mid-sized private bank offering products such as savings accounts, investment products, and credit cards. This project helps the bank identify which **existing customers are most likely to convert** when offered a credit card.

Using customer profile data and banking relationship attributes, a **binary classification model** is built to predict whether a customer will show interest (`Is_Lead = 1`) or not (`Is_Lead = 0`).

---

## 🏦 Business Problem

The bank uses multiple channels (tele-calling, email, net banking, mobile banking) to cross-sell credit cards to existing customers. Manually targeting all customers is inefficient. This model enables **targeted marketing** by identifying high-intent prospects, reducing costs and improving conversion rates.

---

## 🗂️ Dataset Description

| Split | Rows | Columns |
|-------|------|---------|
| Train | 245,725 | 11 |
| Test | 105,312 | 10 |

### Features

| Feature | Description |
|---------|-------------|
| `ID` | Unique customer ID |
| `Gender` | Customer gender |
| `Age` | Customer age |
| `Region_Code` | Anonymised regional code |
| `Occupation` | Employment type |
| `Channel_Code` | Acquisition channel |
| `Vintage` | Months as a customer |
| `Credit_Product` | Existing credit product holder |
| `Avg_Account_Balance` | Average bank account balance |
| `Is_Active` | Active customer flag |
| `Is_Lead` | **Target** — 1 if interested in credit card |

> **Note:** `Credit_Product` has ~11% missing values, imputed using mode.

---

## 🎯 Objectives

- Perform **data inspection** and understand class distribution
- Handle **missing values** in categorical features
- Conduct **Exploratory Data Analysis** with visualisations
- Encode categorical variables using **Label Encoding**
- Train a **classification model** to predict lead conversion
- Evaluate model performance using appropriate metrics

---

## 🔍 Analysis Highlights

- `Is_Lead` distribution is **imbalanced** — visualised using Seaborn countplot
- `Credit_Product` is the only feature with missing values (~11%) — filled with mode
- Both categorical and numerical features are identified and processed separately
- Feature engineering: Label encoding for all categorical columns

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| Python 3.8+ | Core language |
| Pandas | Data manipulation |
| NumPy | Numerical computing |
| Matplotlib / Seaborn | Visualisation |
| Scikit-learn | Preprocessing, modelling, evaluation |

---

## 📁 Project Structure

```
Credit-Card-Lead-Prediction/
│
├── final credit card project.ipynb   # Main analysis notebook
├── train_s3TEQDk.csv                 # Training dataset
├── test_mSzZ8RL.csv                  # Test dataset
├── sample_submission_eyYijxG.csv     # Sample submission format
└── README.md                         # Project documentation
```

---

## 🚀 How to Run

### 1. Clone the repository
```bash
git clone https://github.com/homeshwarnelakurthi/Credit-Card-Lead-Prediction.git
cd Credit-Card-Lead-Prediction
```

### 2. Install dependencies
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
```

### 3. Open the notebook
```bash
jupyter notebook "final credit card project.ipynb"
```

---

## 👨‍💻 Author

**Homeswar Rao Nelakurthi**  
[![GitHub](https://img.shields.io/badge/GitHub-homeshwarnelakurthi-181717?style=flat&logo=github)](https://github.com/homeshwarnelakurthi)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
