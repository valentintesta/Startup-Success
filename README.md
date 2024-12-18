# Startup-Success-Prediction

# Introduction

A startup or start-up is a company or project begun by an entrepreneur to seek, develop, and
validate a scalable economic model. While entrepreneurship refers to all new businesses,
including self-employment and businesses that never intend to become registered, startups
refer to new businesses that intend to grow large beyond the solo founder. Startups face high
uncertainty and have high rates of failure, but a minority of them do go on to be successful
and influential. Some startups become unicorns: privately held startup companies valued at
over US$1 billion.
Startups play a major role in economic growth. They bring new ideas, spur innovation, create
employment thereby moving the economy. There has been an exponential growth in startups
over the past few years. Predicting the success of a startup allows investors to find companies
that have the potential for rapid growth, thereby allowing them to be one step ahead of the
competition.

# Objective

The objective is to predict whether a startup which is currently operating turns into a success
or a failure. The success of a company is defined as the event that gives the company's
founders a large sum of money through the process of M&A (Merger and Acquisition) or an
IPO (Initial Public Offering). A company would be considered as failed if it had to be shut
down.

# About the Data

The data contains industry trends, investment insights and individual company information.
There are 48 columns/features. Some of the features are:
● age_first_funding_year – quantitative
● age_last_funding_year – quantitative
● relationships – quantitative
● funding_rounds – quantitative
● funding_total_usd – quantitative
● milestones – quantitative
● age_first_milestone_year – quantitative
● age_last_milestone_year – quantitative
● state – categorical
● industry_type – categorical
● has_VC – categorical
● has_angel – categorical
● has_roundA – categorical
● has_roundB – categorical
● has_roundC – categorical
● has_roundD – categorical
● avg_participants – quantitative
● is_top500 – categorical
● status(acquired/closed) – categorical (the target variable, if a startup is ‘acquired’ by
some other organisation, means the startup succeed)

# Methodology:

## 1. Data Preprocessing:

**Data Collection:** Initially, a dataset of different startups across the USA was
collected. This dataset likely includes various attributes about each startup,
such as funding history, location, industry, and other relevant information.

**Data Cleaning:** The collected data might contain noise, missing values, or
outliers. Data cleaning involves handling missing values by either imputing
them or removing rows with missing data. Outliers might be treated or
retained based on the specific characteristics of the data.

**Feature Engineering:** This step involves creating new features or transforming
existing ones to better represent the information in the dataset. For example,
you might create new features like the age of the startup, total funding raised,
or location-based features.

**Data Encoding:** Categorical variables, such as industry type or location, need
to be encoded into a numerical format for machine learning algorithms to
work. Common techniques include one-hot encoding or label encoding.

**Data Splitting:** The dataset is typically divided into training and testing sets.
The training set is used to train the machine learning models, while the testing
set is used to evaluate their performance.

## 2. Machine Learning Models:

**Decision Tree:** A Decision Tree is a tree-like model that makes decisions
based on a series of rules learned from the data. It is a straightforward and
interpretable model that can handle both categorical and numerical data.
Decision Trees are prone to overfitting, which means they can perform very
well on the training data but poorly on unseen data.
**Random Forest:** Random Forest is an ensemble learning method that builds
multiple Decision Trees and combines their predictions. It reduces overfitting
compared to a single Decision Tree and generally provides more robust
predictions. Random Forest can handle a large number of features and is less
sensitive to hyperparameter tuning.

## 3. Frontend Development:

● To provide a user-friendly interface for making predictions, we created a
simple frontend using the Gradio library in Python.
● The frontend allowed users to input startup information and receive
predictions based on the trained machine learning models.


# Algorithms Used:

In this project, two popular machine learning algorithms were employed:

**Decision Tree:** A Decision Tree is a tree-like model that makes
decisions based on a series of rules learned from the data. It is a
straightforward andinterpretable model that can handle both categorical
and numerical data. Decision Trees are prone to overfitting, which means
they can perform verywell on the training data but poorly on unseen data.

**Random Forest:** Random Forest is an ensemble learning method that
builds multiple Decision Trees and combines their predictions. It reduces
overfittingcompared to a single Decision Tree and generally provides more
robust predictions. Random Forest can handle a large number of features and
is less sensitive to hyperparameter tuning
