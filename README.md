# Machine-Learning-Models-
Machine learning code for predicting cyber breach severity using Random Forest, XGBoost, and stacked ensemble models. Includes hyperparameter tuning, log-transformed modeling, model evaluation using MAE, RMSE, and R², and actual-versus-predicted analysis.

Machine Learning Models
This directory contains the Python code used to develop, tune, and evaluate machine learning models for predicting cyber breach severity, measured by the number of records affected.
Objective
The objective of the machine learning analysis is to evaluate whether nonlinear and ensemble-based machine learning methods can improve the prediction of cyber breach severity compared with traditional statistical approaches.
Models
The analysis includes the following machine learning approaches:
Random Forest Regression – an ensemble of decision trees used to model nonlinear relationships between organizational/breach characteristics and records affected.
XGBoost Regression – a gradient-boosted tree model designed to capture nonlinear relationships and interactions between predictors.
Stacked Ensemble – combines predictions from the Random Forest and XGBoost models to evaluate whether combining different modeling approaches improves predictive performance.
Model Development
The dataset was divided into training and testing sets. Model hyperparameters were optimized using randomized and grid search procedures. The models were trained using the training data, while the test set was reserved for evaluating out-of-sample predictive performance.
Because the distribution of records affected is highly right-skewed, models were also evaluated using a logarithmic transformation of the target variable. Predictions were transformed back to the original scale where appropriate for interpretation.
Evaluation
Model performance was evaluated using:
Mean Absolute Error (MAE)
Root Mean Squared Error (RMSE)
R²
Log-scale MAE
Log-scale RMSE
Log-scale R²
Actual-versus-predicted plots and other diagnostic visualizations were also used to assess model performance and identify potential limitations.
Reproducibility
The code in this directory is intended to reproduce the machine learning analysis presented in the thesis. Required Python packages and dependencies are documented in the repository's requirements.txt file.
The analysis uses the processed cyber breach dataset described in the repository's data documentation. The original breach data were sourced from the Privacy Rights Clearinghouse (PRC), with additional company-level characteristics collected through publicly available sources.
