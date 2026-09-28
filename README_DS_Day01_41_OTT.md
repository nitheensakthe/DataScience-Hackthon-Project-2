# 🎬 OTT — Why Do Users Stop Watching?

## 📌 Project Overview

This Data Science project investigates **why OTT users reduce or stop their viewing activity after a few weeks**.

The analysis uses user viewing history, session duration, content genre, subscription plan, inactivity period, and retention status to identify behavioural patterns and early signs of declining engagement.

The main objective is **behavioural analysis**, supported by a Random Forest machine-learning model for the challenge's prediction target.

---

## 🎯 Problem Statement

An OTT platform has observed that some users stop watching after a few weeks.

This project investigates:

1. What different viewing behaviour patterns exist?
2. What is the average watch time for different customer segments?
3. Does content diversity influence engagement?
4. What are the early signs of declining engagement?
5. How do subscription plans differ in engagement and retention?
6. Which user behaviours are associated with retention?
7. Can a Random Forest model predict the defined retention target?

---

## 💡 Business Objective

The project aims to provide evidence that can help an OTT platform:

- Improve user engagement
- Detect users at risk of becoming inactive
- Personalize content recommendations
- Improve subscription-plan strategies
- Increase retention
- Reduce user churn

---

## 📊 Dataset

The dataset contains the following fields:

| Feature | Description |
|---|---|
| `User_ID` | Unique identifier for each user |
| `Viewing_History` | User's viewing-history information |
| `Session_Duration` | Duration of viewing sessions |
| `Content_Genre` | Genre/category of content watched |
| `Subscription_Plan` | User's subscription plan |
| `Inactivity_Period` | Number of inactive days/period |
| `Retention_Status` | User retention outcome |

---

## 🧹 Data Cleaning & Validation

The Colab notebook performs:

- Missing-value checks
- Duplicate checks
- Data-type validation
- User-ID validation
- Numerical-value validation
- Outlier inspection
- Categorical-value validation
- Inactivity-period validation
- Retention-status validation
- Feature engineering

Possible derived features include:

```text
Average_Session_Duration
Content_Diversity
Engagement_Score
Inactivity_Category
Session_Category
```

---

# 🔍 Behavioural Analysis

The primary focus of the project is understanding **how users behave before becoming inactive**.

Users can be analysed according to:

```text
Session Duration
        +
Content Diversity
        +
Inactivity Period
        +
Subscription Plan
        +
Retention Status
```

This helps identify groups such as:

- Highly engaged users
- Regular users
- Low-engagement users
- At-risk users
- Inactive users

The exact segments should be based on the patterns found in the dataset.

---

# ⏱️ Average Watch Time by Customer Segment

Average session duration is calculated for different user segments.

Example:

```text
Customer Segment
       ↓
Average Session Duration
       ↓
Engagement Comparison
```

This helps determine which behavioural groups spend more time watching content.

---

# 🎬 Content Diversity Analysis

Content diversity measures how many different genres a user watches.

For example:

```text
User A → Drama only
User B → Drama + Comedy
User C → Drama + Comedy + Action + Thriller
```

A broader range of genres may indicate different engagement behaviour.

The project investigates whether users with higher content diversity show different retention or inactivity patterns.

---

# ⚠️ Early Signs of Declining Engagement

The project identifies behavioural indicators that may occur before users become inactive.

Potential indicators include:

- Decreasing session duration
- Increasing inactivity period
- Low content diversity
- Reduced viewing frequency
- Persistent low engagement
- Differences across subscription plans

The final notebook should report the indicators actually supported by the dataset.

---

# 💳 Subscription Plan Comparison

User behaviour is compared across subscription plans.

Possible comparison metrics:

| Metric | Plan A | Plan B | Plan C |
|---|---:|---:|---:|
| Average Session Duration | — | — | — |
| Average Inactivity | — | — | — |
| Content Diversity | — | — | — |
| Retention Rate | — | — | — |

The actual values should be generated from the Colab notebook.

---

# 📈 Visualizations

The project contains at least **4 important visualizations**.

### 1. Average Session Duration by Subscription Plan

Shows differences in viewing engagement between subscription plans.

### 2. Content Diversity vs Retention

Examines whether users who watch a wider range of genres have different retention outcomes.

### 3. Inactivity Period Distribution

Shows the distribution of inactivity periods and helps identify potentially at-risk users.

### 4. Session Duration by Retention Status

Compares engagement between retained and non-retained users.

---

# 🤖 Machine Learning

## Algorithm: Random Forest

The specified machine-learning algorithm is **Random Forest**.

Random Forest is used to build a prediction model for the challenge's defined target.

The model can use features such as:

```text
Session_Duration
Content_Genre
Subscription_Plan
Inactivity_Period
Content_Diversity
Engagement_Score
```

The target variable is:

```text
Retention_Status
```

---

# 🌲 Random Forest Workflow

