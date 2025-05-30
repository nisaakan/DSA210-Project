# DSA210-Project

## **Project Proposal**
In this term project, I will analyze how daily technology use, including social media and screen time, affects mental health indicators like stress, sleep quality, and productivity.
- Using a dataset from Kaggle, the goal is to explore the link between digital habits and mental well-being, promoting healthier screen time management.
- Excessive screen time and frequent social media use are expected to increase stress and decrease sleep quality, reducing productivity. The analysis will help identify trends for further research and predictive modeling on technology’s impact on mental health.

---
## **Motivation**
With increasing technology use, particularly social media and screen time, understanding its impact on mental health is crucial. By analyzing the Kaggle dataset, I aim to:

- Explore how technology use affects stress, sleep, and productivity.
- Identify trends in mental well-being across usage patterns.
- Provide insights into how screen time management can improve mental health.

---
## **Focus of the Study**
- This study focuses on analyzing the impact of daily technology usage, including social media and screen time, on mental health indicators like stress, sleep quality, and productivity.
- The goal is to understand how digital habits influence well-being and identify trends that could help in managing screen time for improved mental health.

---
## **Task Definition**
This project is framed as a supervised machine learning task:
- **“Predict High_Stress (Stress_Level == 'High') using screen time and related behavioral features.”**
- This binary classification task is addressed using tree-based ML models, and regression models are used to analyze relationships with sleep duration.
---

## **Data Set and Processing**
#### **1)Data Source**
The dataset used for this project was sourced from Kaggle.

- It contains data related to daily technology usage and mental health indicators, including self-reported scores for stress, sleep quality, and mental health.
- The data was collected through surveys and tracking apps that monitor screen time and mental health factors, allowing a comprehensive look at digital habits and well-being.

#### **2)Data Set**
The dataset includes data points that track an individual's daily use of technology and mental health factors. The following items are included:

- **User_ID**: A unique identifier for each participant.
- **Age**: The age of the participant.
- **Screen_Time_Hours**: Total average screen usage in hours.
- **Mental_Health_Status**: Categorical rating (Excellent, Good, Fair, Poor).
- **Stress_Level**: Categorical (Low, Medium, High).
- **Sleep_Hours**: Average sleep duration in hours.
  
 #### **3)Data Preprocessing** 
 The data will be processed to resolve inconsistencies and eliminate outliers.
 
---

## **Feature Engineering**

- **ScreenTime_Level**: Categorized into Low (<2h), Medium (2–6h), and High (>6h).
- **High_Stress**: Binary flag (1 if Stress_Level == 'High', else 0).
- **ScreenTime_to_Sleep**: Ratio of screen time to sleep hours.
- **Stress_Level_Numeric**: Converted stress categories into numeric format (Low=1, Medium=2, High=3).
- **Dummy Encodings**: Categorical variables (Gender, Mental Health Status, Online Support, etc.) were one-hot encoded to be used in models.
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

- Scatterplots and boxplots to identify relationships between two variables.

#### **Multivariate Analysis**

- Heatmap of correlations among variables.

#### **Regression Modeling**

- Apply regression to predict sleep hours based on screen time.

#### **Machine Learning Evaluation**

- Evaluate model performance using MSE and R².

- Use confusion matrix for sleep range predictions.

---

## **Final Report Of The Project**

## **Introduction**
- This project investigates the relationship between technology usage and mental well-being.
- The core objective is to determine whether variables such as screen time, gaming hours, and social media usage significantly affect stress levels and sleep quality. By applying statistical and machine learning techniques, this study attempts to model and predict stress and sleep outcomes from digital usage behavior.

## **Hypothesis**
#### **1)Null Hypothesis (H₀):**
- There is no correlation between screen time sleep hours.
#### **2)Alternative Hypothesis (H₁):**
- There is a correlation between screen time and sleep hours.
  
## **Methods**

#### **Dataset and Collection**
- Data sourced from Kaggle: “Mental Health and Technology Usage 2024”
- Includes features like screen time, sleep duration, physical activity, technology usage, and stress level.

