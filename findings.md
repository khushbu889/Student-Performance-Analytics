
# Student Performance Analytics — Findings

## 1. Average Scores

Among the three subjects, reading had the highest average score, while mathematics had the lowest average score.

This suggests that student performance varied across different academic subjects.

---

## 2. Data Quality

The dataset contains **1,000 student records** and **8 variables**.

The analysis found:

* No missing values
* No duplicate records
* Three numerical score variables
* Five categorical variables

The dataset was therefore suitable for exploratory and predictive analysis.

---

## 3. Gender Analysis

The analysis found differences in average performance across genders.

Female students achieved higher average scores in reading and writing, while male students achieved a higher average mathematics score.

These differences describe patterns within this dataset and should not be interpreted as causal relationships.

---

## 4. Test Preparation Analysis

Students who completed the test preparation course achieved higher average mathematics scores than students who did not complete the course.

To investigate whether this difference was statistically significant, an independent samples t-test was performed.

### Hypotheses

**Null Hypothesis (H₀):** There is no significant difference in mathematics scores between students who completed the test preparation course and those who did not.

**Alternative Hypothesis (H₁):** There is a significant difference in mathematics scores between the two groups.

### Statistical Result

The t-test produced:

* **t-statistic:** 5.787
* **p-value:** 1.04 × 10⁻⁸
* **Significance level:** α = 0.05

Since the p-value is substantially smaller than 0.05, the null hypothesis is rejected.

### Interpretation

There is strong statistical evidence of a difference in mathematics scores between students who completed the test preparation course and those who did not.

---

## 5. Effect Size and Confidence Interval

The mean mathematics score difference between the two groups was calculated to measure the magnitude of the observed difference.

A **95% confidence interval** was also calculated to estimate the uncertainty around the mean difference.

These measures provide additional information beyond statistical significance and help assess the practical importance of the observed difference.

---

## 6. Correlation Analysis

Reading and writing scores showed the strongest positive correlation among the three academic subjects.

This indicates that students who performed well in reading also tended to perform well in writing.

Correlation represents an association between variables and does not establish causation.

---

## 7. Machine Learning Prediction

A binary classification problem was created to predict **high mathematics performance**.

A student was classified as a high performer when their mathematics score was **70 or above**.

The following features were used:

* Gender
* Race/ethnicity
* Parental level of education
* Lunch type
* Test preparation course

---

## 8. Model Evaluation

Two classification models were trained:

1. Logistic Regression
2. Random Forest

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

The models were evaluated on an unseen test dataset to measure their ability to generalize to new observations.

---

## 9. Feature Importance

Random Forest feature importance was used to identify the variables that contributed most strongly to the model's predictions.

This analysis provides insight into which demographic, socioeconomic, and educational characteristics contain useful information for predicting high mathematics performance.

---

## 10. Explainable AI with SHAP

SHAP (SHapley Additive exPlanations) was used to investigate how individual features influenced model predictions.

This provides a more interpretable view of the machine learning model and helps answer:

> Which factors contributed to a prediction of high or low mathematics performance?

SHAP analysis complements traditional feature importance by providing more detailed information about feature contributions.

---

## 11. Overall Conclusion

This project progressed from exploratory data analysis to statistical inference, predictive modeling, and explainable AI.

The analysis found a statistically significant difference in mathematics scores between students who completed the test preparation course and those who did not.

Machine learning models were then developed to predict high mathematics performance, and model interpretation techniques were used to investigate the factors influencing predictions.

The project demonstrates an end-to-end data analytics workflow:

**Data → Exploration → Statistical Testing → Prediction → Evaluation → Explainability**

---

## 12. Limitations

* The dataset contains only 1,000 student records.
* The dataset may not represent all student populations.
* The analysis identifies associations and predictive patterns rather than causal relationships.
* The high-performance threshold of 70 is a modeling choice.
* Important variables such as attendance, study time, previous grades, and learning behavior are not included.
* Model performance may change when evaluated on a different dataset.

---

## 13. Future Research

Future work could:

* Include attendance and study-time data.
* Include previous academic performance.
* Analyze learning behavior over time.
* Use longitudinal student data.
* Compare additional machine learning algorithms.
* Apply more advanced explainable AI methods.
* Investigate personalized academic interventions.
* Evaluate whether predictive models can help identify students who need additional academic support.
