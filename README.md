ValueInvestor_Stock Price Prediction
==============================

This is a stock price prediction system for portfolio companies trading data from emerging markets. 
This repository aims to establish a robust intelligence that met the goal of  predicting stock price valuations on a daily, weekly, and monthly basis and recommending BUY, HOLD, and SELL decisions. Here is my methodology:

* Read and explore the data
* Visualized data with multi plots techniques
* Preprocessed the data
* Used 4 different models for the modeling part:
    * 1 additive regression model (Prophet by Facebook)
    * 2 statistical models(ARIMA/ARIMAX and SARIMAX)
    * 1 deep learning model (LSTM).
* Compared forecasting results
* Used Bollinger Bands technique to visualize my forecasting prices
* Made recommendations to either Buy, Sell, or Hold.

After comparison, the multivariate Prophet and SARIMAX model had the best performance in terms of accuracy, MAE, and MAPE. The Multivariate Prophet was the selected model with an MAE of 1.41 and MAPE Mean Absolute Percentage Error of around 0.005, the model is 99.9% accurate. Further evaluation was using the Bollinger Bands.

![image](https://github.com/dorcas-1404/LakMvbp96Bil1P0R/assets/73675830/8553b5ab-50d2-4f99-acee-3f4e42e719ed)


Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
