
# Practical Explainability Techniques for Machine Learning Models - ODSC East, 2025
This workshop focuses on practical techniques for improving the explainability of machine learning models, emphasizing the importance of understanding why a model makes certain predictions, both during development and after deployment. We will explore methods for calculating global explanations (which show general feature importance) and local explanations (which assess the contribution of each feature to individual predictions). The session will cover linear models, perturbation-based feature importance, and Shapley Additive Explanations (SHAP) for local feature importances. Participants will learn how to implement these techniques using Python and popular libraries like pandas, sklearn, XGBoost, and SHAP to increase model interpretability, fairness, and trust.

## Prerequistes

Please run test_environment.ipynb. It checks the versions of your python and some packages (like pandas, sklearn, xgboost). If the notebook returns all OK, you should be able to run the presentation without issues. If some FAILs are returned, you need to install/update those packages first.

You can recreate the python environment using the odsc_east_2022.yml conda environment file by running these two commands in the terminal:

`conda env create -n odsc_east_2025 -f odsc_east_2025.yml`

`conda activate odsc_east_2025`

You should be able to run the notebook now.

## Author

Andras Zsom (andras_zsom@brown.edu)

## License

This project is licensed under the MIT License.
