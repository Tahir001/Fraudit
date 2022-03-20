# Fraudit
The following repo utilizes a companies data to determine if it's investment request is fraudulent or not.
Please note, the data itself is from a large bank in Canada and cannot be shared (even though it's been censored to not reveal the identity of the companies). 

## Data
There are two datasets: 
- Candian Companies Dataset - About 30k rows of canadian companies asking for Loans / Investments over the span of 3 years. 
- General Companies Dataset - About 28k rows of companies (outside of Canada) asking for loans / investments over the span of last 3 years. 

## Repository Structure
In this repo, we breakdown our End to End modelling pipeline and use a seperate Notebook for each process.

The Pictures Folder contains all of the screenshots we used in our presentation, and some of our visualization output.

The Automatic_Analysis folder contains the result from Pandas Profiling (Automatic EDA library)

The Code Folder contains our process which is entailed as follows: 
1. Exploratory Data Analysis
2. Data Cleaning and Pre-Processing 
3. Solving the class imbalance issue
4. Feature Engineering and Feature Selection
5. Modelling & Hyperparameter Optimization
6. Model Explaination
7. Results & Final Submission

# Table of Contents:
1. [Initial Set-Up & Import Data](#1)
2. [Exploratory Data Analysis](#2) 
    1. [Dataset, Datatypes, Missing Data, Duplicates, Graphs](#2.1)
    2. [Data Cleaning Methods](#2.2)
        1. [Data Prep -- Column Types, Date Manipulations, Removing outliers](#2.2.1)
        2. [Missing Values - Simple Imputer (Mean, Median, Random Imputation, Average Growth)](#2.2.2)
        3. [Missing Values - Three Year Average](#2.2.3)
        4. [Missing Values - Complex Imputer (Deterministic, Stochastic Regression, KNN)](#2.2.4)
    2. [Further Analysis (Barplots, Scatterplots, CustomerID, Classes, Clustering)](#2.2)
    3. [Data Distributions by Features & Investment Type](#2.3)
<br>
4. [Feature Engineering & Feature Selection](#4)
    1. [Creating Additional Financial Features](#4.1)
    2. [Correlation & Co-variance - Pearsons, Spearmans](#4.2)
    3. [Subset Selection - Forward, Backwards, Best](#4.3) 
    4. [Feature Importance - Linear & Non-Linear Classifer (Lasso & Random Forest)](#4.4)
    5. [RFE](4.5)
    6. [Principal Component Analysis](#4.6)
    7. [Autoencoders](#4.7)
    8. [QUBO](#4.8)
<br>
5. [Data Pre-processing](#5)
    1. [Standardization & Normalization](#5.1)
    2. [Class Imbalance Issue - Oversampling, Undersampling, SMOTE & ASIDANYA](5.2)
    3. [Synthetic Data Generation - Generative Adversial Networks (GANs)](5.3)
<br>

6. [Defining Metrics & Baseline Models ](#6)
    1. [Model Metrics(Confusion Matrix, Custom Loss function, Log loss)](6.1)
    2. [Linear Baseline Model](6.2)
    3. [Non-Linear Baseline Model](6.3)
<br>

6. [Model Training & Evaluation](#6)
    1. [Hyperparameter Optimization](6.1)
7. [Final Model & Results for Task 1](#7)
8. [Task 2 -- Solution Implementation](#8)
9. [Final Model & Results for Task 2](#9)
10. [Task 3 -- Solution Implementation (customized NNs)](#10)
11. [Final Model & Results for Task 2](#11)

## Presentation Slides
A Rough Draft of the presentation slides can be found here: https://docs.google.com/presentation/d/1TSxYwJy-8RPQgrMXTs8Cb-ag7hUpsb4q29BoZ7dX5Z4/edit?usp=sharing
