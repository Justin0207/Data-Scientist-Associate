# Data-Scientist-Associate
This is a repository containing my submission in the Datacamp DSA certification examination.

# 🛵 Moped Ownership Prediction

This repository presents a machine learning solution for **EMO**, a motorcycle manufacturer, to identify reviews submitted by people who never owned their electric moped. Owner feedback is essential for improving the product, and this solution helps filter out reviews from non-owners using a classification model.

---

## 🧐 Business Overview

EMO launched its first electric moped in India in 2019. Reviews are a key source of insight for the product team—but fake or irrelevant reviews (especially from non-owners) can distort decision-making.

### ❓ Customer Question

> Can you predict which reviews come from people who have never owned the moped before?

---

## 🧩 Dataset Overview

The dataset comes from a local moped review website and is available at: moped.csv



| Column Name       | Description |
|-------------------|-------------|
| `Used it for`     | Purpose of use: "Commuting" or "Leisure" |
| `Owned for`       | Ownership status: `<= 6 months`, `> 6 months`, or `Never Owned` <br> → Converted to: `Owned` vs `Never Owned` |
| `Model name`      | Moped model name |
| `Visual Appeal`   | Rating (1-5), missing values filled with `0` |
| `Reliability`     | Rating (1-5), missing values filled with `0` |
| `Extra Feature`   | Rating (1-5), missing values filled with `0` |
| `Comfort`         | Rating (1-5), missing values filled with `0` |
| `Maintenance cost`| Rating (1-5), missing values filled with `0` |
| `Value for money` | Rating (1-5), missing values filled with `0` |

---

## 🔄 Data Preprocessing

- Convert ownership labels:
  - `<= 6 months` and `> 6 months` → `Owned`
  - `Never Owned` → `Non-Owner`
- Handle missing numeric values by filling with `0`
- Encode categorical columns (e.g., `Used it for`, `Model name`)
- Standardize or scale numeric features

---

## 🛠️ Machine Learning Pipeline

1. **EDA**
   - Ownership distribution
   - Review patterns across models and features
2. **Feature Engineering**
   - Categorical encoding
   - Handling missing values
3. **Modeling**
   - Logistic Regression
   - SVC
4. **Evaluation**
   - Accuracy, Precision, Recall, F1-score
   - ROC-AUC

---

## ✅ Output

- Binary classification:
  - `1` → Owner
  - `0` → Non-owner
    
- Best model: 82% Accuracy

---

## 📬 Contact
For questions or contributions, reach out via:

Email: anyanwujustice27@gmail.com


