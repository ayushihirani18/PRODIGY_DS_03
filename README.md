# Task 3: Data Analysis and Decision Tree Model

## Overview
This repository contains the implementation and analysis of a Decision Tree model applied to the **bank dataset**. The objective was to predict customer responses based on various demographic and transactional features.

## Dataset
The dataset consists of 17 columns and 4521 rows, representing customer data, including:
- **Demographics**: Age, Job, Marital Status, Education
- **Financial Information**: Balance, Loan Status, Housing Loan
- **Contact Details**: Day, Month, Duration of the last contact
- **Outcome**: Whether the customer subscribed to a term deposit

## Key Steps

### 1. Data Preprocessing
- Loaded and inspected the dataset for null values and duplicates.
- Encoded categorical variables using `LabelEncoder`.
- Performed exploratory data analysis to understand data distributions and correlations.

### 2. Exploratory Data Analysis
- Visualized the age distribution, marital status, and job roles with respect to subscription outcomes.
- Generated a correlation heatmap to identify significant feature relationships.

### 3. Model Building
- Splitted the dataset into training and testing sets (80:20 split).
- Built a Decision Tree Classifier using `sklearn` with the following parameters:
  - Criterion: Gini
  - Max Depth: 5
  - Random State: 42

### 4. Model Evaluation
- Achieved an accuracy of **89.83%** on the test set.
- Generated a classification report with precision, recall, and F1-score.
- Visualized the decision tree structure for better interpretability.

### Confusion Matrix
| Predicted | No   | Yes  |
|-----------|------|------|
| **No**    | 781  | 26   |
| **Yes**   | 66   | 32   |

### Metrics
- **Precision**: 74%
- **Recall**: 65%
- **Weighted Average F1-score**: 89%

## Visualizations
- **Age Distribution**:
  Histogram showing the frequency distribution of customer ages.
- **Marital Status vs Deposits**:
  Count plot segmented by subscription outcome.
- **Decision Tree Visualization**:
  A graphical representation of the decision-making process.
  
## Dependencies
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`

## Future Work
- Optimize hyperparameters for better precision and recall.
- Experiment with other classification models like Random Forest and XGBoost.
- Analyze additional features for deeper insights.

## Results
The model provides a strong foundation for customer prediction analysis, aiding in better targeting and decision-making processes. Let's continue refining and exploring! 🚀

---

Feel free to contribute or provide suggestions. Let’s collaborate to make this project even better! ✨

#MachineLearning #DataScience #DecisionTrees
