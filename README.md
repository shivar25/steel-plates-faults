# Manufacturing Fault Classification & Process Analysis using Machine Learning
### Project Overview

Manufacturing quality control is crucial for enhancing yield, minimizing defects, and maintaining process stability.
This project focuses on analyzing manufacturing process data and building machine learning models to classify different types of faults in steel plates. The goal is to identify key process parameters associated with specific fault types and provide data-driven insights for process improvement.

The project is designed with a production mindset and a focus on quality improvement, aligning with real-world manufacturing analytics use cases.

### Objectives

Analyze manufacturing process parameters related to steel plate production

Classify different fault types using machine learning models

Compare interpretable and non-linear models for fault classification

Identify key process parameters influencing fault occurrence

Provide actionable insights to support quality improvement and fault diagnosis

### Dataset

### Dataset: Steel Plates Faults Dataset

### Source: Kaggle (originally from UCI Machine Learning Repository)

### Description:

Each row represents a faulty steel plate

Features include geometric, surface, luminosity, and orientation-related process parameters

The target variable represents the type of manufacturing fault

### Tools & Technologies

### Programming Language: Python

### Libraries:

pandas, numpy

matplotlib, seaborn

scikit-learn

### Methodology
### 1. Exploratory Data Analysis (EDA)

Examined data structure, distributions, and class imbalance

Analyzed fault type distribution

Performed group-wise statistical analysis to understand differences across fault categories

### 2. Feature Engineering

Converted multiple fault indicator columns into a single multiclass target variable (Fault_Type)

Selected relevant numeric process parameters as features

### 3. Modeling

### Logistic Regression

Used as an interpretable baseline model

Helped identify linear separability and class overlap

### Random Forest Classifier

Used to capture non-linear interactions between process parameters

Improved classification performance across major fault categories

### 4. Model Evaluation

Classification report (precision, recall, F1-score)

Confusion matrix analysis to study misclassification patterns

Feature importance analysis for interpretability

### Key Insights & Conclusions
### Key Process Insights

Feature importance analysis shows that geometric parameters, surface area characteristics, and orientation-related features play a major role in distinguishing fault types. Parameters such as conveyor length, surface area metrics, and luminosity-based features have a strong influence on fault classification.

### Model Comparison

Logistic Regression provided a strong, interpretable baseline but struggled with overlapping fault classes

Random Forest improved performance by capturing non-linear relationships between process parameters

### Process Improvement Recommendations

Prioritize monitoring of high-impact geometric and surface-related parameters

Stabilize material handling and alignment to reduce fault variability

Use the trained model as a decision-support tool for early fault diagnosis and targeted quality inspections

### Repository Structure
manufacturing-quality-ml/
│
├── data/
│   └── SteelPlatesFaults.csv
├── notebooks/
│   └── manufacturing_quality_analysis.ipynb
└── README.md

### Future Work

Incorporate anomaly detection for early fault warning

Explore model explainability techniques (e.g., SHAP)

Extend analysis to include time-based or batch-level process data

### Author

Shiva Ranjan
M.Sc. Statistics, IIT Kanpur
