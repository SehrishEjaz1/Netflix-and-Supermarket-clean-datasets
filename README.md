# Netflix-and-Supermarket-clean-datasets
# (Data Cleaning & Analysis Datasets)

This repository contains the cleaned versions of the datasets used for Assignment 2. These datasets are published and versioned here to be used for future analysis and direct raw loading in upcoming assignments.

## 📦 Repository Details
* **Current Version:** v1.0
* **Release Date:** October 2026
* **Status:** Public (For grading and evaluation purposes)

---

## 📊 Dataset 1: Netflix Movies and TV Shows
* **Original Source:** [Kaggle - Netflix Movies and TV Shows by Shivam Bansal](https://kaggle.com)
* **File Name:** `netflix_titles.csv`

### 🛠️ Data Cleaning Summary:
* **Missing Values:** Handled missing values in critical columns like `director`, `cast`, and `country` by replacing them with 'Unknown' or using mode imputation where appropriate.
* **Date Standardization:** Converted the `date_added` column into a standard `YYYY-MM-DD` datetime format. Added an explicit `year_added` column for trend analysis.
* **Data Consistency:** Stripped leading/trailing whitespaces from textual columns and standardized maturity ratings.
* **Outliers & Flags:** Identified and flagged titles with structural anomalies (e.g., negative duration gaps where the release year was recorded after the platform addition date).

---

## 🛒 Dataset 2: Supermarket Sales
* **Original Source:** Provided by the Course Instructor (`supermarket_Sales.csv`)
* **File Name:** `supermarket_sales.csv`

### 🛠️ Data Cleaning Summary:
* **Data Types:** Validated and converted numerical data types (Prices, Quantities, Taxes, and Totals) ensuring accurate precision.
* **Date & Time:** Standardized the `Date` and `Time` formats to ensure seamless time-series and hourly sales analysis.
* **Format Checking:** Verified that categorical columns like `Product line`, `Branch`, and `Customer type` contained consistent string formats without typos or trailing spaces.
* **Integrity Validation:** Cross-checked mathematical computations (such as `Total = Unit Price * Quantity + Tax`) to ensure no corrupted rows existed.

---

## 🚀 How to Use
The raw CSV files from this repository can be loaded directly into Jupyter Notebook / Google Colab using their respective GitHub raw links for Assignment 3.
