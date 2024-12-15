# Investigating the Effect of Eating Habits on the Academic Performance of Students

## Introduction

Eating habits have been shown to impact the academic abilities of students by influencing cognitive abilities, energy levels, and overall health. Nutrients critical for brain development can be gained through a balanced diet rich in iron, folate, and omega-3 fatty acids. This requires a diet including fruits, vegetables, and whole grains.

Studies indicate that breakfast provides consistent energy and essential nutrients to the brain, which correlates with better academic performance. In contrast, unhealthy eating patterns, such as frequent fast food consumption, lead to fatigue and decreased focus, negatively affecting academic outcomes.

The frequency and quality of meals, particularly breakfast, play an important role in academic performance. Students who skip breakfast tend to score lower in cognitive assessments than those who eat it regularly. This underscores the need for interventions promoting healthier eating behaviors to improve dietary habits and academic outcomes. Achieving this, however, relies on data-driven research to analyze eating habits and identify pivotal features affecting academic performance.

## Objectives:
- To analyze the relationship between grade point average (GPA) and various eating habits.
- To identify the most important features in predicting GPA.

## 1. Dataset Overview

The food dataset was sourced from the Kaggle database. Key columns included `breakfast`, `exercise`, `eating out`, `weight`, `calories per day`, `gender`, `mother's education`, among others. GPA served as the target variable.


## 2. Correlation Analysis

The correlation heatmap identified relationships between numerical features. Most correlations were weak (< 1), indicating variable independence. 

![image](https://github.com/user-attachments/assets/0edc47d8-1e61-4f79-b53a-53695310acfd)

**Fig 1: Correlation heatmap to assess the relationship between different variables.**


Notable findings:
- A negative correlation (close to zero) exists between self-perception of weight and feeling healthy. 
- Waffle cookie consumption negatively correlates with both self-perceived weight and feelings of healthiness.


## 3. Univariate Analysis

### GPA Distribution
A histogram visualized the distribution of GPA, showing a right-skewed trend:

![image](https://github.com/user-attachments/assets/68621ff9-1179-441f-8b25-50201c7aa961)

**Fig 2: Overall distribution of GPA scores.**

- GPA values concentrated around 3.0 and 3.75–4.0.
- Peaks at 3.0 (highest frequency) and 3.5–3.8 (secondary cluster).
- Fewer students scored below 2.5 or at the extreme upper end (4.0).

### Outliers in GPA and Weight
Boxplots highlighted:
- **GPA:** Concentrated between 3.25–3.75, median ~3.5. Outliers indicate a few underperforming students.

![image](https://github.com/user-attachments/assets/08ca2401-80eb-4706-aa95-8308bcd12c40)

**Fig 3: Identifying outliers in GPA values**

- **Weight:** Concentrated between 135–180, with outliers on the higher end, possibly linked to junk food consumption or low exercise frequency.

![image](https://github.com/user-attachments/assets/03e625c6-bb49-4fd6-92ef-4906373a800a)

**Fig 4: Identifying outliers in weight values**

## 4. Bivariate Analysis

### Calories per Day vs. GPA

![image](https://github.com/user-attachments/assets/8bac249b-df19-4d45-a8c4-39085cbe7989)

**Fig 5: Calories per day vs. GPA plot**

A scatter plot revealed no clear trend, indicating a weak relationship. High GPA values appeared across all calorie intake levels.

### Breakfast and GPA

![image](https://github.com/user-attachments/assets/5c0ed4d1-8a8a-482d-88cb-d625d632eefa)

**Fig 5: Analyzing the effect of breakfast on GPA values**

Students who eat breakfast have a slightly higher median GPA (~3.5) compared to non-breakfast eaters (~3.4). The range for breakfast eaters is wider, with outliers suggesting additional influencing factors.

### Gender and GPA

![image](https://github.com/user-attachments/assets/9246c0f4-224f-42ff-a9c5-6bf0551e81d3)

**Fig 6: Gender vs GPA**

The boxplot shows:
- Median GPA for males: 3.5.
- Median GPA for females: 3.3.
- Both genders displayed similar variability and overall GPA ranges.

### Exercise Frequency and GPA

![image](https://github.com/user-attachments/assets/2a8ebacf-595a-4f04-8ca1-205ee0de5918)

**Fig 7: Exercise vs GPA plot**

Boxplots by exercise frequency shows:
- **Frequency 1:** Median GPA ~3.4, wider range with outliers.
- **Frequency 2:** Median GPA slightly higher (~3.5), similar range to Frequency 1.
- **Frequency 3:** Narrower distribution, clustered around 3.0, with multiple outliers.


## 5. Multivariate Analysis

![image](https://github.com/user-attachments/assets/e4b5101c-9f92-4873-ae21-d6dbbb762658)

**Fig 8: Exploring the relationship between key features**

This pairplot explores relationships among key features like GPA, gender, weight, calorie intake, breakfast habits, and exercise frequency. 

Key insights:
- **GPA and Exercise:** Moderate exercise correlated with slightly higher GPA.
- **Weight and Calories:** Positive correlation, as expected.
- **GPA and Eating Out:** No clear relationship.
- **Gender Clustering:** Gender showed categorical clustering but no strong correlations with GPA or weight.


## 6. Feature Importance Analysis

![image](https://github.com/user-attachments/assets/2f69c73d-04d3-4bb1-b434-dbc45d213d6b)

**Fig 9: Feature importance in predicting the GPA values**

A Random Forest model ranked feature importance for predicting GPA. Surprisingly, the top predictor was the mother’s education level, emphasizing the role of family background in academic success.


## Conclusion and Interpretation

The analysis reveals that eating habits and lifestyle factors have a small but noticeable impact on GPA:
- **Breakfast:** Students who eat breakfast tend to perform slightly better academically.
- **Exercise:** Moderate exercise (1–2 times per week) is linked to better GPAs than more frequent exercise.
- **Weight and Calories:** These are interrelated but show no clear effect on GPA.

The most critical factor influencing GPA is **mother’s education**, highlighting the significance of family background. While healthy eating and exercise help, educational support at home has the strongest impact on student success.

## References

Adolphus, K., Lawton, C. L., & Dye, L. (2013). The effects of breakfast on behavior and academic performance in children and adolescents. Frontiers in Human Neuroscience, 7. https://doi.org/10.3389/fnhum.2013.00425
