# MSME Success Prediction and Risk Scoring

A machine learning project for predicting Micro, Small, and Medium Enterprise (MSME) success, identifying key business success factors, assessing business risk, and simulating policy interventions to support data-driven MSME development.

## Overview

Micro, Small, and Medium Enterprises (MSMEs) play an important role in economic growth and employment. However, their success is influenced by various factors, including financial management, business planning, access to capital, industry experience, and digital technology adoption.

This project develops a machine learning-based classification system to predict MSME success. The system also incorporates model interpretation, risk scoring, and policy simulation to generate insights that can support more targeted MSME development programs.

## Objectives

- Analyze the characteristics of successful and unsuccessful MSMEs.
- Compare machine learning models for predicting MSME success.
- Identify important success factors using Feature Importance and SHAP.
- Develop a risk scoring system based on predicted success probabilities.
- Simulate policy interventions to evaluate their potential impact on MSME success.

## Methodology

The project follows these main steps:

1. **Data Preprocessing** — Handle missing values and duplicate records, prepare variables, and standardize numerical features where appropriate.
2. **Exploratory Data Analysis (EDA)** — Examine variable distributions, success rates, and relationships between business characteristics and MSME success.
3. **Model Development** — Train and compare classification algorithms.
4. **Model Evaluation** — Evaluate model performance using Accuracy, Precision, Recall, F1-Score, ROC-AUC, and cross-validation.
5. **Model Interpretation** — Use Feature Importance and SHAP to identify the variables that contribute most to predictions.
6. **Risk Scoring** — Categorize MSMEs according to their predicted probability of success.
7. **Policy Simulation** — Evaluate hypothetical interventions by modifying selected business characteristics and observing changes in predicted success rates.

## Machine Learning Models

The study considers the following classification algorithms:

- Logistic Regression
- AdaBoost
- XGBoost
- CatBoost

The model comparison results reported in the analysis also include LightGBM. AdaBoost was selected as the best-performing model in the reported evaluation.

## Dataset

The dataset contains 13 variables: 12 predictor variables and one target variable, `Success`.

The predictors cover several aspects of MSME characteristics:

- **Demographic:** Age, Education, and Owner Gender.
- **Financial and Business Resources:** Initial Capital and Financial Record Keeping.
- **Digital Adoption:** Internet Usage.
- **Business Planning and Strategy:** Business Plan, Marketing Effort, and Partnership.
- **Experience and Professional Support:** Industry Experience, Parent Business Experience, and Professional Advice.

The target variable is defined as follows:

| Value | Meaning |
|---|---|
| 1 | Successful MSME |
| 0 | Unsuccessful MSME |

## Model Interpretation

Two interpretation techniques are used:

- **Feature Importance:** Identifies variables with high relative importance in the model's predictions.
- **SHAP (SHapley Additive exPlanations):** Explains how individual features contribute to predictions at both the overall dataset level and the individual MSME level.

These techniques help translate model outputs into more actionable insights for MSME development.

## Risk Scoring

The predicted probabilities are used to classify MSMEs into risk categories. This process can help policymakers and business support organizations identify enterprises that may require additional assistance and prioritize interventions according to their needs.

## Policy Simulation

Four hypothetical policy scenarios are evaluated:

1. **Business Incubation** — Improve business planning and financial record-keeping practices.
2. **Digital Transformation** — Increase internet adoption among MSMEs.
3. **Capital Assistance** — Improve the adequacy of initial business capital.
4. **Integrated MSME Development** — Combine multiple interventions to support business development.

The simulations compare predicted success rates under different intervention coverage levels. Their results represent model-based scenarios rather than guaranteed outcomes of real-world policy implementation.

## Key Findings

According to the reported model evaluation:

- AdaBoost achieved an accuracy of **96%**.
- AdaBoost achieved a precision, recall, and F1-score of **91.7%** each.
- AdaBoost achieved a ROC-AUC of **98.5%**.
- Its mean F1-score across 10-fold cross-validation was **94.8%**.

The analysis also highlights the importance of business planning, industry experience, internet usage, and financial management in understanding MSME success.

## Tools and Technologies

The project applies machine learning, exploratory data analysis, model evaluation, and model interpretation techniques. Specific programming languages, libraries, and environment requirements should be documented according to the implementation used in the repository.

## Limitations

The findings depend on the available dataset, the target definition, and the assumptions used in the policy simulations. Simulated changes in predicted success probabilities should not be interpreted as causal effects or guarantees of actual policy outcomes.

## Authors

- Danella Citra Aldarena
- Maria Immaculata Dyah Hita Widowati
- Ike Maya Setya

Faculty of Science and Data Analytics  
Institut Teknologi Sepuluh Nopember (ITS)

