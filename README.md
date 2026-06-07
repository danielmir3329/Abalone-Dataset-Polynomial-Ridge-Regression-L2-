# Overview

This project uses **Polynomial Ridge Regression** to predict abalone age (Rings) from physical measurements in the Kaggle Abalone Dataset.

Polynomial features allow the model to capture non-linear relationships, while Ridge regularization helps reduce overfitting by shrinking coefficient values.

# Dataset

**Target Variable:** Rings

**Features:**
- Sex
- Length
- Diameter
- Height
- Whole Weight
- Shucked Weight
- Viscera Weight
- Shell Weight

# Feature Engineering

Additional features were created to improve model performance:

- Shell Ratio
- Length-to-Diameter Ratio
- Volume
- Density

These features provide additional biological information related to growth and age.

# Data Preparation

- One-hot encoded categorical variables
- Generated polynomial features
- Applied Ridge regularization
- Split data into training and validation sets (80/20)

# Model

A **Polynomial Ridge Regression** model was developed using:

- Polynomial Features
- Ridge Regression (L2 Regularization)
- Scikit-Learn Pipeline

This approach captures non-linear relationships while controlling model complexity.

# Results

| Model | RMSLE |
|---------|---------|
| Polynomial Ridge Regression | **0.1579** |

The model achieved strong predictive performance and demonstrated the benefit of combining polynomial features with regularization.

# Visualizations

The project includes:

- Actual vs Predicted Values
- Residual Plot
- Feature Importance Analysis
- Polynomial Regression Fit

These visualizations help assess model accuracy and behavior.

# Key Findings

- Non-linear relationships exist within the Abalone dataset.
- Polynomial features improved model flexibility.
- Ridge regularization helped prevent overfitting.
- Engineered biological features contributed to prediction accuracy.

# Technologies

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Jupyter Notebook
