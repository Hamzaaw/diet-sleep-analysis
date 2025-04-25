# Diet & Sleep Study: Analyzing the Relationship Between Nutrition and Sleep Quality

## Project Overview
This project explores the relationship between dietary habits and sleep quality. Using three months of self-tracked diet data from MyFitnessPal and sleep data from a smartwatch, I analyze how factors such as macronutrient intake (protein, fiber, carbohydrates, fats) influence total sleep duration and sleep stages (REM, deep sleep, light sleep).

The primary goal is to uncover patterns and test hypotheses regarding how different foods affect sleep quality. The study focuses only on days when I woke up naturally (without an alarm) to eliminate external disruptions. By applying data science techniques, I determine whether specific dietary habits correlate with improved or worsened sleep quality.

---

## Motivation

**Why This Project?**  
- **Personal Relevance:** Sleep quality is crucial for overall health, especially for individuals with autoimmune disorders. Poor sleep can exacerbate inflammation and trigger flare-ups. Understanding how my diet impacts sleep will help me optimize both health and immune regulation.  
- **Scientific Curiosity:** While studies suggest nutrition affects sleep, I want to see if these trends hold for my own body.  
- **Data Science Application:** This project allows me to apply statistical analysis, hypothesis testing, and machine learning to real-world personal data.

---

## Data Source & Collection

### Diet Data (MyFitnessPal Logs)
- **Columns:**  
  - Date  
  - Calories Consumed (kcal)  
  - Macronutrient Breakdown (Carbohydrates, Protein, Fat)  
  - Fiber Intake (g)  
  - Sugar Intake (g)  
  - Last Meal Hour (24h clock)

### Sleep Data (Smartwatch Logs)
- **Columns:**  
  - Date  
  - Total Sleep Duration (hrs)  
  - Sleep Efficiency (% of time asleep in bed)  
  - Deep Sleep (%)  
  - REM Sleep (%)  
  - Light Sleep (%)  
  - Resting Heart Rate (bpm)  
  - Natural Wakeup (Boolean)

---

## Data Cleaning & Preprocessing
- Remove days with missing sleep data.  
- Filter out days with alarm-based wake-ups (keep only natural wake-up days).  
- Convert meal timing into **Hours Before Sleep** (time between last meal and bedtime).  
- Normalize nutrient intake to account for varying total calories:
  - **Fiber per 1000 kcal** = Fiber (g) / (Calories / 1000)  
  - **Protein per 1000 kcal** = Protein (g) / (Calories / 1000)  

---

## Exploratory Data Analysis (EDA)
1. **Merge** diet and sleep datasets on `Date`.  
2. **Filter** for natural wake-up days only.  
3. **Feature creation**:  
   - Hours Before Sleep  
   - Fiber per 1000 kcal  
   - Protein per 1000 kcal  
4. **Visualizations & Insights**:  
   - Time series plots of sleep metrics vs. dietary factors.  
   - Correlation heatmap (including normalized features).  
   - Boxplots (e.g., deep sleep % by high vs. low fiber).  
   - Scatter plots (e.g., Hours Before Sleep vs. Sleep Efficiency).

---

## Hypothesis Testing
1. **Fiber intake → Deep Sleep %**  
   - Test: Mann-Whitney U (one-tailed)  
2. **Hours Before Sleep → Sleep Efficiency %**  
   - Test: Spearman rank correlation  
3. **Protein intake → REM Sleep %**  
   - Test: Spearman rank correlation  

Each test includes statistical results, boxplots or scatter + regression line, and clear interpretation.

---

## Machine Learning (ML) Methods
- **Regression Analysis**: Predict sleep efficiency or deep sleep % from dietary and timing features.  
- **Clustering Analysis**: Identify patterns/groups (e.g., “High Protein, Poor Sleep” vs. “Balanced Diet, Good Sleep”).  

---

## Limitations & Future Work
**Challenges:**  
- Confounding variables (stress, exercise, screen time) may influence sleep.  
- Limited sample size (personal data only).  
- Missing data on some days requiring imputation.  

**Future Directions:**  
- Incorporate additional lifestyle data (e.g., stress levels, physical activity).  
- Compare personal findings with public sleep datasets for validation.  
- Extend the study to 6–12 months for more robust conclusions.  

---

## Tools & Technologies
- **Python:** pandas, NumPy, matplotlib, seaborn, scikit-learn, scipy  
- **Jupyter Notebook:** Exploratory analysis & hypothesis testing  
- **GitHub:** Version control & project tracking  

---

## Project Timeline

| Date        | Milestone                                           |
|-------------|-----------------------------------------------------|
| **March 10** | Submit project proposal (GitHub README)            |
| **April 18** | Collect data & conduct exploratory data analysis   |
| **April 25** | Submit enriched EDA + hypothesis testing           |
| **May 23**   | Apply machine learning models                      |
| **May 30**   | Final project submission (report/video/webpage)    |

---

## Conclusion
This project provides actionable insights into how diet influences sleep quality. By combining personal tracking with data science techniques—EDA, statistical testing, and ML—I aim to uncover meaningful patterns to optimize nutrition and sleep habits. The findings will also contribute to a broader understanding of diet-sleep interactions in health research.
