# Pro_cyclist_strava_data_analysis

## Project Overview : 
This project aims to learn and practice new skills by analyzing several years of data from a professional cyclist. The data used for this project was retrieved using [Scrap_public_strava_data](https://github.com/VioleauPierre/Scrap_public_strava_data).

## Librairies used
- pandas
- numpy
- statistics
- datetime
- sweat
- scipy
- matplotlib
- seaborn
- plotly

## Skills : 
- Data Analysis: Understanding how to load, manipulate, and analyze data using libraries like pandas and numpy.
- Data Visualization: Creating various types of visualizations to represent data trends and patterns using matplotlib, seaborn, and Plotly.
- Statistical Analysis: Utilizing statistical functions and methods to extract meaningful insights from the data.
- Time Series Analysis: Handling and analyzing time-based data to uncover temporal trends and variations.
- Optimization Techniques: Implementing optimization algorithms (e.g., least_squares and curve_fit) for curve fitting and other data-related optimizations.
- Cycling and sports performance metrics : CP (Critical Power), W', FTP (Functional Threshold Power), TSS (Training Stress Score), and more.

## Table of Contents

1. [Creation of a Study Data-frame](#1-creation-of-a-study-data-frame)
-    1.1 [Base of the Data-frame](#11-base-of-the-data-frame)
-    1.2 [Adding Other Metrics](#12-adding-other-metrics)
-    1.3 [Creation of a Second Data-frame](#13-creation-of-a-second-data-frame)
-    1.4 [Determining CP, W', and FTP](#14-determining-cp-w-and-ftp)
-    1.5 [Adding Intensity Factor, TSS, and Variability Index](#15-adding-intensity-factor-tss-and-variability-index)
-    1.6 [Adding Power Distribution](#16-adding-power-distribution)
-    1.7 [Adding PPR and PPR 2000KJ](#17-adding-ppr-and-ppr-2000kj)
2. [Visualization of the Data](#2-visualization-of-the-data)
-    2.1 [Overview of the Dataframes](#21-overview-of-the-dataframes)
-    2.2 [Distance, Duration, and TSS](#22-distance-duration-and-tss)
-    2.3 [Mean Maximal Power](#23-mean-maximal-power)
-    2.4 [Year Recap](#24-year-recap)
-    2.5 [TSS, ATL, CTL, and TSB Evolution](#25-tss-atl-ctl-and-tsb-evolution)
-    2.6 [Power Distribution](#26-power-distribution)
-    2.7 [PPR and PPR 2000KJ](#27-ppr-and-ppr-2000kj)
-    2.8 [Radar Chart of Power](#28-radar-chart-of-power)

## 1. Creation of a Study Data-frame

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

### 1.7 Adding PPR and PPR 2000KJ

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

