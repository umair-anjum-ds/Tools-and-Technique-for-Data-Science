# 🐍 Data Munging with Python

> A complete, end-to-end data cleaning and analysis notebook using NumPy, Pandas, Scikit-Learn, Matplotlib and Seaborn.

![Python 3](https://img.shields.io/badge/Python-3-blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-green)
![Data Science](https://img.shields.io/badge/Data-Science-orange)

---

## 📌 About This Project

This notebook is a **complete, end-to-end data munging workflow** built entirely in Python. It takes a deliberately messy employee dataset and processes it step-by-step — removing duplicates, fixing inconsistent text, handling missing values, engineering new features, joining tables, reshaping data, running group summaries, and producing visualizations.

All five major Python data science libraries are used throughout the 40-cell notebook, covering the full pipeline from raw messy data to clean, analysis-ready output.

---

## 📦 Libraries Used

| Library | Purpose |
|---|---|
| **NumPy** | Missing values (`np.nan`), numeric arrays and math operations |
| **Pandas** | DataFrames, cleaning, groupby, merge, pivot — the core of the notebook |
| **Scikit-Learn** | Label encoding categorical columns for ML-readiness |
| **Matplotlib** | Bar charts, histograms and low-level plot control |
| **Seaborn** | Box plots, scatter plots, count plots and heatmaps |

---

## 📋 The Dataset

A small but intentionally messy employee table with **8 raw rows** and **6 columns**:

| employee_id | name | age | gender | salary | department |
|---|---|---|---|---|---|
| 101 | Ali Khan | 25 | M | 50000 | IT |
| 102 | ` Sara Ahmed ` | NaN | Female | $60,000 | HR |
| 103 | Ahmed Raza | 32 | Male | 55000 | it |
| 104 | Fatima Noor | 29 | F | NaN | Finance |
| 105 | Usman Ali | 41 | male | 85000 | `HR ` |
| ⚠️ 103 | Ahmed Raza | 32 | Male | 55000 | it |
| 106 | Ayesha Malik | 27 | F | 65000 | FINANCE |
| 107 | Bilal Shah | 35 | MALE | $72,000 | ` Hr` |

> ⚠️ Issues include: duplicate IDs, extra whitespace, inconsistent gender/department casing, salary as strings with `$` and `,`, and missing values.

---

## 📓 Notebook Contents (40 Cells)

| Cell | Topic | Libraries |
|---|---|---|
| 1 | Import libraries | pandas, numpy, sklearn, matplotlib, seaborn |
| 2 | Create messy dataset | pandas, numpy |
| 3 | Inspect raw data (head, tail, shape, dtypes, describe) | pandas |
| 4 | Identify missing values | pandas |
| 5 | Identify duplicate records | pandas |
| 6 | Remove duplicate employees | pandas |
| 7 | Clean names — strip whitespace | pandas |
| 8 | Standardize gender values | pandas, numpy |
| 9 | Standardize department names | pandas |
| 10 | Convert salary strings to numbers | pandas |
| 11 | Fill missing age with median | pandas |
| 12 | Fill missing salary with department median | pandas |
| 13 | Create monthly salary column | pandas |
| 14 | Create salary categories (Low / Medium / High) | pandas |
| 15 | Create age groups (Young / Mid-career / Senior) | pandas |
| 16 | Select and drop columns | pandas |
| 17 | Filter rows by conditions | pandas |
| 18 | Sort rows | pandas |
| 19 | Count employees by group | pandas |
| 20 | Summary statistics (mean, median, min, max, sum) | pandas |
| 21 | Salary by department | pandas |
| 22 | Salary by gender | pandas |
| 23 | Department + gender analysis | pandas |
| 24 | Chain pipeline (filter → assign → sort) | pandas |
| 25 | Create benefits dataset | pandas |
| 26 | Left join | pandas |
| 27 | Inner join | pandas |
| 28 | Full (outer) join | pandas |
| 29 | Calculate total compensation | pandas |
| 30 | Wide → Long reshape (.melt) | pandas |
| 31 | Long → Wide reshape (.pivot) | pandas |
| 32 | Data validation checks | pandas |
| 33 | Label encoding (ML prep) | scikit-learn |
| 34 | Bar chart — avg salary by department | matplotlib |
| 35 | Box plot — salary distribution by department | seaborn |
| 36 | Count plot — employees by gender | seaborn |
| 37 | Scatter plot — age vs salary by department | seaborn |
| 38 | Heatmap — salary category vs department | seaborn |
| 39 | Histogram — age distribution | matplotlib |
| 40 | Final cleaned dataset output | pandas |

---

## 🚀 How to Run

**1. Install the required libraries**
```bash
pip install numpy pandas scikit-learn matplotlib seaborn notebook
```

**2. Launch Jupyter Notebook**
```bash
jupyter notebook
```
Your browser will open automatically.

**3. Open the notebook**
Navigate to `data_munging.ipynb` and click to open it.

**4. Run all cells**
Go to **Kernel → Restart & Run All** to execute every cell from top to bottom.

**5. Or run in Google Colab (no install needed)**
Upload `data_munging.ipynb` to [colab.research.google.com](https://colab.research.google.com) and click **Run All**.

---

## 📁 Project Files

| File | Description |
|---|---|
| `data_munging.ipynb` | Main Jupyter Notebook — 40 cells, fully runnable |
| `README.md` | This file |

---

## 🎯 What This Notebook Covers

- Creating and inspecting a DataFrame with **pandas**
- Finding and fixing missing values (`NaN`) with **numpy**
- Removing duplicates and cleaning messy text
- Standardizing inconsistent values (gender, department)
- Engineering new columns (monthly salary, age groups, categories)
- Filtering, sorting, and grouping data
- Joining two DataFrames (left, inner, outer)
- Reshaping data between wide and long format
- Encoding categorical data with **scikit-learn**
- Creating bar charts, box plots, scatter plots, heatmaps, and histograms with **matplotlib** and **seaborn**

---

*Built with Python 3 · NumPy · Pandas · Scikit-Learn · Matplotlib · Seaborn*