```text
Raw OTT Dataset
       ↓
Data Cleaning
       ↓
Feature Engineering
       ↓
Exploratory Data Analysis
       ↓
Feature Encoding
       ↓
Train / Test Split
       ↓
Random Forest
       ↓
Prediction
       ↓
Model Evaluation
       ↓
Behavioural Insights
```

---

# 📏 Model Evaluation

For a classification problem, the Random Forest model can be evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- ROC-AUC, where appropriate

Example output:

```text
Accuracy  : XX.XX%
Precision : XX.XX%
Recall    : XX.XX%
F1 Score  : XX.XX%
```

The actual values should be replaced with the results produced by the Colab notebook.

---

# 🔎 Key Insights

The final project should provide **5–7 evidence-based insights**.

Examples of insight categories:

### Insight 1 — Viewing Behaviour

Identify the major user viewing patterns and engagement groups.

### Insight 2 — Session Duration

Determine whether users with longer sessions show different retention behaviour.

### Insight 3 — Content Diversity

Examine whether users who watch multiple genres have different engagement or retention patterns.

### Insight 4 — Inactivity

Identify inactivity levels associated with declining engagement.

### Insight 5 — Subscription Plans

Compare engagement and retention across subscription plans.

### Insight 6 — Early Warning Signals

Identify behavioural patterns that may indicate users are moving toward inactivity.

### Insight 7 — Prediction

Identify which behavioural features are important for the Random Forest prediction task.

> Replace these examples with the actual findings obtained from the dataset.

---

# 💡 Practical Action Plan

Based on the behavioural analysis, an OTT platform can consider:

### 1. Early Engagement Alerts

Identify users showing increasing inactivity or decreasing session duration.

### 2. Personalized Recommendations

Recommend content based on each user's viewing history and genre preferences.

### 3. Content Diversity

Introduce users to relevant content from additional genres when appropriate.

### 4. Subscription Plan Analysis

Use engagement and retention patterns to understand differences between plans.

### 5. Re-Engagement Campaigns

Send personalized recommendations or reminders to users showing early signs of declining engagement.

### 6. Continuous Monitoring

Create an engagement-monitoring pipeline that tracks session duration, inactivity and content diversity.

---

# 🧰 Technologies Used

### Programming Language

- Python

### Libraries

```text
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
```

### Machine Learning

```text
Random Forest
```

### Development Environment

```text
Google Colab
Jupyter Notebook
Python
```

---

# 📁 Project Structure

```text
DS_Day01_41_OTT_User_Engagement/
│
├── data/
│   └── ott_user_behavior.csv
│
├── notebooks/
│   └── ott_user_engagement_analysis.ipynb
│
├── visualizations/
│   ├── session_duration_by_plan.png
│   ├── content_diversity_retention.png
│   ├── inactivity_distribution.png
│   └── session_duration_retention.png
│
├── models/
│   └── random_forest_model.pkl
│
├── README.md
│
└── requirements.txt
```

---

# ⚙️ Running the Project in Google Colab

1. Open the notebook in Google Colab.
2. Upload `ott_user_behavior.csv`.
3. Run the cells from top to bottom.
4. Perform data cleaning and validation.
5. Run the EDA section.
6. Generate the four visualizations.
7. Perform behavioural analysis.
8. Train the Random Forest model.
9. Evaluate the model.
10. Record the final 5–7 insights.

---

# 📦 Requirements

The project requires:

```text
pandas
numpy
matplotlib
seaborn
scikit-learn
```

Install them in Colab if necessary:

```python
!pip install pandas numpy matplotlib seaborn scikit-learn
```

---

# 🎯 Expected Output

The completed project provides:

- ✅ Cleaned and validated OTT dataset
- ✅ Exploratory Data Analysis
- ✅ Behavioural segmentation
- ✅ Average watch-time analysis
- ✅ Content-diversity analysis
- ✅ Early declining-engagement analysis
- ✅ Subscription-plan comparison
- ✅ 4 visualizations
- ✅ 5–7 key insights
- ✅ Trained Random Forest model
- ✅ Model evaluation results
- ✅ Practical OTT engagement strategy

---

# 🏆 Project Outcome

This project demonstrates how **Data Science and Machine Learning can be used to understand customer behaviour in the Streaming and OTT industry**.

The overall analysis follows:

```text
User Behaviour
      ↓
Engagement Analysis
      ↓
Content Diversity
      ↓
Inactivity Detection
      ↓
Retention Analysis
      ↓
Random Forest Prediction
      ↓
Business Action Plan
```

The goal is not only to predict retention, but to understand **why users become less engaged and what behavioural signals appear before disengagement**.

---

# 👨‍💻 Author

**Nithen Sakthi**

Data Science Project  
**DS_Day01_41 — OTT: Why Do Users Stop Watching?**

---

# ⭐ Project Keywords

```text
Data Science
OTT Analytics
Streaming Analytics
User Behaviour Analysis
Customer Segmentation
User Engagement
Content Diversity
Customer Retention
Churn Analysis
Inactivity Analysis
Random Forest
Machine Learning
Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn
```

---

## 📜 License

This project is created for educational and academic purposes.
