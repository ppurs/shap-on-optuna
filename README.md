# **Shap on OPTUNA**

Project developed as part of programming assignment for the *Explainable Artificial Inteligence* course at the Jagiellonian University.

## About
The goal was to run hyperparameter optimization algorithm such as Optuna, collect results from it and use SHAP to try to explain the impact of different hyperparameters on the quality of the optimization process.

### Models and datasets
Two models and datasets were selected for experiments: 
* RandomForestClassifier on Adult dataset
* XGBoostRegressor on California housing dataset 

### Steps
1. Optuna was run on a model and its corresponding dataset. 
2. The results of the optimization process was collected.
3. Three models were chosen for SHAP:
   * RandomForestRegressor
   * XGBoostRegressor
   * MLPRegressor
4. The models were tuned using Optuna.
5. For each model SHAP values were calculated on the results obtained in point 2.
6. SHAP explanations were compared.
   
:bangbang: **Charts from Optuna are not visible in the GitHub preview. To see them, you need to download the *project.ipynb* notebook.**

## Authors
* Rafał Kowalczyk
* Paulina Purs
