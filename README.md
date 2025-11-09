# PolyAI
Polymers are large molecular structures composed of repeating subunits (monomers) that form the basis of most plastics and rubbers, each type exhibiting distinct chemical, structural, and mechanical properties.
By applying data-driven Machine Learning techniques, PolyAI seeks to automatically identify polymer types and estimate the percentage of recycled material in polymer blends, supporting the development of more sustainable recycling processes.

## 🎯 Goals
- **Polymer Classification**. Identify the polymer type based on chemical and structural features. Given the tabular nature of the dataset, containing both numerical and categorical variables, the project adopts a **Random Forest classifier**, an ensemble learning method that constructs multiple decision trees on bootstrapped subsets of the data and combines their outputs through majority voting.
This approach is efficient for small datasets, as it captures non-linear relationships, tolerates noise, and handles heterogeneous features without requiring extensive preprocessing.
To enhance interpretability, feature importance analysis (via SHAP values) will be performed to highlight the chemical and structural features that most strongly influence the classification outcome.  
- **Recycled Content Prediction**: Estimate the percentage of recycled material in a polymer sample using chemical and structural parameters.
For this regression task, PolyAI employs a **Gradient Boosting Regressor** (GBR), an ensemble model that sequentially builds decision trees to minimize the residual errors of previous iterations.
Gradient boosting offers high accuracy for tabular regression problems and can capture complex, non-linear relationships between parameters and recycled content.
Hyperparameter tuning and cross-validation are applied to ensure robustness and generalization despite the limited dataset size.


<img width="1231" height="1299" alt="image" src="https://github.com/user-attachments/assets/2c73e490-88bb-4b65-8d8d-35962f4d7c47" />
