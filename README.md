# Titanic Dataset Preprocessing with Label Encoding & Visualization

This repository contains a complete preprocessing pipeline for the Titanic dataset from [Kaggle](https://www.kaggle.com/datasets/yasserh/titanic-dataset). The goal is to clean and transform the data for further analysis or machine learning.

---

## 📁 Dataset

- Source: [Titanic - Machine Learning from Disaster](https://www.kaggle.com/datasets/yasserh/titanic-dataset)
- File used: `titanic.csv`

---

## 📊 Preprocessing Steps

1. **Load the dataset**  
   - View data types, null values, and statistics

2. **Handle missing values**  
   - `Age`: filled using median  
   - `Embarked`: filled using mode  
   - Dropped `Cabin` due to too many missing values  
   - Dropped rows with null `Fare`

3. **Encoding**  
   - Used `LabelEncoder` for `Sex`, `Embarked`, and `Pclass`

4. **Normalization**  
   - Applied `StandardScaler` on `Age` and `Fare` features

5. **Outlier Detection & Removal**  
   - Used IQR method to remove outliers from `Age` and `Fare`
   - Boxplots show data before and after cleaning

6. **Visualizations**  
   - Survival distribution  
   - Gender distribution  
   - Age distribution  
   - Boxplots for outlier removal

---

## 📦 Requirements

Install the required libraries using:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
