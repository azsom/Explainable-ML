
# Introduction to Interpretability in ML - ODSC East, 2023
Machine learning projects are rarely like a kaggle competition. It is thrilling to see your name jump up on the leaderboard which makes competitions exciting and dare I say addictive. However predictive power in real life is much less important than kaggle competitions would have you believe. Often it is just as important to understand why a model makes a certain prediction. The ‘why’ plays an important role during the model development phase as well as after deployment. Complex machine learning pipelines are difficult to debug and issues can go unnoticed. One way to help increase trust in the model during the development stage is to improve its interpretability. Subject matter experts usually can tell which features should be predictive in advance and if your model disagrees with their intuition, that’s a good reason to investigate further and it could point to mistakes in your pipeline. Explanations can be crucial after deployment too because often it is not enough to provide predictions only. If the model has significant impact (e.g., in finance or health care), explanations specific to each data point (e.g., a customer or a patient) are a must.

We will review a couple of methods and tools to calculate global and local explanations in this workshop. Global explanations provide an overview of your model and it answers questions like ‘Which features does my model rely on the most or least in general?’. Local explanations describe how much each feature contributes to the prediction of each data point. Local explanations are important if you need to measure the equity and fairness of your model.

We will start with linear models and we will discuss under what conditions the weights of linear models can be used as explanations. I will introduce the pros and cons of perturbation feature importance which is a model-agnostic approach to calculate global explanations. Some model-specific explanations will also be briefly discussed. And we will close with what I consider to be the state of the art technique to calculate local feature importances: the Shapley Additive Explanations.

We will use python and packages like pandas, numpy, sklearn, XGBoost, and shap.

The slides are in interpretability_in_ML.ipynb, and a pdf version is also provided.

## Prerequistes

Please run test_environment.ipynb. It checks the versions of your python and some packages (like pandas, sklearn, xgboost). If the notebook returns all OK, you should be able to run the presentation without issues. If some FAILs are returned, you need to install/update those packages first.

You can recreate the python environment using the odsc_east_2022.yml conda environment file by running these two commands in the terminal:

`conda env create -n odsc_east_2023 -f odsc_east_2023.yml`

`conda activate odsc_east_2023`

You should be able to run interpretability_in_ML.ipynb now.

## Author

Andras Zsom (andras_zsom@brown.edu)

## License

This project is licensed under the MIT License.
