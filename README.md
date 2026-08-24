# Student Performance Analytics

## 📌 Project Overview

This project performs an end-to-end analysis of student academic performance using exploratory data analysis, statistical hypothesis testing, machine learning, and explainable AI.

The main objective is to investigate factors associated with mathematics performance and evaluate whether demographic, socioeconomic, and educational characteristics can be used to predict high mathematics performance.

---

## 🎯 Research Questions

This project investigates the following questions:

1. Does completing a test preparation course significantly affect mathematics scores?
2. What factors are associated with differences in student performance?
3. Can student characteristics be used to predict high mathematics performance?
4. Which machine learning model provides better predictive performance?
5. Which features contribute most to the model's predictions?

---

## 📊 Dataset

The dataset contains information about **1,000 students**.

### Features

* Gender
* Race/ethnicity
* Parental level of education
* Lunch type
* Test preparation course
* Mathematics score
* Reading score
* Writing score

**Source:** Kaggle

---

## 🔍 Exploratory Data Analysis

The project begins with exploratory analysis to understand the distribution and relationships within the dataset.

The analysis includes:

* Data quality checking
* Missing-value analysis
* Duplicate-value checking
* Descriptive statistics
* Average score analysis
* Gender-based comparisons
* Test preparation analysis
* Correlation analysis
* Data visualizations

---

## 🧪 Statistical Analysis

An independent samples t-test was conducted to investigate whether mathematics scores differed significantly between students who completed the test preparation course and those who did not.

A significance level of **α = 0.05** was used.

The analysis produced a statistically significant result, indicating a significant difference in mathematics scores between the two groups.

Effect size information and a **95% confidence interval** were also calculated to provide additional context about the observed difference.

---

## 🤖 Machine Learning

The project formulates high mathematics performance as a binary classification problem.

A student is classified as a **high performer when their mathematics score is 70 or above**.

### Models

Two machine learning models were evaluated:

* Logistic Regression
* Random Forest Classifier

### Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix

The models were trained using an 80/20 train-test split with stratification.

---

## 🧠 Explainable AI

To understand the factors influencing model predictions, the project uses:

### Feature Importance

Random Forest feature importance is used to identify the variables that contribute most to predictions.

### SHAP

SHAP (SHapley Additive exPlanations) is used to provide a more detailed interpretation of model predictions.

This helps move beyond simply asking:

> "How accurate is the model?"

and instead investigates:

> "Why did the model make this prediction?"

---

## 📈 Key Findings

The analysis indicates that:

* Students who completed the test preparation course had significantly different mathematics scores compared with students who did not complete the course.
* Test preparation and other demographic, socioeconomic, and educational characteristics provide useful information for predicting high mathematics performance.
* Machine learning models can be used to identify patterns associated with high mathematics performance.
* Feature importance and SHAP analysis provide insight into the variables influencing model predictions.

---

## ⚠️ Limitations

* The dataset contains 1,000 student records and may not represent all student populations.
* The analysis identifies associations and predictive patterns but does not establish causal relationships.
* Defining a high-performing student as having a mathematics score of 70 or above is a modeling choice.
* Additional factors such as attendance, study time, previous academic performance, and learning behavior are not included.
* Model performance may differ when evaluated on a different dataset.

---

## 🔬 Future Research

Future work could:

* Incorporate attendance and study-time information.
* Include previous academic performance.
* Analyze student learning behavior.
* Use longitudinal student data.
* Compare additional machine learning models.
* Investigate personalized academic interventions.
* Explore whether predictive models can help identify students who may benefit from additional academic support.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* SciPy
* SHAP
* Jupyter Notebook
* VS Code

---

## 📁 Project Structure

```text
Student-Performance-Analytics/
│
├── data/
│   └── student_data.csv
│
├── notebooks/
│   └── student_performance_analysis.ipynb
│
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run

Clone the repository:

```bash
git clone https://github.com/khushbu889/Student-Performance-Analytics.git
```

Navigate to the project:

```bash
cd Student-Performance-Analytics
```

Install the required libraries:

```bash
pip install -r requirements.txt
```

Open the notebook:

```bash
jupyter notebook
```

Then open:

```text
notebooks/student_performance_analysis.ipynb
```

---

## 👩‍💻 Author

**Khushboo Kumari**

B.Tech Computer Science Engineering
Interested in Data Analytics, Machine Learning, and AI
