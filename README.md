# Do Students Who Receive Tutoring Have Different Academic Performance?

A statistical analysis project examining whether tutoring sessions are associated with differences in exam scores, using the Kaggle Student Performance dataset.

## Main Research Question

Do students who receive tutoring have different academic performance?

### Sub-Questions

1. What does the distribution of exam scores look like for tutored vs. non-tutored students?
2. Is there a statistically significant difference between the mean exam scores of the two groups?
3. How much of a difference in scores can we expect between students who get tutoring and those who don't?

## Variables

| Variable | Type | Role |
|---|---|---|
| Tutoring Session (Yes/No) | Categorical | Independent Variable (IV) |
| Exam Score | Numeric | Dependent Variable (DV) |

**Note:** `Tutoring_Sessions` in the raw dataset is numeric (0–3). It is recoded into two groups — "No Tutoring" (0 sessions) and "Tutored" (1+ sessions) — to match the research question.

## Dataset

- **Source:** Kaggle — Student Performance Dataset
- **Format:** CSV
- **Key columns used:** `Tutoring_Sessions`, `Exam_Score`

## Methodology

1. Data cleaning and grouping (`Tutoring_Sessions` → `Tutoring` category)
2. Descriptive statistics (mean, median, standard deviation)
3. Boxplot visualization of exam scores by group
4. Assumption checks (Shapiro-Wilk for normality, Levene's test for equal variance)
5. Two-sample t-test
6. 95% Confidence Interval for the mean difference (μ1 − μ2)
7. Supplementary correlation check between number of sessions and exam score

## Tools & Libraries

- Python 3
- pandas, numpy
- matplotlib, seaborn
- scipy.stats
