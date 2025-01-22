# **Shap on OPTUNA**

Project developed as part of a programming assignment for the *Explainable Artificial Intelligence* course at the Jagiellonian University.

## About
The goal was to run hyperparameter optimization algorithm such as Optuna, collect results from it and use SHAP to try to explain the impact of different hyperparameters on the quality of the optimization process. Then, as a project extension, to use a rule-based explainer for the instance with the best score.
Additionally, we trained the DecisionTreeRegressor to get another explanation for this instance and the optimization process.

### Models and datasets
Two models and datasets were selected for experiments: 
* RandomForestClassifier on Adult dataset
* XGBoostRegressor on California housing dataset

As the rule-based explainers, LORE and LUX were chosen. 

### Steps
1. Optuna was run on a model and its corresponding dataset. 
2. The results of the optimization process was collected.
3. The DecisionTreeRegressor was trained on the results from point 2 and explanation for given instance was obtained.
4. Three models were chosen for SHAP:
   * RandomForestRegressor
   * XGBoostRegressor
   * MLPRegressor
5. The models were tuned using Optuna.
6. For each model SHAP values were calculated on the results obtained in point 2.
7. SHAP explanations were compared.
8. LORE was run on the results from point 2, explanation and counterfactual explanations for given instance were obtained.
9. As above, LUX was run on the results obtained in point 2.   
   
:bangbang: **Charts from Optuna are not visible in the GitHub preview. To see them, you need to download the *project.ipynb* notebook.**

## Authors
* Rafał Kowalczyk
* Paulina Purs
