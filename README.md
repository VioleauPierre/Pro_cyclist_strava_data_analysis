# Pro_cyclist_strava_data_analysis

## Project Overview : 
This project aims to learn and practice new skills by analyzing several years of data from a professional cyclist from 2012 to early 2023 (from 14 years old to 25). The data used for this project was retrieved using [Scrap_public_strava_data](https://github.com/VioleauPierre/Scrap_public_strava_data).

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
-    1.5 [Adding Intensity Factor, TSS, and Variability Index](#15-adding-intensity-factor-tss)
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

For the study we need to group the data from the dictionnary into data-frame; the first one will contain one row per activity and the second one one row per day.

### 1.1 Base of the Data-frame

First data frame contain one row per activity, for each activty a type and a date.

### 1.2 Adding Other Metrics

Add distance, duration (with correction on incorrect value due to long break in ride), power avg, normalized power, avg and max heart rate, efficiency factor (power/heart rate), best power for several duration from 5s to 2h and best power after 2000Kj (= under fatigue).

### 1.3 Creation of a Second Data-frame

Creation of the second data frame containing one row per day, add a slicing PPR (Best power for a given duration from 20 day before to 20 after) as all training are not done to achieve the best power.

### 1.4 Determining CP, W', and FTP

Critical power and W' are determined for each day using a combinaison of duration from 3min to 30min, then the FTP is calculate from 3 different way and the max value wil be the used FTP: 
- using the formula of the power duration model : CP + W'/D with D the duration (3600s)
- 0,95 * 20min Power
- ,90 * 8min Power

### 1.5 Adding Intensity factor, TSS

As we now have an FTP value for each day, we can add for each activity intensity factor and TSS. In the second data-frame we can add for each day TSS, Fatigue (ATL), fitness (CTL) and form (TSB).

### 1.6 Adding Power Distribution

Creation of a small data-frame containing one row per year and power distribution for each year. Power is divided in 25w band.

### 1.7 Adding PPR and PPR 2000KJ

Creation of a small data-frame containing the PPR and PPR after 2000KJ for each year.

## 2. Visualization of the Data

Various visualizations used to represent the data.

### 2.1 Overview of the Dataframes

First data-frame is made of 2830 rows and 41 columns, the second one have 4199 rows and 41 columns

### 2.2 Distance, Duration, and TSS

![image](https://github.com/VioleauPierre/Pro_cyclist_strava_data_analysis/assets/129098391/216f0d4f-ed26-4b60-afe8-e8c061275852)

### 2.3 Mean Maximal Power

![image](https://github.com/VioleauPierre/Pro_cyclist_strava_data_analysis/assets/129098391/350a0f73-fe13-4e84-8414-3b402a4e4b1a)
 Mean maximal power show that on short duration there is almost no progression, in contrary we can see an improvement for longer duration. Looking a MMP after 2000Kj, we see a improvement over years, capacity to produce power under fatigue is key determinent of performance in cycling.

### 2.4 Year Recap

![image](https://github.com/VioleauPierre/Pro_cyclist_strava_data_analysis/assets/129098391/4d75b409-253a-46b5-a0ed-c4f2ac3b1eb3)

Interestingly, the rider had bigger years in volume and distance in 2018 and 2019 compare to years after 2020. As he change team in 2020 this is certainly associated with a new coach and new trainings methods.
### 2.5 TSS, ATL, CTL, and TSB Evolution

A plot of the evolution of TSS, ATL, CTL and TSB for each year, for exemple in 2018 we see that the rider was in his best shape for late august and september (Tour de l'avenir, Canadians WT races and World championship).

![image](https://github.com/VioleauPierre/Pro_cyclist_strava_data_analysis/assets/129098391/c5cc85db-9f4c-4d6b-8187-ce42188538dc)

### 2.6 Power Distribution

Plot of the power distribution for every year and a comparison of 2020 to 2022. Looking at the biggest peak for each year, which correspond to endurance ride and as his coach like Z2 ride, we can estimate that the rider can sustain more power for the same level of intensity in 2022 compare to 2020. There is also almost no useless time on bike as we can see very low level of time spend in the zone between 25W and 224W. This an other area of improvement between 2020 and 2022. 

### 2.7 PPR and PPR 2000KJ

Plot of PPR and PPR 2000KJ for each year

### 2.8 Radar Chart of Power

Explain the radar chart comparing power to the top 10% value of professional riders.

