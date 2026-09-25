# 🥩 Food Consumption & Probability Distributions — Statistical Analysis

An exploratory statistics project in **Python** covering descriptive statistics, hypothesis testing, and probability distribution identification, using **Pandas, Seaborn, NumPy** and a custom **permutation test**.

This project was built as a final assignment to practice core statistical analysis skills: descriptive stats, data visualization, resampling-based hypothesis testing, and distribution recognition.

---

## 🎯 Project Overview

| | |
|---|---|
| 🥗 **Part 1** | Descriptive statistics & hypothesis testing on global food consumption / CO2 emissions |
| 🎲 **Part 2** | Identifying probability distributions from raw sampled data |
| 🛠️ **Tools** | Python, Pandas, NumPy, Seaborn, Matplotlib |
| 📁 **Data** | `food_consumption.csv`, `distributions.csv` |

---

## 📁 Repository Structure

```
├── data/
│   ├── food_consumption.csv
│   └── distributions.csv
├── Final_Assignment_Statistic.ipynb
└── README.md
```

---

## 🥗 Part 1 — Food Consumption & CO2 Emissions

Explored a dataset of **food consumption and CO2 emissions by country and food category**.

**Key steps & questions answered:**
- 📊 Used `.describe()` grouped by `food_category` to compare consumption statistics — **dairy products** showed the highest median consumption
- 📦 Built a multi-category **boxplot** of `co2_emission` per food category — **beef** stood out with the largest interquartile range (IQR)
- 🔺 Identified **beef** as the food category with the highest average CO2 emissions
- 🧪 Ran a **permutation test** (20,000 resamples) to test whether the difference in average consumption between **poultry** and **fish** is statistically significant
- ✅ Compared the resulting **p-value** against α = 0.05 to accept/reject the null hypothesis

**Skills demonstrated:** descriptive statistics, `groupby()` aggregation, boxplot/histogram visualization, resampling methods, hypothesis testing, p-value interpretation

---

## 🎲 Part 2 — Identifying Probability Distributions

Given a dataset of 7 columns, each sampled from a different (unlabeled) probability distribution, the goal was to **recognize each distribution visually and statistically**.

**Key steps & questions answered:**
- 🔍 Used `.info()` and `.describe()` to inspect data types (boolean, float, integer) across columns
- 📈 Looped through every column, plotting a **histogram or bar chart** depending on data type
- 🧩 Matched each column to its underlying distribution by shape:
  - `distribution_1` → **Bernoulli**
  - `distribution_2` → **Binomial**
  - `distribution_3` → **Continuous Uniform**
  - `distribution_4` → **Gaussian (Normal)**
  - `distribution_5` → **Poisson**
  - `distribution_6` → **Discrete Uniform**
  - `distribution_7` → **Exponential**

**Skills demonstrated:** distribution recognition, data type inspection, iterative visualization, applied probability theory

---

## 🛠️ Tech Stack

- 🐼 **Pandas** — data loading & descriptive statistics
- 🔢 **NumPy** — resampling & numerical operations
- 📉 **Seaborn** & **Matplotlib** — boxplots, histograms, bar charts
- 📓 **Jupyter Notebook**

---

## ▶️ How to Run

1. Clone this repository
   ```bash
   git clone <your-repo-url>
   cd <repo-name>
   ```
2. Install the required libraries
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Open the notebook in Jupyter and run the cells in order
   ```bash
   jupyter notebook
   ```

---

## 💡 Key Takeaways

- 🐄 Beef stands out sharply from other food categories in both CO2 emission level and variability
- 🧪 Permutation testing is a simple, assumption-light way to check whether an observed difference between two groups is likely due to chance
- 🎲 Distribution shape (skew, boundedness, discreteness) is often enough to identify the underlying probability distribution without formal fitting

---

## 👤 About Me

I'm a junior data analyst building hands-on experience with Python and statistical analysis. This project reflects my growing skills in **descriptive statistics, hypothesis testing, and data visualization**.

📫 Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/giovanni-de-santis-092621322/) or check out more of my projects on GitHub!
