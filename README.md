# wine-alcohol-prediction
Machine Learning regression project for predicting alcohol content in wine

Video Link: https://drive.google.com/file/d/1Faudj2jolFwFkLz3fLOpX67NmzzGxa6a/view?usp=drive_link

Abstract
The quality and composition of red wine are influenced by its physicochemical properties. This project aims to predict alcohol content in red wines using the UCI Wine Quality dataset. Multiple regression models were implemented, including Linear Regression, Ridge, Lasso, Random Forest, and Gradient Boosting. A preprocessing pipeline handled missing values, scaled numeric features, and encoded categorical features. Random Forest regression achieved the highest R^2 score on cross-validation and performed best on unseen test data. Feature importance analysis revealed density, volatile acidity, and sulphates as the most influential predictors. Residual and prediction error analysis confirmed the model’s robustness. The trained pipeline was saved for future use on new wine samples.

Introduction
Red wine contains numerous chemical and physical components that jointly influence its properties, including alcohol content, pH, density, and acidity. Accurate prediction of alcohol content is important for quality control and industrial processing. This project uses the UCI red wine dataset to model alcohol content as a function of physicochemical features. Preprocessing pipelines ensure robust handling of numeric and categorical data. The goal is to identify the most effective regression model and interpret the contribution of individual wine features.

Literature Review
Di & Yang (2022) applied a 1D-Convolutional Neural Network (1D-CNN) to capture correlations among physicochemical features. Their model outperformed baseline methods, such as SVM and Random Forest, in predicting wine quality by incorporating dropout and batch normalization.
Amrutha (2023) evaluated Linear Regression, SVR, and Random Forest. Random Forest achieved the highest R^2 and lowest error, highlighting its suitability for regression tasks with correlated features.
Jain et al. (2023) compared Random Forest and XGBoost for wine quality prediction. Tree-based models consistently outperformed linear and shallow models, confirming their robustness and interpretability.
These studies indicate that both deep learning and tree-based ensemble models are effective for wine prediction tasks. This project focuses on Random Forest regression for its accuracy, interpretability, and suitability for numerical feature prediction.

Methodology
Data Loading and Preprocessing
Dataset: UCI Wine Quality – red wine data
Target Variable: alcohol
Features: 11 physicochemical attributes (numeric); no ID or irrelevant columns
Preprocessing:
Numeric features: mean imputation + standard scaling

Model Setup
Baseline Models Tested: Linear Regression, Ridge, Lasso, Random Forest, Gradient Boosting
Final Model: Random Forest Regressor (100 estimators, random_state=123)

Conclusion
The project demonstrates that Random Forest regression is highly effective for predicting alcohol content in red wines. Proper preprocessing, feature selection, and evaluation ensure robust model performance.

References
Di, S., & Yang, Y. (2022). Prediction of Red Wine Quality Using One-Dimensional Convolutional Neural Networks. University of New South Wales & University of Technology Sydney.
Amrutha. (2023). Red Wine Alcohol Prediction Using Machine Learning Models.
Jain, K., Kaushik, K., Gupta, S. K., Mahajan, S., & Kadry, S. (2023). Machine learning-based predictive modelling for the enhancement of wine quality. Scientific Reports, 13, 17042. https://doi.org/10.1038/s41598-023-44054-3

