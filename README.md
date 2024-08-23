# ML Olympiad - Sustainable Urban Living 🏡

## Overview

Finding a suitable place to live is a crucial decision that significantly impacts your well-being. While online listings provide information, it can be challenging to assess a property's true "habitability" based solely on descriptions. This is where AI can lend a helping hand!

This project was part of the Kaggle competition, **ML Olympiad - Sustainable Urban Living**, where I developed a machine learning model to predict the habitability score of a property based on available details. The goal was to create a user-friendly system that empowers individuals to make informed decisions about their living spaces.

**Competition Result:** 🥉 3rd Place  
**Goal:** Develop an ML model that predicts the Sustainable Habitability Score of a property based on the provided data.

## Key Approaches

In the pursuit of the best model for predicting habitability scores, several approaches were explored. Below are the main strategies and techniques used:

1. **Utilization of Cross-Validation Strategy:**

   - Employed rigorous cross-validation to evaluate various algorithms, including RandomForest Regressor, XGB Regressor, LGBM Regressor, MLP Regressor (Neural Network), DecisionTree Regressor, Lasso, GradientBoosting Regressor, and Linear Regression.

2. **Training with RandomForest Regressor:**

   - Focused on optimizing the performance of the RandomForest Regressor by fine-tuning hyperparameters.

3. **Training with XGB Regressor:**

   - Similar optimization efforts were made with XGB Regressor to enhance model accuracy.

4. **Ensemble Methods (Stacked Regressor):**
   - **Method 1:** Combined RandomForest Regressor and XGB Regressor.
   - **Method 2:** Expanded the ensemble to include LGBM Regressor and MLP Regressor (Neural Network), in addition to RandomForest and XGB Regressors.

## Results Comparison

The models were evaluated based on Root Mean Square Error (RMSE), Mean Absolute Error (MAE), Mean Squared Error (MSE), and R² Score across various datasets (training, validation, and test sets). The ensemble method in **Approach 4 - Method 2** emerged as the top performer:

| Approach              | RMSE     | MAE      | MSE       | R² Score  | Competition Score |
| --------------------- | -------- | -------- | --------- | --------- | ----------------- |
| Approach 2            | 5.68     | 4.40     | 32.28     | 0.839     | 5.96980           |
| Approach 3            | 5.72     | 4.44     | 32.68     | 0.837     | 5.98977           |
| Approach 4 (Method 1) | 5.68     | 4.40     | 32.21     | 0.839     | 5.94858           |
| Approach 4 (Method 2) | **5.55** | **4.33** | **30.85** | **0.846** | **5.67223**       |

## Discussion

Overall, the ensemble methods, particularly **Approach 4 - Method 2**, provided the highest predictive accuracy, consistently outperforming other approaches. This suggests that ensemble learning can significantly enhance model performance in predicting habitability scores.

## Repository Contents

- **Report:** [Link to the report](./Report.pdf)
- **Jupyter Notebooks:** [Link to notebooks](./notebooks)
- **Data:** [Link to data](./data)

## Conclusion

This project demonstrated the effectiveness of ensemble methods in predicting sustainable habitability scores. The approaches and insights gained from this competition can be applied to similar predictive modeling tasks in real-world scenarios.
