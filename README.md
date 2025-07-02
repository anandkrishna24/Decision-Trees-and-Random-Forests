# 🌳 Task 5 – Decision Trees & Random Forests (AI & ML Internship)

This project focuses on learning and applying tree-based models—**Decision Trees** and **Random Forests**—for binary classification. The dataset used is the [Heart Disease Dataset](https://www.kaggle.com/datasets/johnsmith88/heart-disease-dataset) from Kaggle.

---

## 📁 Dataset Summary

- **Dataset**: Heart Disease UCI
- **Rows**: 303
- **Target Column**: `target` (0 = No Disease, 1 = Heart Disease)
- **Features**: 13 health-related attributes (e.g., `age`, `cholesterol`, `thal`, `cp`)

---

## 🛠 Tools & Libraries Used

- **Programming Language**: Python
- **Libraries**:  
  - `pandas`, `numpy` for data handling  
  - `matplotlib`, `seaborn` for visualization  
  - `scikit-learn` for model training, evaluation, and tree visualization

---

## 🔍 Problem Statement

> Build classification models to predict whether a person has heart disease using Decision Tree and Random Forest algorithms.  
> Evaluate model performance and understand model behavior using feature importances and visualizations.

---

## 🚀 Workflow Summary

### 1. Data Preprocessing
- Loaded the dataset (`heart.csv`)
- Separated features and target (`X`, `y`)
- Applied train-test split (80% train, 20% test)
- Standardized the features using `StandardScaler`

---

### 2. Decision Tree Classifier
- Trained a default Decision Tree model.
- Visualized the full tree using `plot_tree()`.
- Evaluated on test set using:
  - Accuracy
  - Classification report (precision, recall, F1-score)
- Example Result:  
  **Accuracy**: ~79%

---

### 3. Pruned Decision Tree
- Limited `max_depth` to 3 to avoid overfitting.
- Evaluated pruned model performance.
- Example Result:  
  **Accuracy (pruned)**: ~77%

---

### 4. Random Forest Classifier
- Trained a `RandomForestClassifier` with 100 trees.
- Evaluated test performance.
- Extracted and plotted feature importances.
- Example Result:  
  **Accuracy**: ~85%

---

### 5. Cross-Validation
- Applied 5-fold cross-validation to both models.
- Compared average cross-validation scores.
- Results:
  - **Decision Tree (CV)**: ~75%
  - **Random Forest (CV)**: ~83%

---

## 📊 Feature Importance (Top 5)
| Feature        | Importance |
|----------------|------------|
| ca             | High       |
| thal           | High       |
| cp             | Medium     |
| oldpeak        | Medium     |
| chest pain (cp)| Medium     |

These help identify which medical indicators are most predictive of heart disease.

---

## 📘 What I Learned

- How to build and visualize decision trees.
- How overfitting can occur in deep trees.
- How to prune trees by setting `max_depth`.
- Why Random Forests are more stable and accurate.
- How to extract and interpret feature importance.
- How to evaluate using cross-validation.

---
