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


## 🧾 Dataset Descriptions

📁 Course_Sales_Data.csv

Gender: Male/Female

Group: Group_A / Group_B (used in A/B testing)

Pre_Score, Post_Score: Scores before and after a course

Study_Hours: How long a learner studied

Exam_Score: Final evaluation score

Income: Monthly income

Satisfaction_Level: 1 to 5 (Likert scale)

Purchased: Whether the course was bought or not (Yes/No)

📁 Packaging Uniqueness Survey

Uniqueness: Category of packaging appeal (Extremely Unique, etc.)

Purchase Likelihood: Customer's buying intent (Likely, Unlikely, etc.)

---


```markdown
# 🧪 All-in-One Hypothesis Testing Project

This repository contains a comprehensive, end-to-end collection of **parametric** and **non-parametric** hypothesis tests implemented in Python, along with synthetic sales-related data. It serves as a complete resource for students, data analysts, and researchers looking to understand and perform various hypothesis tests using real-world style datasets.

---

## ✅ What’s Included

This project includes implementation, assumptions, interpretation, and visualization for the following statistical hypothesis tests:

### 🔹 Parametric Tests (Assume normal distribution)

| Test Name           | Purpose                                                                 |
|---------------------|-------------------------------------------------------------------------|
| **Z-Test**          | Compare sample mean to population mean (known σ)                        |
| **One-sample T-Test** | Compare sample mean to population mean (unknown σ)                     |
| **Independent T-Test** | Compare means between two independent groups                          |
| **Paired T-Test**   | Compare means of the same group before/after a change                   |
| **One-way ANOVA**   | Compare means across 3 or more independent groups                       |
| **Pearson Correlation** | Measure linear relationship between two continuous variables         |
| **F-Test**          | Compare variances between two groups                                    |
| **Bartlett’s Test** | Test if variances are equal across multiple groups                      |
| **Levene’s Test**   | Similar to Bartlett’s but more robust to non-normality                  |
| **Linear Regression** | Test relationship and prediction between variables                     |

---

### 🔸 Non-Parametric Tests (No normality assumption)

| Test Name               | Purpose                                                              |
|--------------------------|-----------------------------------------------------------------------|
| **Mann-Whitney U Test**  | Non-parametric alternative to Independent T-Test                     |
| **Wilcoxon Signed-Rank Test** | Non-parametric alternative to Paired T-Test                      |
| **Kruskal-Wallis Test**  | Non-parametric alternative to One-way ANOVA                          |
| **Spearman Correlation** | Non-parametric correlation (rank-based)                              |
| **Chi-Square Test of Independence** | Test association between two categorical variables         |
| **Chi-Square Goodness of Fit** | Test how well observed frequencies match expected frequencies |
| **Friedman Test**        | Non-parametric alternative to Repeated Measures ANOVA                |

---

## 🛠️ How to Use

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/hypothesis-testing-project.git
cd hypothesis-testing-project
````

### 2. Open Notebook

Open the file in Jupyter Notebook or any Jupyter-compatible environment:

```bash
jupyter notebook "All Hypothesis Test in One File.ipynb"
```

### 3. Run the Cells

Follow each section step by step. The notebook includes:

* Data creation
* Assumption testing (normality, variance, etc.)
* Test application
* Result interpretation

---

## 🔍 Pre-requisite Checks (Done in Notebook)

Before running each test, the following conditions are automatically checked:

* **Normality** → Shapiro-Wilk Test
* **Variance Equality** → Levene’s/Bartlett’s/F-Test
* **Sample Size** → Auto handled in Z-test/T-test selection
* **Data Type** → Ensures test compatibility

---

## 📈 Visualization

* Boxplots
* Histograms
* Distribution Curves
* Pairwise scatterplots
* Heatmaps (for correlation)

These help visually interpret the data and support test selection.

---

## 📚 Learning Goals

By exploring this notebook, you will:

* Understand the differences between parametric vs non-parametric tests
* Know when to use which test and why
* Learn to check test assumptions before application
* Interpret p-values, test statistics, and conclusions correctly
* Practice hypothesis testing using Python and `scipy`, `statsmodels`, `seaborn`, `pandas`, etc.

---

## 🧠 Technologies Used

* **Python**
* `pandas`, `numpy` – data manipulation
* `scipy.stats` – statistical tests
* `matplotlib`, `seaborn` – visualization
* `statsmodels` – regression and ANOVA

---

## ✅ Output Examples

Each test outputs:

* Null and alternative hypothesis
* Test statistic
* p-value
* Interpretation (in natural language)

Example:

```
Z-test Result:
Z-statistic = -0.7473
P-value = 0.4549
Interpretation: No significant difference between sample and population mean
```

---

## 📌 Future Improvements

* Add GUI-based interface for interactive testing
* Integrate real-world datasets from Kaggle/UCI
* Export results as PDF/Excel reports

---

## 🤝 Contributions

Pull requests and suggestions are welcome!
If you find any mistake or want to add more tests or examples, feel free to open an issue.

---

## 📜 License

This project is open-source and free to use under the MIT License.

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


