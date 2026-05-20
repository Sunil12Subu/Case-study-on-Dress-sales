# Dress Sales EDA — Retail Fashion Dataset Analysis

> Exploratory data analysis on an online dress sales dataset, examining how product attributes, pricing, and seasonal patterns influence sales performance — with a full data-cleaning pipeline from raw inputs to insight.

---

## Overview

This project performs end-to-end EDA on two linked datasets: one capturing dress attribute details (style, material, colour, size, season) and another tracking weekly sales figures per dress ID. The goal was to clean and standardise messy real-world retail data, then surface actionable patterns in product performance — mirroring typical e-commerce analytics workflows.

## Key questions explored

- Which dress attributes (style, season, material) correlate with higher sales?
- How do price and rating interact with sales volume?
- What is the distribution of sales across different dress categories?
- Which features contain the most missing or invalid values, and how should they be treated?

## Tech stack

[![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=flat&logo=numpy&logoColor=white)](https://numpy.org/)
[![Matplotlib](https://img.shields.io/badge/Matplotlib-11557c?style=flat)](https://matplotlib.org/)
[![Seaborn](https://img.shields.io/badge/Seaborn-4C72B0?style=flat)](https://seaborn.pydata.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)](https://jupyter.org/)

## Project structure

```
dress-sales-eda/
├── data/
│   ├── Attribute+DataSet.csv       # Dress attribute details (style, colour, season, etc.)
│   └── Dress+Sales.csv             # Weekly sales figures per dress ID
├── notebooks/
│   └── EDA+Dress+sales.ipynb       # Full EDA notebook
├── Features description.txt        # Column-level data dictionary
└── README.md
```

## Data cleaning steps applied

- Identifying and correcting data types across mixed-format columns
- Fixing structural issues in rows and columns (headers, delimiters)
- Imputing and removing missing values based on column significance
- Detecting and handling outliers in sales and price columns
- Standardising inconsistent categorical values (e.g. colour and size variants)
- Filtering invalid or out-of-range records prior to analysis

## Selected findings

- **Season** is a strong differentiator — Autumn and Winter dresses show notably different sales distributions compared to Summer styles
- **Price range** has a non-linear relationship with sales; mid-range items outperform both budget and premium ends
- A significant proportion of attribute columns contain **missing or inconsistently encoded values**, requiring careful imputation before any modelling
- **Style and fabric type** show moderate correlation with average weekly sales, suggesting scope for attribute-based recommendation features

## How to run

```bash
git clone https://github.com/Sunil12Subu/Case-study-on-Dress-sales
cd Case-study-on-Dress-sales
pip install pandas numpy matplotlib seaborn jupyter
jupyter notebook EDA+Dress+sales.ipynb
```

---

*Part of a data analysis portfolio by [Sunil Subramaniam Sreedhar](https://linkedin.com/in/sunil-subramaniam-sreedhar) — Senior Data Analyst based in Dortmund, Germany.*
