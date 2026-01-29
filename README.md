# 🏦 Bank Customer Churn Prediction & Data Mining

This project aims to identify bank members likely to leave the institution (churn) to help implement targeted customer relationship management campaigns. It covers the entire data science pipeline: from complex data cleaning and fusion to predictive modeling and feature importance analysis.

## 📊 Business Problem
The objective is to produce an "attrition score" representing the probability of a customer resigning. By analyzing historical data of former members and current clients, the model identifies high-risk profiles based on their demographic and banking behavior.

## 🛠️ Data Engineering & Preprocessing
Real-world banking data is often messy. This project involved significant effort in:
* **Data Cleaning:** Handled missing values and identified aberrant data (e.g., placeholder dates like 0000-00-00).
* **Data Fusion:** Merged fragmented CSV tables to create a unified dataset for training.
* **Feature Engineering:** * Recoding categorical variables (gender, family status, client types).
    * Calculating temporal features such as "Member Seniority" (Years since joining).
* **Dimensionality Reduction:** Applied techniques to improve model performance and computational efficiency.

## 🤖 Predictive Modeling
We compared different classification algorithms to find the most accurate model for predicting churn:
1. **Support Vector Machine (SVM)**
2. **k-Nearest Neighbors (kNN)**
3. **Naive Bayes**

### Performance Evaluation
The models were evaluated using a strict split of Training, Validation, and Test sets to ensure the scores reflect real-world generalization. Key metrics tracked include Accuracy, Precision, and Recall.

## 📂 Project Structure
* `Bank.ipynb`: Complete Jupyter Notebook containing data exploration, cleaning, and model training.
* `Data/`: Data to work with.
* `Documentation/Rapport_APP_BI_Data_Mining.pdf`: Full technical report detailing the methodology and statistical analysis.

## ⚙️ Installation & Execution
1. **Requirements:**
   ```bash
   pip install pandas numpy scikit-learn matplotlib seaborn
   ```
2. **Run: Launch the Jupyter Notebook:**

```bash
jupyter notebook Bank.ipynb
```
---
*Developed as part of the Business Intelligence Master's curriculum at Avignon University.*
