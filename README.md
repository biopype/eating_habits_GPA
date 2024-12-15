# Investigating the Effect of Eating Habits on the Academic Performance of Students

This project analyzes the relationship between eating habits and academic performance (GPA), highlighting key factors influencing student success.

## Data
Comprehensive report: [report](report.md)

Dataset: [dataset](dataset.csv)

Code: [code](code.py)

Results: [results](results/)

## Objectives
- Investigate the correlation between GPA and eating habits.
- Identify key predictors of GPA.

## Dataset
- Source: Kaggle.
- Features: `breakfast`, `exercise`, `eating out`, `weight`, `calories`, `gender`, `mother's education`, and GPA (target).

## Key Findings
1. **Breakfast & GPA**: Students who eat breakfast have slightly higher GPAs (~3.5) than those who skip (~3.4).
2. **Exercise**: Moderate exercise (1–2 times/week) correlates with better GPAs.
3. **Weight & Calories**: Positive correlation, but no clear impact on GPA.
4. **Mother’s Education**: The strongest predictor of GPA, emphasizing family background.

## Analysis Methods
- Correlation heatmaps: Identified weak relationships between variables.
- Boxplots & Histograms: Highlighted GPA distribution and outliers.
- Random Forest: Ranked feature importance.

## Conclusion
Healthy eating and exercise moderately impact GPA, but family background, particularly mother’s education, is the strongest influence on academic success.
