# Titanic Survival Prediction - End-to-End ML Project
##  Project Objective
The objective of this project is to build a binary classification Machine Learning model that predicts passenger survival on the Titanic based on socio-demographic and travel features such as Age, Gender, Ticket Class, and Fare.
##  Dataset Source
- **Dataset:** Kaggle Titanic - Machine Learning from Disaster
- **Target Variable:** `Survived` (0 = No, 1 = Yes)
## 🛠️ Methodology & Workflow
1. **Data Preprocessing & Cleaning:**
   - Handled missing values (`Age` imputed using median, `Embarked` using mode).
   - Removed non-predictive attributes (`Cabin`, `PassengerId`, `Name`, `Ticket`).
   - Handled outliers in `Fare` by capping extreme values at the 99th percentile.
   - Encoded categorical variables (`Sex`, `Embarked`) using One-Hot Encoding.
2. **Exploratory Data Analysis (EDA):** Visualized age distributions, survival rate by passenger class, and gender-based survival rates using Seaborn and Matplotlib.
3. **Model Training & Tuning:**
   - Trained **Logistic Regression** and **Random Forest Classifier** models.
   - Fine-tuned Random Forest hyperparameters using `GridSearchCV`.
4. **Model Evaluation:** Evaluated performance using Accuracy, Precision, Recall, F1-Score, and ROC-AUC metrics.
##  Model Performance Comparison

| Metric | Logistic Regression | Random Forest (Tuned) |
| :--- | :--- | :--- |
| **Accuracy** | 81.01% | **82.68%** |
| **Precision** | 78.57% | **81.16%** |
| **Recall** | 74.32% | **75.68%** |
| **F1-Score** | 76.39% | **78.32%** |
| **ROC-AUC** | 0.798 | **0.814** |

##  Key Actionable Insights
- **Gender Priority:** Female passengers had a significantly higher survival rate (~74%) compared to males (~19%).
- **Socio-Economic Status:** 1st Class passengers had the highest survival rate, indicating priority access to lifeboats.
- **Best Model:** The **Tuned Random Forest Classifier** outperformed Logistic Regression across all metrics and is selected for final deployment.
## 🚀 How to Run locally
1. Clone the repository:
   ```bash
   git clone <your-repository-link>
