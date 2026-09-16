# California Housing – Exploratory Data Analysis (EDA)

## 📊 Project Overview

This project presents an **Exploratory Data Analysis (EDA)** of a California Housing dataset as part of my Data Analyst learning journey.

The objective of this analysis is to understand the structure and quality of the dataset, explore important patterns and relationships, identify potential anomalies, and generate meaningful insights for further analysis.

---

## 🎯 Objectives

The main objectives of this project are:

* Understand the dataset structure and data quality
* Explore distributions of key numerical variables
* Compare important variables across categories
* Analyze relationships between numerical variables
* Identify potential outliers and unusual observations
* Generate candidate insights and follow-up questions
* Create decision-relevant visualizations

---

## 🛠️ Tools & Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Google Colab**
* **GitHub**

---

## 📁 Dataset

The cleaned dataset contains:

* **2,000 observations**
* **15 variables**
* No missing values in the final dataset
* Duplicate records were removed during data preparation

### Important Variables

| Variable                   | Description                           |
| -------------------------- | ------------------------------------- |
| `longitude`                | Geographic longitude                  |
| `latitude`                 | Geographic latitude                   |
| `housing_median_age`       | Median housing age                    |
| `total_rooms`              | Total number of rooms                 |
| `total_bedrooms`           | Total number of bedrooms              |
| `population`               | Population                            |
| `households`               | Number of households                  |
| `median_income`            | Median income                         |
| `ocean_proximity`          | Ocean proximity category              |
| `median_house_value`       | Median house value                    |
| `rooms_per_household`      | Derived rooms-to-household ratio      |
| `bedrooms_per_room`        | Derived bedrooms-to-rooms ratio       |
| `population_per_household` | Derived population-to-household ratio |

---

## 🔎 EDA Process

The analysis followed these major steps:

1. Dataset loading and validation
2. Dataset structure and statistical summary
3. Numerical variable distribution analysis
4. Categorical segmentation using `ocean_proximity`
5. Relationship analysis using scatter plots
6. Correlation analysis
7. Investigation of unusual patterns
8. Identification of candidate insights
9. Follow-up question generation
10. Final decision-relevant visualizations

---

## 📈 Key Findings

### 1. Median Income and House Value

The correlation between `median_income` and `median_house_value` was:

**0.942**

This indicates a **very strong positive linear association** between the two variables in this dataset.

> Correlation does not imply causation.

---

### 2. Possible Upper Cap in House Values

There are **32 observations out of 2,000**, representing **1.6% of the dataset**, with:

`median_house_value = 500001`

The repeated maximum value suggests a possible upper cap in the variable.

This should be considered when interpreting high-value properties.

---

### 3. Differences Across Ocean-Proximity Categories

Average house values varied across the different `ocean_proximity` categories.

The `ISLAND` category had only **19 observations**, so comparisons involving this group should be interpreted cautiously.

These differences represent observed associations in the dataset and do not establish causation.

---

### 4. Potential Data-Quality Anomaly

An unusually high:

`bedrooms_per_room = 15.39`

was identified.

The corresponding observation contained:

* `total_rooms = 66`
* `total_bedrooms = 1015.54`

This is an unusual combination and should be investigated before using this derived variable in downstream analysis.

---

## 📊 Visualizations

The project includes four key visualizations:

1. **Median Income vs Median House Value**
2. **Average House Value by Ocean Proximity**
3. **Distribution of Median House Value**
4. **Housing Median Age vs Median House Value**

These charts were selected to communicate distributions, category differences, relationships, and potential patterns in the data.

---

## ❓ Follow-up Questions

The analysis generated several questions for further investigation:

* Why are 32 observations capped at exactly `500001`?
* Does the possible upper-value cap affect the income–house-value relationship?
* What explains the extreme `bedrooms_per_room` observation?
* Do house values differ across ocean-proximity categories after controlling for income?
* Are there additional data-quality anomalies in the dataset?

---

## 💡 Key Learning

This project helped me understand that **EDA is not simply about creating charts**.

A good EDA process involves:

**Explore → Compare → Investigate → Validate → Interpret → Ask better questions**

The goal is to understand what the data is telling us while avoiding unsupported conclusions.

---

## 🚀 Future Improvements

Possible next steps include:

* Deeper outlier investigation
* Statistical testing
* More detailed geographic analysis
* Feature relationship analysis
* Predictive modeling
* House-value prediction using machine learning

## 👨‍💻 About the Project

This project is part of my ongoing journey to develop practical **Data Analytics** skills through hands-on projects.

I am currently building experience in:

**Excel | Python | Pandas | Data Visualization | Exploratory Data Analysis | Data Analytics**

---

## 📌 Project Status

**Status: Completed – Phase 1 EDA**

More analysis projects will be added as I continue my Data Analyst learning journey.
