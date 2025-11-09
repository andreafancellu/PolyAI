# PolyAI
**PolyAI** explores the use of Machine Learning and Deep Learning for polymer classification and quantitative prediction of recycled material content in blends.

## 🎯 Goals
- **Polymer Classification**. Identify the polymer type based on chemical and structural features. Given the tabular nature of the dataset, containing both numerical and categorical variables, the project adopts a **Random Forest classifier**, an ensemble learning method that constructs multiple decision trees on bootstrapped subsets of the data and combines their outputs through majority voting.
This approach is efficient for small datasets, as it captures non-linear relationships, tolerates noise, and handles heterogeneous features without requiring extensive preprocessing.
To enhance interpretability, feature importance analysis (via SHAP values) will be performed to highlight the chemical and structural features that most strongly influence the classification outcome.  
- **Recycled Content Prediction**: Estimate the percentage of recycled material in a polymer sample using chemical and structural parameters.
For this regression task, PolyAI employs a **Gradient Boosting Regressor** (GBR), an ensemble model that sequentially builds decision trees to minimize the residual errors of previous iterations.
Gradient boosting offers high accuracy for tabular regression problems and can capture complex, non-linear relationships between parameters and recycled content.
Hyperparameter tuning and cross-validation are applied to ensure robustness and generalization despite the limited dataset size.


