# DSA210-Project

## **Project Proposal**
In this term project, I will analyze how daily technology use, including social media and screen time, affects mental health indicators like stress, sleep quality, and productivity. Using a dataset from Kaggle, the goal is to explore the link between digital habits and mental well-being, promoting healthier screen time management. Excessive screen time and frequent social media use are expected to increase stress and decrease sleep quality, reducing productivity. The analysis will help identify trends for further research and predictive modeling on technology’s impact on mental health.

---
## **Motivation**
With increasing technology use, particularly social media and screen time, understanding its impact on mental health is crucial. By analyzing the Kaggle dataset, I aim to:

- Explore how technology use affects stress, sleep, and productivity.
- Identify trends in mental well-being across usage patterns.
- Provide insights into how screen time management can improve mental health.

---
## **Focus of the Study**
This study focuses on analyzing the impact of daily technology usage, including social media and screen time, on mental health indicators like stress, sleep quality, and productivity. The goal is to understand how digital habits influence well-being and identify trends that could help in managing screen time for improved mental health.

---
## **Data Set and Processing**
#### **1)Data Source**

The dataset used for this project was sourced from Kaggle. It contains data related to daily technology usage and mental health indicators, including self-reported scores for stress, sleep quality, and mental health. The data was collected through surveys and tracking apps that monitor screen time and mental health factors, allowing a comprehensive look at digital habits and well-being.
#### **2)Data Set**
The dataset includes data points that track an individual's daily use of technology and mental health factors. The following items are included:

- **User_ID**: A unique identifier for each participant.
- **Age**: The age of the participant.
- **Daily_Screen_Time (hours)** : Average daily screen time in hours.
- **Mental_Health_Score (1-10)**: Self-reported mental health score, where 1 is poor, and 10 is excellent.
- **Stress_Level (1-10)**: Self-reported stress level, where 1 is very low, and 10 is very high.
- **Sleep_Quality (1-10)**: Self-reported sleep quality score.
 #### **3)Data Preprocessing** 
 - The data will be processed to resolve inconsistencies and eliminate outliers.
---

## **Data Analysis Plan**
#### **Data Preprocessing**
- Inconsistencies and outliers in the data will be cleaned.
  
#### **Exploratory Data Analysis (EDA)**
- The distributions of screen time, stress levels, sleep quality, and productivity will be analyzed.
- Key trends and patterns in these variables will be visualized.
  
#### **Correlation Analysis**
- The relationships between screen time and stress, sleep quality, and productivity will be examined.
- Pearson or Spearman correlation coefficients will be calculated.
  
#### **Univariate Analysis**
- Explore frequency and distribution of each variable (e.g., histograms).

#### **Bivariate Analysis**

- Scatter plots and boxplots to identify relationships between two variables.

#### **Multivariate Analysis**

- Heatmap of correlations among variables.

#### **Regression Modeling**

- Apply regression to predict sleep hours based on screen time.

#### **Machine Learning Evaluation**

- Evaluate model performance using MSE and R².

- Use confusion matrix for sleep range predictions.

---
## **Hypotheses**

#### **1)Null Hypothesis (H₀):**
There is no significant relationship between screen time and stress or sleep duration.

#### **2)Alternative Hypothesis (H₁):**
Screen time significantly impacts stress levels and sleep quality.

---

## **Findings**
In this project, I expect to find:

- A correlation between high screen time and increased stress levels, as well as lower sleep quality.
- Possible negative effects of excessive social media use on productivity.
- Key trends linking specific usage patterns to mental well-being, helping to identify optimal screen time management strategies.
- Insights into how reducing screen time might improve productivity and overall mental health.

## **Analysis Results**

#### **1)Univariate Insights:**

- Most users report 2–6 hours of daily technology use.
- Average sleep is ~6.3 hours.
- Majority of stress levels are in the "Medium" category.

#### **2)Correlation & Regression:**

- Weak or no statistically significant correlation between screen time and sleep (r ≈ -0.01, p > 0.05).
- OLS Regression showed no predictive power (R² ≈ 0.00, p = 0.26).

#### **3)Group Analysis:**

- Medium stress level users had highest average tech use.
- Low stress associated with higher physical activity.
  
#### **4)Machine Learning:**

- Model	MSE	R² Score
- Linear Regression	2.11	Very Low
- ML models confirmed screen time is a weak predictor of sleep duration.
- Confusion matrix showed moderate classification accuracy for central sleep ranges (4–6 hrs).
  
  |**Model**                |**Mean Squared Error(MSE)**   	|**R^2**      |
  |-------------------------|-----------------------------------|-------------|
  |Linear Regression        | 2.11			| Very Low       |

---

## **Limitations**

**Screen Time Data**:The screen time data was taken from device tracking, but it might miss some screen usage (like certain apps or settings).

**Sample Size**:Data was collected for just one month, so it's hard to make conclusions for longer periods.

**Self-Reported Data**:Productivity was self-reported, which could be biased or inaccurate.

## **Future Work**
- Use automatic data collection for more accurate tracking of screen time, stress, sleep, and productivity over time.

- Collect data over several months for better and more reliable results.

- Look into other factors, like how different apps or activities (e.g., social media, gaming) affect mental health.
---

## **Conclusion**
- We fail to reject the null hypothesis as the p-values are > 0.05. There is no statistically significant relationship between screen time and sleep duration. However, exploratory trends suggest that users with medium stress use more technology, and lower stress is associated with higher physical activity.
- This project highlights the importance of monitoring and managing screen time as part of a broader wellness strategy.
- Further data collection and refined feature engineering can help uncover deeper insights into how digital habits influence mental health.
---

