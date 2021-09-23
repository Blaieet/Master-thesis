_**Note**: this is the public repository of the project, which does not contain the XGBoost implementation._ 

# Accuracy comparison between Sparse Autoregressive and XGBoost models for high-dimensional product sales forecasting #

This is my thesis of the Master in Fundamentals Principles of Data Science from Universitat de Barcelona, with the collaboration of Accenture's applied intelligence department and the supervision of Jordi Vitrià, PhD.

### Brief introduction ###

Sales forecasting is the process of estimating future revenue for resource allocation, budgeting or simply to perform informed business decisions. When predicting a product's sales we use its past data in order to train our algorithms. Yet, there are lots of external factors that affect a product's revenue: sales of another similar product  cannibalization), applied promotions (like discounts) or even the weather of that week-sales. 

Our work consists of evaluating how much do these inter-product relationships affect a forecast accuracy. Using popular machine learning and data science tools, we designed a framework that enables the building, training and evaluation of two models and its comparison through a detailed set of forecast metrics. 

Given today's data abundance, companies face another issue when performing these predictions: the big dimensionality of their datasets of sales records, known has endogenous variables, and discounts, marketing campaigns or advertising results, known as exogenous variables.

Therefore, we trained the following models:

* **Sparse Vector Autoregressive model (VAR)**: specialized on modeling these possible product associations. Modified for the input of high-dimensional datasets.

* **XGBoost**: a widely, versatile and flexible used tool among Kaggle competitors that overperformed in the past few years any other kind of machine learning algorithm on large-scale regression, classification or ranking problems. Nonetheless, is not specialized on detecting these product relationships.

Given a huge dataset of ore than 2600 product (divided in segments) sales from a home improvement, gardening, and workshop retailer, alongside discount and duration promotion variables, through a two-year or more date span, we forecasted one-month ahead sales. Then, we tested both models using time series evaluation metrics in order to assess which model is better and how good were our predictions. 

As a conclusion, we found that the Vector Autoregressive model is more accurate than the XGBoost model, showing
that relationships between products affect a forecast performance.

### Structure

* [Master Thesis report](https://bitbucket.org/blaiot/master_thesis_blai_ras/src/master/Master%20Thesis%20Report.pdf)
* [Original dataset](https://bitbucket.org/blaiot/master_thesis_blai_ras/src/master/Data/)
* [XGBoost model building & training (property of Accenture)](https://bitbucket.org/blaiot/master_thesis_blai_ras/src/master/XGBoost/TFM%20Blai/TFM%20Blai.Rproj)
* [Trained models](https://bitbucket.org/blaiot/master_thesis_blai_ras/src/master/Models/Processed/)
* [VAR model results](https://bitbucket.org/blaiot/master_thesis_blai_ras/src/master/VAR%20Results/)
* [XGBoost model results](https://bitbucket.org/blaiot/master_thesis_blai_ras/src/master/XGBoost/TFM%20Blai/Evaluation%20Results/)

#### Notebooks

* [Data cleaning and pre-processing](https://bitbucket.org/blaiot/master_thesis_blai_ras/src/master/01.%20Preprocess.ipynb)
* [Training and Evaluation of the VAR model](https://bitbucket.org/blaiot/master_thesis_blai_ras/src/master/02.%20Training%20%26%20Evaluation%20(VAR).ipynb)
* [XGBoost evaluation](https://bitbucket.org/blaiot/master_thesis_blai_ras/src/master/XGBoost/TFM%20Blai/Evaluation%20Results/)

### Contact

You can contact me for any kind of questions, discussions or comments about my work at:

* [Email](mailto:blai.ras.jim@gmail.com)

* [LinkedIn](https://www.linkedin.com/in/blai-ras-590381192/)

* [Instagram](https://www.instagram.com/blaiot/)

### Citation

```

@misc{VARComparisonBRJ,
title={Accuracy comparison between Sparse Autoregressive and XGBoost models for high-dimensional product sales forecasting},
url={https://bitbucket.org/blaiot/master_thesis_blai_ras/src/master/Master%20Thesis%20Report.pdf},
note={Master Thesis paper},
author={Blai Ras},
  year={2021}
}

```