# 🧠 Stroke Prediction for Early Intervention & Patient Stratification

This project applies machine learning to predict stroke risk based on patient health records, helping healthcare providers detect high-risk individuals early and allocate preventive care resources more efficiently.

## 📌 Objectives

- Select and clean meaningful health features from the dataset
- Perform Exploratory Data Analysis (EDA) to understand trends and correlations
- Address class imbalance using ADASYN (Adaptive Synthetic Sampling)
- Train and evaluate multiple classification models: Logistic Regression, Random Forest, XGBoost, and others
- Optimize decision thresholds to prioritize **recall**—minimizing missed stroke cases
- Stratify patients into **low**, **medium**, and **high-risk** categories

## 🛠️ Key Methods

- Feature engineering: creation of risk scores and interaction terms
- Dimensionality reduction via `SelectKBest` using ANOVA F-value
- Model evaluation based on metrics like Accuracy, Recall, F1 Score, and ROC AUC
- Custom threshold tuning with Precision-Recall Curve analysis

## 🔍 Key Findings

- **Logistic Regression** achieved the highest recall (0.83) and AUC (0.85), making it the most suitable for medical screening where catching actual stroke cases is critical.
- Top features across models included **Age**, **Glucose Level**, and **BMI Interactions**.
- The model was able to identify patients at high risk even when they lacked classic symptoms like hypertension—capturing silent risk profiles.

## 💡 Future Work

- Expand feature set with additional metrics (e.g., cholesterol levels, physical activity, medication history)
- Incorporate temporal (time-series) data for better trend detection
- Combine models using ensemble techniques (e.g., stacking or voting) for improved balance between recall and precision
- Deploy the model via an API for integration with hospital systems or mobile health applications


## 👥 Use Case

- Developed for educational use.
