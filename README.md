# 🌳 Heart Disease Prediction using Decision Trees & Random Forests

This project is part of the AI & ML Internship Task 5. It demonstrates how tree-based machine learning models can be used to classify whether a patient has heart disease based on clinical features. We use both a **Decision Tree Classifier** and a **Random Forest Classifier** to compare performance and understand feature importance.

---

## 🎯 Objective

- Build classification models using decision trees and random forests
- Visualize and interpret the decision-making process
- Evaluate models using accuracy, confusion matrix, and classification report
- Compare performance and generalizability using cross-validation

---

## 📁 Dataset

- **Source:** [Heart Disease Dataset on Kaggle](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset)
- **Attributes:** 13 features such as `age`, `chol`, `cp`, `thalach`, `sex`, `exang`, etc.
- **Target Variable:** `target` (0 = no disease, 1 = disease)

---

## 🛠 Tools & Libraries

- **Python**
- **Pandas**, **NumPy** – Data processing
- **Matplotlib**, **Seaborn** – Visualization
- **Scikit-learn** – ML models and evaluation
- **Graphviz / plot_tree** – Tree visualization

---

## 🔄 Workflow

### 1. Load and Explore Data
- Checked for nulls and datatypes
- Explored feature distributions and correlations

### 2. Data Preprocessing
- No missing values
- Split into features (`X`) and target (`y`)
- Train-test split (80/20)

### 3. Decision Tree Classifier
- Trained with controlled depth to avoid overfitting
- Visualized using `plot_tree()`
- Evaluated using accuracy, precision, recall, and F1-score

### 4. Random Forest Classifier
- Used 100 trees
- Compared accuracy with the single decision tree
- Extracted and visualized feature importances

### 5. Cross-Validation
- 5-fold CV to estimate model generalization

---

## 📊 Results

| Model          | Accuracy | Cross-Validated Accuracy  |
|----------------|----------|---------------------------|
| Decision Tree  | 0.82     | 0.78                      |
| Random Forest  | 0.87     | 0.83                      |

> ✅ Random Forest outperformed a single decision tree due to reduced overfitting and better generalization.

---

## 📈 Visual Outputs

### 🔍 Decision Tree (Max Depth = 4)
![Decision Tree]![Screenshot 2025-06-18 214918](https://github.com/user-attachments/assets/c5b69cdf-83c1-4862-8039-6119fa3c6ef9)


### ⭐ Feature Importances (Random Forest)
![Screenshot 2025-06-18 215354](https://github.com/user-attachments/assets/06026f3d-5c50-4793-9f61-e49b9238f96c)


---


