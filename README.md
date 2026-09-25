# 🤖 Machine Learning

A structured repository documenting my journey of learning **Machine Learning, Data Science, and Artificial Intelligence** through hands-on practice, experiments, notebooks, and projects.

The goal of this repository is to build a strong understanding of Machine Learning fundamentals by combining **theory + implementation + practical projects**.

---

## 📌 About This Repository

This repository contains my Machine Learning learning journey, starting from the fundamentals of Python-based data manipulation and gradually moving toward Machine Learning algorithms and real-world projects.

It includes:

- Python for Machine Learning
- NumPy
- Pandas
- Matplotlib
- Data preprocessing
- Exploratory Data Analysis (EDA)
- Statistics for Machine Learning
- Machine Learning algorithms
- Model evaluation
- Feature engineering
- Model deployment
- End-to-end Machine Learning projects
- Google Colab notebooks
- Practice exercises and experiments

---

## 🗂️ Repository Structure

```text
Machine_Learning/
│
├── NumPy/
│   ├── numpy_basics.ipynb
│   ├── numpy_arrays.ipynb
│   ├── numpy_operations.ipynb
│   └── numpy_practice.ipynb
│
├── Pandas/
│   ├── pandas_basics.ipynb
│   ├── dataframes.ipynb
│   ├── data_cleaning.ipynb
│   └── pandas_practice.ipynb
│
├── Matplotlib/
│   ├── visualization_basics.ipynb
│   └── visualization_practice.ipynb
│
├── Data_Preprocessing/
│   ├── missing_values.ipynb
│   ├── encoding.ipynb
│   ├── feature_scaling.ipynb
│   └── feature_engineering.ipynb
│
├── Exploratory_Data_Analysis/
│   ├── eda_basics.ipynb
│   └── datasets/
│
├── Machine_Learning/
│   ├── Linear_Regression/
│   ├── Logistic_Regression/
│   ├── Decision_Trees/
│   ├── Random_Forest/
│   ├── KNN/
│   ├── SVM/
│   └── Clustering/
│
├── Projects/
│   ├── Project_1/
│   ├── Project_2/
│   └── Project_3/
│
├── README.md
└── requirements.txt
```

> The folder structure will evolve as I progress through different Machine Learning concepts and projects.

---

# 🧠 Learning Roadmap

## 1. Python for Machine Learning

Before working with Machine Learning algorithms, I am strengthening my Python fundamentals.

Topics include:

- Variables
- Data types
- Lists
- Tuples
- Dictionaries
- Sets
- Conditional statements
- Loops
- Functions
- List comprehensions
- Object-Oriented Programming
- Exception handling
- File handling
- Modules and packages

---

# 🔢 NumPy

NumPy is used for numerical computing and forms the foundation for working with numerical datasets.

### Topics

- NumPy arrays
- Array dimensions
- Array indexing
- Array slicing
- Array reshaping
- Data types
- Mathematical operations
- Broadcasting
- Aggregation functions
- Random numbers
- Matrix operations
- Dot product
- Matrix multiplication
- Array splitting
- Array joining

### Example

```python
import numpy as np

arr = np.array([[1, 2, 3],
                [4, 5, 6]])

print(arr.shape)
```

---

# 🐼 Pandas

Pandas is used for data manipulation and analysis.

### Topics

- Series
- DataFrames
- Reading datasets
- Data selection
- Filtering
- Sorting
- GroupBy
- Aggregation
- Missing values
- Duplicate values
- Data cleaning
- Merging datasets
- Joining datasets
- Exporting data

Example:

```python
import pandas as pd

df = pd.read_csv("dataset.csv")

print(df.head())
print(df.info())
print(df.describe())
```

---

# 📊 Data Visualization

Visualization helps understand patterns and relationships within datasets.

### Tools

- Matplotlib
- Seaborn

### Topics

- Line plots
- Bar charts
- Histograms
- Scatter plots
- Box plots
- Heatmaps
- Distribution plots
- Correlation visualization

---

# 🧹 Data Preprocessing

Data preprocessing is an important step before training Machine Learning models.

Topics include:

- Handling missing values
- Removing duplicates
- Detecting outliers
- Encoding categorical variables
- Feature scaling
- Normalization
- Standardization
- Feature selection
- Feature engineering
- Train/test splitting

---

# 🔍 Exploratory Data Analysis

EDA is used to understand a dataset before building a Machine Learning model.

The process includes:

```text
Dataset
   ↓
Understand the data
   ↓
Clean the data
   ↓
Analyze distributions
   ↓
Find relationships
   ↓
Detect outliers
   ↓
Identify important features
   ↓
Prepare data for modeling
```

---

# 🤖 Machine Learning

The Machine Learning section contains implementations and experiments with different algorithms.

## Supervised Learning

### Regression

- Linear Regression
- Multiple Linear Regression
- Polynomial Regression
- Regularization
  - Ridge
  - Lasso
  - Elastic Net

### Classification

- Logistic Regression
- K-Nearest Neighbors
- Support Vector Machines
- Decision Trees
- Random Forest
- Naive Bayes
- Gradient Boosting

---

# 🔵 Unsupervised Learning

Topics include:

- K-Means Clustering
- Hierarchical Clustering
- DBSCAN
- Dimensionality Reduction
- Principal Component Analysis (PCA)

---

# 📈 Model Evaluation

Understanding model performance is an important part of Machine Learning.

### Regression Metrics

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### Classification Metrics

- Accuracy
- Precision
- Recall
- F1
