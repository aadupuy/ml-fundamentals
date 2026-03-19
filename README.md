# ML Fundamentals & Model Comparison

This repository documents my study and implementation of core machine learning algorithms, along with a complete end-to-end classification project on the Breast Cancer dataset.

## Final Project: Model Comparison on Breast Cancer Dataset

Main notebook: ML_comparison_project.ipynb

This project compares multiple classification models of increasing complexity:
- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting

### What this project demonstrates

A full ML workflow, including:

1. Data Analysis
- Class distribution
- Feature distributions
- Correlation analysis
- Feature separation between classes

2. Model Training
- Baseline linear model (Logistic Regression)
- Non-linear model (Decision Tree)
- Ensemble methods (Random Forest, Gradient Boosting)

3. Evaluation Strategy
- Train / Validation / Test split (70 / 15 / 15)
- Cross-validation (ROC-AUC)
- ROC curve comparison
- Confusion matrix analysis

4. Metrics used
- Accuracy
- Precision
- Recall
- ROC-AUC

### Key Results

- Logistic Regression performs surprisingly well, showing strong generalization
- Decision Tree overfits heavily (perfect train, worse validation)
- Random Forest achieves the best validation performance
- Gradient Boosting generalizes best on the test set

This highlights an important real-world insight: the model that performs best on validation does not always perform best on unseen data.

### Final Model

Gradient Boosting is selected as the final model because it provides the best balance between:
- Accuracy
- Precision
- Recall

It achieves:
- High overall performance
- Strong generalization
- Better recall for malignant cases (critical in medical applications)

### Key Takeaways

- Model complexity increases risk of overfitting
- Ensemble methods improve robustness
- Validation performance alone is not sufficient for model selection
- Evaluation should prioritize task-specific metrics (e.g. recall in healthcare)

## Other Notebooks

This repository also includes implementations and experiments on:
- Linear Regression
- Logistic Regression
- Decision Trees
- Random Forests
- Gradient Boosting
- Regularization & evaluation techniques

## Tech Stack

- Python
- NumPy / Pandas
- Matplotlib
- Scikit-learn

### About

This project is part of my effort to strengthen my foundations in machine learning, with a focus on understanding:
- Model behavior
- Overfitting vs generalization
- Proper evaluation workflows