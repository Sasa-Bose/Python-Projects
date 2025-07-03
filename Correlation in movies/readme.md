# 🎬 Movie Dataset Analysis

This project is a data analysis exercise focused on exploring and visualizing relationships in a movie dataset, particularly examining how features like **budget**, **votes**, and **release year** correlate with **gross earnings**.

---

## 📁 Dataset

The dataset used in this analysis is `movies.csv`, which includes the following columns:

- `name`, `rating`, `genre`, `year`, `released`, `score`, `votes`, `director`, `writer`, `star`, `country`, `budget`, `gross`, `company`, `runtime`

---

## 📊 Objectives

- Clean and preprocess the data.
- Identify missing values and handle them.
- Analyze the relationship between movie budget and gross earnings.
- Investigate correlations between numerical features.
- Visualize insights using scatter plots, regression lines, and heatmaps.

---

## 🛠️ Libraries Used

- `pandas` — for data manipulation and analysis
- `numpy` — for numerical operations
- `matplotlib` — for static plotting
- `seaborn` — for advanced visualizations

---

## 🧹 Data Cleaning & Preparation

1. **Handling Missing Data**
   - Checked the percentage of missing values in each column.
   - Filled missing values in `budget` and `gross` with `0`.

2. **Data Type Conversion**
   - Converted `budget` and `gross` to `int64` for numerical operations.

3. **Date Correction**
   - Extracted the correct year from the `released` column to create a new column `yearcorrect`.

4. **Duplicates**
   - Removed duplicate entries from the dataset.

---

## 📈 Exploratory Data Analysis (EDA)

### 1. Budget vs Gross Earnings

- **Scatter Plot**:
  A basic scatter plot was created to visualize the relationship between a movie’s budget and its gross earnings.

- **Regression Plot**:
  A regression line was added using Seaborn to better understand the linear correlation.


## 🔍 Correlation Analysis

- Pearson correlation was used to identify relationships between numerical features such as year, score, votes, budget, gross, and runtime.
- A heatmap was created to visualize the strength and direction of these correlations.
- Strongest positive correlations:
  - Budget vs Gross: 0.75
  - Votes vs Gross: 0.63
  - Year vs YearCorrect: 0.99

---

## 🧠 Encoding Categorical Data

- Categorical (text-based) columns like name, genre, director, company, etc., were converted to numerical values.
- This transformation enabled the inclusion of all columns in the correlation matrix.
- The encoding used assigns a unique integer to each category within a column.

---

## 🔥 Key Insights

- Higher budgets are strongly associated with higher gross earnings.
- Movies that receive more votes also tend to earn more revenue.
- There is a very strong correlation between the originally recorded year and the year extracted from the release date.
- Encoding categorical data allows for a broader correlation analysis across all features, not just numeric ones.

---

## 🧪 How to Run

1. Ensure you have Python installed (version 3.8 or higher is recommended).
2. Install the required libraries: pandas, numpy, matplotlib, and seaborn.
3. Place the `movies.csv` file in the same directory as your analysis script or notebook.
4. Open and run the file using a Python IDE or Jupyter Notebook.

---

## 📌 Future Improvements

- Improve missing value handling using more sophisticated techniques (e.g., median imputation).
- Introduce more advanced feature engineering to uncover deeper insights.
- Integrate data from external sources like IMDb or TMDB to enrich the dataset.
- Apply machine learning models to predict movie success.
- Build interactive dashboards for real-time visualization and exploration.

---