#### **Data Processing**

- Cleaned and standardized numeric values.
- Outliers handled via IQR method.
- Missing values filled using mean (numerical) or mode (categorical).
- Feature engineering added variables like ScreenTime_to_Sleep, High_Stress, and Avg_Tech_Screen.
- One-hot encoding applied to categorical features.

#### **Exploratory Data Analysis(EDA)**

- Users reported an average of ~6.5 hours of sleep and 2–6 hours of screen time.
- Most stress levels were in the "Medium" category.
- Higher screen time and lower physical activity were associated with higher stress.

#### **Statistical Tests**

- Pearson correlation between screen time and sleep: r ≈ -0.01, p > 0.05 → No significant relationship.
- Pearson correlation between screen time and stress level: r ≈ +0.12, p < 0.05 → Weak but significant positive correlation.
- OLS Regression showed screen time alone has no predictive power for sleep (R² ≈ 0.00, p = 0.26).

#### **Visualization**

## **Analysis Results**

#### **1)Univariate Insights:**

- Most users report 2–6 hours of daily technology use.
- Average sleep is ~6.5 hours.
- Majority of stress levels are in the "Medium" category.

#### **2)Correlation & Regression:**

- Weak or no statistically significant correlation between screen time and sleep (r ≈ -0.01, p > 0.05).
- OLS Regression showed no predictive power (R² ≈ 0.00, p = 0.26).

#### **3)Group Analysis:**

- Medium stress level users had highest average tech use.
- Low stress associated with higher physical activity.
  
#### **4)Machine Learning:**

#### Machine Learning Models:
-  Decision tree and random forest models are used instead of relying solely on linear regression. These models are suitable for classification and regression tasks and perform better with non-linear patterns present in behavioral data.
- ML models confirmed screen time is a weak predictor of sleep duration.
- Confusion matrix showed moderate classification accuracy for central sleep ranges (4–6 hrs).
- Multi-dimensional features may be necessary for accurate mental health prediction.
- Model	MSE	R² Score
- Linear Regression	0.61 Low

 | **Model**         |**R^2**   | **Mean Squared Error(MSE)**  |
 |-------------------|----------|--------------------|
 | Random Forest     | -0.03     | Lower        |
 | Decision Tree     | -0.90     | Higher             |

---

## **Findings**


## **Limitations**

**Screen Time Data**:The screen time data was taken from device tracking, but it might miss some screen usage (like certain apps or settings).

**Sample Size**:Data was collected for just one month, so it's hard to make conclusions for longer periods.

**Self-Reported Data**:Productivity was self-reported, which could be biased or inaccurate.

**Self-Reported Variables**: Stress and mental health status are subjective and may introduce personal bias.


## **Future Work**
- Use automatic data collection for more accurate tracking of screen time, stress, sleep, and productivity over time.

- Collect data over several months for better and more reliable results.

- Look into other factors, like how different apps or activities (e.g., social media, gaming) affect mental health.
---

## **Conclusion**
#### **Pearson correlation:**
- A Pearson correlation test between screen time and sleep hours returned r ≈ -0.01 and p > 0.05.
- Therefore, we **fail to reject the null hypothesis**, indicating no significant linear relationship between these variables.
  
#### **Hypothesis Test:**
- We fail to reject the null hypothesis as the p-values are > 0.05. There is no statistically significant relationship between screen time and sleep duration. However, exploratory trends suggest that users with medium stress use more technology, and lower stress is associated with higher physical activity.

#### **Overall Insights:**
This study demonstrates how machine learning techniques can be used to uncover behavioral patterns related to stress. While screen time alone is not a strong predictor of sleep quality, incorporating additional variables such as physical activity, age, and technology usage improves the explanatory power of predictive models.

- The project underscores the value of tracking digital habits and using data-driven methods to support mental wellness.
- With expanded data collection and more advanced feature engineering, future studies can deliver deeper insights into how digital behavior influences mental health outcomes.
  
---

