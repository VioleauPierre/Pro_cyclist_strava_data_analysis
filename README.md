# Pro_cyclist_strava_data_analysis

## Project Overview : 
This project aims to develop a machine learning model to predict whether an early breakaway will take the win in a cycling Grand Tour stage. The train data used for this project is taken from the years 2013 to 2022 and the test data from 2023 (waiting for Vuelta result). The project includes data preparation, model selection, cross-validation, and evaluation of different machine learning algorithms.[Vue](https://github.com/vuejs/vue)

## Librairies used
- pandas
- numpy
- scikit-learn
- matplotlib

## Skills : 
- Machine Learning Models: Various machine learning models are explored, including Logistic Regression, SVM, Decision Trees, Random Forest, Naive Bayes, and K-Nearest Neighbors (KNN).
- Model Selection and Evaluation: The project uses cross-validation to select the best-performing model and evaluates the models using accuracy scores and Receiver Operating Characteristic (ROC) curves to measure their predictive performance.
- Hyperparameter Tuning: Hyperparameter tuning is demonstrated using GridSearchCV to optimize the KNN model's performance by finding the best values for hyperparameters.

## Table of Contents

1. [Creation of a Study Data-frame](#creation-of-a-study-data-frame)
-    1.1 [Base of the Data-frame](#base-of-the-data-frame)
-    1.2 [Adding Other Metrics](#adding-other-metrics)
-    1.3 [Creation of a Second Data-frame](#creation-of-a-second-data-frame)
-    1.4 [Determining CP, W', and FTP](#determining-cp-w-and-ftp)
-    1.5 [Adding Intensity Factor, TSS, and Variability Index](#adding-intensity-factor-tss-and-variability-index)
-    1.6 [Adding Power Distribution](#adding-power-distribution)
-    1.7 [Adding PPR and PPR 2000KJ](#adding-ppr-and-ppr-2000kj)
2. [Visualization of the Data](#visualization-of-the-data)
-    2.1 [Overview of the Dataframes](#overview-of-the-dataframes)
-    2.2 [Distance, Duration, and TSS](#distance-duration-and-tss)
-    2.3 [Mean Maximal Power](#mean-maximal-power)
-    2.4 [Year Recap](#year-recap)
-    2.5 [TSS, ATL, CTL, and TSB Evolution](#tss-atl-ctl-and-tsb-evolution)
-    2.6 [Power Distribution](#power-distribution)
-    2.7 [PPR and PPR 2000KJ](#ppr-and-ppr-2000kj)
-    2.8 [Radar Chart of Power](#radar-chart-of-power)

## 1 Creation of a Study Data-frame

Describe the purpose and process of creating the study data-frame.

### 1.1 Base of the Data-frame

Explain the foundational data and metrics included in the base data-frame.

### 1.2 Adding Other Metrics

Describe the process of adding additional metrics to the data-frame.

### 1.3 Creation of a Second Data-frame

Explain the purpose and content of the second data-frame containing daily information.

### 1.4 Determining CP, W', and FTP

Explain the power duration model used to determine CP, W', and FTP.

### 1.5 Adding Intensity Factor, TSS, and Variability Index

Describe the inclusion of Intensity Factor, TSS, and Variability Index in the activity data-frame.

### 1.6 Adding Power Distribution

Explain the process of adding power distribution with a 25W band width.

### 1.7 dding PPR and PPR 2000KJ

Describe how PPR and PPR 2000KJ are calculated and added to each year's data.

## 2. Visualization of the Data

Explain the various visualizations used to represent the data.

### 2.1 Overview of the Dataframes

Describe the visualization that provides an overview of the two dataframes.

### 2.2 Distance, Duration, and TSS

Explain the visualization of Distance, Duration, and TSS.

### 2.3 Mean Maximal Power

Describe the visualization of Mean Maximal Power, both overall and under fatigue.

### 2.4 Year Recap

Explain the visualization summarizing each year's Distance, Duration, and number of activities.

### 2.5 TSS, ATL, CTL, and TSB Evolution

Describe the visualization showcasing the evolution of TSS, ATL, CTL, and TSB.

### 2.6 Power Distribution

Explain the visualization representing the power distribution.

### 2.7 PPR and PPR 2000KJ

Describe the visualization of PPR and PPR 2000KJ.

### 2.8 Radar Chart of Power

Explain the radar chart comparing power to the top 10% value of professional riders.
