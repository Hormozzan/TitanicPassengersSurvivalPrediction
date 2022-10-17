# Titanic Passengers' Survival Prediction
In this notebook, I have done some exploratory data analysis, feature engineering, feature encoding, model evaluation, hyperparameter tuning, and finally, created a supermodel by combining previous models. In the sections below, I am goning to dive into each headline and explain the main ideas behind each.

## Exploratory Data Analysis

To get an intuition about what the samples look like, I started with looking at column names and the first samples in the training data. Also, the `.info()` method helped me figure out what kind of data type each column has and how many samples in each column have non-null values. Also, the `.describe()` method help us extract some statistical properties from numerical columns.
A covenient way of computing something like correlation between the target value ("Survived") and other columns is to calculate it's mean over possible values of other columns. In other words, I grouped the "Survived" column by some other columns and calculated its mean over their possible values. Although this manner is not the exact way of computing correlation (which is done by known methods such as Pearson), it can just give us a sense about which column may have more impact on predicting the target.
