# Bank Marketing - Data Mining Project 🏦📊

## 📌 Project Overview
This repository contains a semester project for the **"Statistical Methods of Data Mining"** course at the Czech University of Life Sciences Prague (ČZU v Praze). 

The primary goal of this project is to analyze a **real-world dataset from a real Portuguese bank, sourced from Kaggle**. We built predictive models to determine whether a client will subscribe to a term deposit (target variable: `y`) based on the results of their telemarketing campaigns.

**Authors:** Ondřej Kotala, Daiana Bikmaeva, Robert Sládek, Pavel Dikan  
**Year:** 2025

## 🛠 Tools & Techniques
* **Tool:** IBM SPSS Modeler
* **Techniques Used:** * Data Understanding & Exploration
  * Data Preparation (Handling missing values, outlier treatment)
  * Feature Engineering (Addressing multicollinearity, capping extreme values)
  * Predictive Modeling & Evaluation

## 📂 Repository Structure
* `/data/` — Contains the campaign datasets (`bank-additional-full.csv`, `bank-additional.csv`) and the variable description text file.
* `/models/` — Contains IBM SPSS Modeler streams (`.str`) and generated models (`.gen`).
* `/docs/` — Comprehensive project documentation and reports (e.g., `MARKETING V5_1.pdf`).

## 📊 Key Insights & Data Preparation
During the **Data Understanding** and **Data Preparation** phases, several critical steps were taken to ensure high model quality:
* **Hidden Missing Values:** Addressed implicit missing data (labeled as "unknown") across categorical variables.
* **Multicollinearity:** Identified and resolved high correlation among macroeconomic indicators (`euribor3m`, `emp.var.rate`, and `nr.employed`) by keeping only the most relevant variable.
* **Outlier Capping:** Handled extreme values in variables like `campaign` (number of contacts). The right tail was capped at the 99th percentile (value of 14) to make the distribution more compact and robust for modeling.
* **Target Leakage:** Removed the `duration` variable as highly predictive but unknown before a call is actually made, ensuring a realistic predictive model.

## 📄 Documentation
For a deep dive into the business logic, methodology, statistical analysis, and final model evaluation, please refer to the main documentation file located in the `/docs/` folder.

## 🎓 What I Learned (Skills Acquired)
* **End-to-End Analytics:** Mastered the complete data mining lifecycle using the CRISP-DM framework, from business understanding to model evaluation.
* **Data Quality Management:** Learned how to identify and solve critical data issues in real-world datasets, such as hidden missing data (e.g., "unknown" categories), outliers, and target leakage.
* **Statistical Rigor:** Gained practical experience in exploratory data analysis (EDA), correlation analysis, and resolving multicollinearity to build simpler, more reliable predictive models.
* **Visual ML Pipelines:** Developed strong hands-on skills in creating visual machine learning workflows and building binary classification models using **IBM SPSS Modeler**.
