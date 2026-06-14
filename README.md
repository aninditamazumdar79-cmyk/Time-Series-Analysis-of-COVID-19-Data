# Time-Series-Analysis-of-COVID-19-Data
Time-Series Analysis of COVID-19 Data.Summer Internship Project for IDEAS Foundation, ISI Kolkata (May–June 2026)."
# Time-Series Analysis of COVID-19 Data

This repository contains the project notebook for the **Time-Series Analysis of COVID-19 Data**, developed as part of the **Summer Internship Program 2026** at the **IDEAS - Institute of Data Engineering, Analytics and Science Foundation** (Technology Innovation Hub @ Indian Statistical Institute, Kolkata).

## 📌 Project Overview
The objective of this project is to perform comprehensive time-series analysis, exploratory data analysis (EDA), and clustering evaluation on global COVID-19 records. The project focuses on handling continuous pandemic data, transforming features to structural time-series objects, and isolating patterns across distinct geographical regions. Additionally, basic unsupervised machine learning evaluation is conducted on benchmark feature arrays.

## 🛠️ Key Features & Tasks Completed
* **Data Processing & Type Conversion**: Handled raw global pandemic files and programmatically converted temporal elements into proper `datetime64[ns]` schemas using `pandas`.
* **Slicing & Subsetting**: Filtered extensive data sets into targeted time windows (from March 2020 through August 2023 inclusive) for streamlined time-series exploration.
* **Geographical Aggregations**: Grouped statistics to pinpoint the top 5 most affected nations based on cumulative historical counts.
* **Temporal Downsampling**: Formulated granular trends into quarterly and monthly intervals utilizing custom pivot matrices sorted by World Health Organization (WHO) zones.
* **Unsupervised Clustering**: Trained a 10-cluster Scikit-Learn `KMeans` algorithm on high-dimensional data arrays.
* **Performance Evaluation**: Crafted a tracking mechanism utilizing `scipy.stats.mode` to handle cluster remapping and computed a robust macro-averaged F1 Score.

## 📁 Dataset Information
1. **WHO-COVID-19-global-daily-data.csv**: Contains daily recorded figures for new infections, cumulative caseloads, new fatalities, and total deaths categorized by country codes and explicit WHO regions.
2. **MNIST Digits Dataset**: Comprises 1,797 samples with 64 feature dimensions mapping handwritten numerals (0-9) used for the machine learning validation module.

## 💻 Technical Stack
* **Language**: Python 3.10+
* **Environment**: Google Colab / Jupyter Notebook
* **Primary Libraries**: 
  * `pandas` (Data structure handling, datetime parsing, and pivot tables)
  * `numpy` (Vector operations)
  * `scikit-learn` (Dataset streaming, KMeans clustering, and metrics evaluation)
  * `scipy` (Statistical mode distribution parsing)

## 📊 Summary of Core Analytical Results
* **Trimmed Time Frame Volume**: 306,960 structural logs parsed across active parameters.
* **Peak Infection Event**: Globally recorded on **2022-01-30**, reaching a single-day high of **8,401,963** newly confirmed positive cases.
* **Top 5 Most Affected Sovereign Territories**: 
  1. United States of America (Max Cumulative: 103,436,829 cases)
  2. China (Max Cumulative: 99,381,761 cases)
  3. India (Max Cumulative: 45,055,954 cases)
  4. France (Max Cumulative: 39,042,805 cases)
  5. Germany (Max Cumulative: 38,437,875 cases)
* **K-Means Model Performance**: Achieved a macro-averaged F1 score of **0.8628** on the classification sub-assignment after implementing true-label index alignment.

## 🚀 How to Run the Project
1. Clone this repository to your local machine or open it inside Google Colab:
   ```bash
   git clone https://github.com
   ```
2. Download the required WHO global daily tracking file and upload it when prompted by the `files.upload()` pipeline cell.
3. Execute the notebook sequentially to regenerate the summary dataframes, regional pivot views, and clustering metrics.

---
**Created by**: Samyabrata Roy  
**Designation**: Associate Software Developer  
**Organization**: IDEAS - Institute of Data Engineering, Analytics and Science Foundation (Summer 2026)
