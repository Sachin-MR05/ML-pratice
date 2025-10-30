# Machine Learning Development Life Cycle

## Table of Contents

- [Problem Framing](#problem-framing)
- [Gathering Data](#gathering-data)
- [Data Preprocessing](#data-preprocessing)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Feature Engineering](#feature-engineering)
- [Model Training, Evaluation, and Selection](#model-training-evaluation-and-selection)
- [Model Deployment](#model-deployment)
- [Testing](#testing)
- [Optimization](#optimization)

## Problem Framing
The problem framing is the first and the most important part in the MLDLC process. Because after we start cooking, we can't change the dish halfway. So we want to analyze it beforehand, like what you want to solve, who is your customer, how much will it cost, how many people I need in my team, what model we want to choose, where can we get the data.

## Gathering Data
1. **CSV** - Downloading the data from the external source as a CSV format directly.
2. **API** - Calling the APIs using Python code and generating a CSV and using it.
3. **Web Scraping** - Web scraping with Python from any website, example: getting the price of all products from Amazon.

The models can't access the database directly, so we make it into a data warehouse with Extract, Transform, Load (ETL), then we fetch the data from the data warehouse.

Spark, cluster form of data storing.

## Data Preprocessing
After data gathering, we can't use the data directly to train the model because the data is unclean, unstructured, with outliers, so we want to preprocess the data.

## Exploratory Data Analysis
Analyzing the data to find the relationship between them by:
1. Visualizing.
2. Univariate (finding the mean, median, etc., for single column) / Bivariate (finding the mean, median, etc., for two columns) / Multivariate (finding the mean, median, etc., for multi columns).
3. Outlier detection.
4. Checking the imbalance in the data.

## Feature Engineering
- Finding which columns are wanted and which columns are unwanted.
- Finding how much time it takes for each feature to train the model and how to reduce it.
- How to combine two or more columns and make the model more accurate.

## Model Training, Evaluation, and Selection
- Finding the best algorithm for our data. No one knows which algorithm is best for the data gathered. We use all the different algorithms to find the best algorithm.
- Evaluating the model's performance with different metrics and finding the best models.
- Ensemble multiple models to find the best result.

## Model Deployment
For model deployment, we convert the model into a binary file (pickle) and convert it into an API by storing it on the server (Heroku, AWS, GCP).

## Testing
Testing with fewer people and getting feedback and updating the model.

## Optimization
- Load balancing
- Retraining on server
- Routing
    



    


    