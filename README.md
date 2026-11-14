# CodeAlpha 
## Task 1: Exploratory Data Analysis (EDA) on Students Performance
**Notebook by:** Ranjana Singh 
**Notebook:** [codealpha-eda-students-performance.ipynb](codealpha-eda-students-performance.ipynb)


## Project Overview
This project performs Exploratory Data Analysis (EDA) on the Students Performance in Exams dataset using Python.

The objective is to explore student scores, identify patterns, understand relationships between subjects, and analyse academic performance.

## Dataset
- **Source:** https://www.kaggle.com/datasets/spscientist/students-performance-in-exams
- **Author:** spscientist
- **Records:** 1,000 students
- **Original Features:** 8 columns

The dataset is not included in this repository. Download it from the [Kaggle dataset page](https://www.kaggle.com/datasets/spscientist/students-performance-in-exams). No license is specified on the page.

## Objectives

- Understand the structure and quality of the data.
- Compare scores across student groups.
- Study how the three subject scores relate to each other.
- Detect outliers and group students into performance categories.


## Analysis Performed
1. Load the dataset and inspect it with `head()`, `shape`, `info()` and `describe()`.
2. Check for missing values and duplicates.
3. Review category distributions (gender, parental education, test preparation).
4. Compare average scores by gender, test preparation, parental education and lunch type, with bar charts.
5. Analyse correlations between subjects with a heatmap.
6. Plot score distributions (histograms) and spread (boxplot).
7. Detect outliers using the IQR method.
8. Create an `average_score` column and categorise performance.
9. Summarise the final insights.

**Performance categories (based on average score):**

| Category | Average score |
|---|---|
| Excellent | 80 and above |
| Good | 60 to 79 |
| Average | 40 to 59 |
| Needs Improvement | below 40 |


## Key Learning Outcomes
- **Overall scores:** average Math 66.1, Reading 69.2 and Writing 68.1. The overall average score is about 67.8.
- **Gender:** males scored higher in Math (68.7 vs 63.6). Females scored higher in Reading (72.6 vs 65.5) and Writing (72.5 vs 63.3).
- **Test preparation:** students who completed the course scored higher in all three subjects, with the biggest gap in Writing (74.4 vs 64.5).
- **Parental education:** students whose parents hold a master's or bachelor's degree scored highest, and those whose parents had only high school education or less scored lowest.
- **Lunch type:** students with standard lunch scored higher in every subject. The biggest gap is in Math (70.0 vs 58.9).
- **Correlation:** Reading and Writing are very strongly correlated (0.95). Math is strongly correlated with Reading (0.82) and Writing (0.80).
- **Outliers:** Math 8, Reading 6 and Writing 5. These are a small share of the data, so no records were removed.
- **Performance categories:** Good 517, Average 255, Excellent 198, Needs Improvement 30.

> These findings show associations in this dataset. They do not prove cause and effect.

## Tools and Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Kaggle Notebook
