# 📊 All-in-One Statistical Testing Project: Parametric & Non-Parametric Analysis

## 🎥 Video Walkthroughs

* 🎓 **Full Code + Concept Explanation**: [Watch Here](https://youtu.be/vqXt1wZuaIk?si=byCFR5mYxtwTQQOV)
* 🧠 **Non-Technical Output Summary (For Recruiters)**: [Watch Here](https://youtu.be/link_to_recruiter_friendly_video)

---

## 📌 Project Overview

This comprehensive project demonstrates the application of **all major hypothesis testing techniques** (both parametric and non-parametric) using a synthetic sales and survey dataset. It is designed to help learners and professionals understand how and when to use each test through hands-on examples and business scenarios.

---

## 🎯 Problem Statement

Real-world datasets often demand diverse statistical approaches based on the data type and distribution. This project aims to teach:

* When to use **Parametric** vs **Non-Parametric** tests
* How to check assumptions (e.g., normality, variance homogeneity)
* How to implement and interpret hypothesis tests in Python

---

## 🧠 Objectives

* Explore various statistical tests under different conditions.
* Build decision-making skills using real-world hypotheses.
* Create a unified framework combining all hypothesis tests in one notebook.

---

## 📊 Dataset Description

The dataset includes survey-style and numeric performance data with the following features:

* `Exam_Score`: Continuous variable (normally distributed) used for mean comparison tests.
* `Sales_Before`, `Sales_After`: Used for paired tests.
* `Region`, `Branch`: Categorical values for group comparisons.
* `Packaging_Uniqueness`, `Purchase_Likelihood`: Categorical variables used for Chi-Square testing.
* `Product_Quality_Rank`, `Satisfaction_Score`: Ordinal values used for non-parametric rank tests.

---

## 🧪 Statistical Tests Overview

### 🔷 PARAMETRIC TESTS

#### 1. One-Sample Z-Test

* 🎯 Used when population standard deviation is **known**
* 🧪 Goal: Is sample mean significantly different from population mean?
* ✅ Assumptions: Normality, continuous data, known σ
* 🧾 Example: Is average `Exam_Score` different from 60?

#### 2. One-Sample T-Test

* 🎯 Used when population σ is **unknown**
* 🧪 Goal: Same as Z-test but with sample std
* ✅ Assumptions: Normality, continuous, unknown σ

#### 3. Independent T-Test

* 🎯 Compare means of **two independent groups**
* ✅ Assumptions: Normality, equal variances (Levene’s Test)
* 🧾 Example: Is mean score of `Branch A` different from `Branch B`?

#### 4. Paired T-Test

* 🎯 Compare means of **related groups**
* 🧪 Goal: Check if mean difference ≠ 0
* ✅ Assumptions: Normality of difference scores
* 🧾 Example: `Sales_Before` vs `Sales_After`

#### 5. One-Way ANOVA

* 🎯 Compare means of **3+ groups**
* ✅ Assumptions: Normality, equal variances
* 🧾 Example: Compare `Exam_Score` across multiple `Regions`

#### 6. Pearson Correlation

* 🎯 Check linear relationship between two continuous variables
* ✅ Assumptions: Normality, linearity
* 🧾 Example: Relationship between `Hours_Studied` and `Exam_Score`

#### 7. F-Test (Equality of Variance)

* 🎯 Compare variances of two groups
* ✅ Assumptions: Normality, continuous

#### 8. Bartlett’s Test

* 🎯 Test equal variances across 3+ groups
* ✅ Assumptions: Normality, homoscedasticity

#### 9. Levene’s Test

* 🎯 Similar to Bartlett but more robust to non-normality

---

### 🔶 NON-PARAMETRIC TESTS

#### 1. Chi-Square Test of Independence

* 🎯 Assess relationship between two categorical variables
* ✅ Assumptions: Expected frequency ≥ 5
* 🧾 Example: Is `Packaging_Uniqueness` related to `Purchase_Likelihood`?

#### 2. Mann-Whitney U Test

* 🎯 Alternative to Independent T-test
* ✅ Assumptions: Ordinal or continuous data, non-normal

#### 3. Wilcoxon Signed-Rank Test

* 🎯 Alternative to Paired T-test
* ✅ Assumptions: Paired, ordinal/non-normal

#### 4. Kruskal-Wallis H Test

* 🎯 Alternative to One-Way ANOVA
* ✅ Assumptions: Ordinal/non-normal data

#### 5. Spearman Rank Correlation

* 🎯 Non-parametric correlation
* ✅ Assumptions: Ordinal data or non-linear monotonic relationship

---

## 🧪 Assumption Checks

| Test Type      | Normality Required? | Equal Variance? | Data Type   |
| -------------- | ------------------- | --------------- | ----------- |
| Z / T-Test     | ✅ Yes               | 🔁 Sometimes    | Continuous  |
| ANOVA          | ✅ Yes               | ✅ Yes           | Continuous  |
| Chi-Square     | ❌ No                | ❌ No            | Categorical |
| Mann-Whitney   | ❌ No                | ❌ No            | Ordinal     |
| Wilcoxon       | ❌ No                | ❌ No            | Ordinal     |
| Kruskal-Wallis | ❌ No                | ❌ No            | Ordinal     |
| Pearson Corr   | ✅ Yes               | ❌ N/A           | Continuous  |
| Spearman Corr  | ❌ No                | ❌ N/A           | Ordinal     |

---

## 🛠 Technologies Used

* Python (pandas, numpy, scipy, seaborn, matplotlib)
* Jupyter Notebook

---


## 🚀 How to Run

1. Clone the repository
2. Open Jupyter Notebook
3. Run all cells sequentially

---

## 🧾 Final Summary

This notebook acts as a statistical testing toolkit. It lets you:

* Decide which test to use based on data & assumptions
* Learn via real-world examples
* Visualize and interpret statistical results

---

## 🤝 Contact

Made by Md. Mahamud Mredha – feel free to connect:

* LinkedIn: [https://www.linkedin.com/in/md-mahamud-mredha-294046208/](https://www.linkedin.com/in/md-mahamud-mredha-294046208/)
* GitHub: [https://github.com/mdmahamudmredha](https://github.com/mdmahamudmredha)
* YouTube: [Dropout Programmer](https://www.youtube.com/@DropoutProgrammer)

---

> "Statistical thinking will one day be as necessary for efficient citizenship as the ability to read and write." — H.G. Wells


