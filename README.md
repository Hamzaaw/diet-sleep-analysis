# **Diet & Sleep Study: Analyzing the Relationship Between Nutrition and Sleep Quality**

## **Project Overview**

This project explores the relationship between dietary habits and sleep quality. Using three months of self-tracked **diet data from MyFitnessPal** and **sleep data from a smartwatch**, I will analyze how factors such as macronutrient intake (protein, fiber, carbohydrates, fats) influence **total sleep duration and sleep stages (REM, deep sleep, light sleep).**

The primary goal is to uncover patterns and test hypotheses regarding **how different foods affect sleep quality**. The study will focus only on **days when I woke up naturally (without an alarm)** to eliminate external disruptions. By applying data science techniques, I will determine whether specific dietary habits correlate with improved or worsened sleep quality.

## **Motivation**

### **Why This Project?**

- **Personal Relevance:** Sleep quality is crucial for overall health, and it is even more critical for individuals like me who have an **autoimmune disorder**. Poor sleep can exacerbate inflammation, weaken immune function, and trigger flare-ups. Understanding how my diet impacts my sleep will help me optimize both health and immune regulation, contributing to better symptom management and overall well-being.
- **Scientific Curiosity:** While studies suggest **nutrition affects sleep**, I want to see if these trends hold **for my own body**.
- **Data Science Application:** This project allows me to apply **statistical analysis, hypothesis testing, and machine learning** to real-world personal data.

## **Data Source & Collection**

### **Dataset**

I will use two primary data sources:

1. **Diet Data (MyFitnessPal Logs)**

   - **Calories Consumed (kcal)**
   - **Macronutrient Breakdown** (Carbohydrates, Protein, Fat)
   - **Fiber Intake (grams)**
   - **Meal Timing** (time of last meal)
   - **Sugar Intake (grams)**

2. **Sleep Data (Smartwatch Logs)**

   - **Total Sleep Duration (hours)**
   - **Sleep Efficiency (% of time asleep while in bed)**
   - **Deep Sleep Percentage (%)**
   - **REM Sleep Percentage (%)**
   - **Resting Heart Rate During Sleep**

### **Data Cleaning & Preprocessing**

- Remove **days with missing sleep data**.
- Filter out **days where I used an alarm** (only include natural wake-up days).
- Standardize timestamps and convert meal timing into useful metrics (e.g., “Hours Before Sleep”).
- Normalize macronutrient intake based on total calories to account for daily variation.

## **Exploratory Data Analysis (EDA)**

### **Visualizations & Insights**

- **Time Series Analysis:** Sleep trends over time in response to dietary changes.
- **Correlation Heatmap:** How strongly different dietary factors correlate with sleep quality.
- **Boxplots:** Comparing macronutrient intake between **good sleep** vs. **poor sleep** nights.
- **Scatter Plots:** Exploring relationships like **fiber intake vs. deep sleep percentage**.

## **Hypothesis Testing**

I will conduct statistical tests to determine significant relationships, including:

1. **Does high fiber intake improve deep sleep?**

   - *Null Hypothesis (H₀):* Fiber intake has no effect on deep sleep.
   - *Alternative Hypothesis (H₁):* Higher fiber intake increases deep sleep percentage.
   - *Test Method:* Mann-Whitney U test.

2. **Does consuming more calories earlier in the day improve sleep efficiency?**

   - *Null Hypothesis (H₀):* Meal timing has no effect on sleep efficiency.
   - *Alternative Hypothesis (H₁):* Eating earlier leads to better sleep.
   - *Test Method:* Linear regression.

## **Machine Learning (ML) Methods**

To extend the analysis, I will apply basic ML models:

1. **Regression Analysis:** Predict **sleep quality scores** based on dietary factors.
2. **Clustering Analysis:** Identify groups with **distinct diet-sleep patterns** (e.g., “High Protein, Poor Sleep” vs. “Balanced Diet, Good Sleep”).

## **Limitations & Future Work**

### **Challenges:**

- **Confounding Variables:** External factors like stress and exercise could influence sleep.
- **Sample Size:** The dataset is limited to my personal data (not generalizable to all populations).
- **Missing Data:** Some days might lack complete tracking, requiring imputation methods.

### **Future Work:**

- Compare personal findings with **public sleep datasets** to validate trends.
- Incorporate additional lifestyle factors (e.g., **stress, physical activity**).
- Run an extended study over **6-12 months** for more robust conclusions.

## **Tools & Technologies**

- **Python (pandas, NumPy, seaborn, matplotlib, scikit-learn)** for data analysis and visualization.
- **Jupyter Notebook** for exploratory data analysis and modeling.
- **GitHub** for version control and project tracking.

## **Project Timeline**

| Date         | Milestone                                              |
| ------------ | ------------------------------------------------------ |
| **March 10** | Submit project proposal (GitHub README)                |
| **April 18** | Collect data & conduct exploratory data analysis (EDA) |
| **May 23**   | Apply machine learning models                          |
| **May 30**   | Final submission                                       |

## **Conclusion**

This project will provide actionable insights on how diet influences sleep quality. By combining **personal tracking with data science techniques**, I aim to uncover meaningful patterns that could optimize **both my nutrition and sleep habits**. The findings will also contribute to a broader understanding of **diet-sleep interactions** in the field of health and wellness research.

