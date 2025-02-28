# Heart Attack Prediction - Exploratory Data Analysis (EDA)

## Overview

This project performs exploratory data analysis (EDA) on the **Heart Attack Prediction in India** dataset. The goal is to analyze various health parameters and identify potential patterns or risk factors associated with heart attacks.

## Dataset

- **File Name:** `heart_attack_prediction_india.csv`
- **Source:** [Provide source if available]
- **Description:** The dataset contains medical and demographic information of patients, which helps in analyzing factors contributing to heart attacks.

### Features (Columns)

- `Patient_ID` (Dropped) - Unique identifier for each patient.
- Other relevant health indicators (to be detailed further based on dataset).

## Preprocessing

- Removed `Patient_ID` as it does not contribute to analysis.
- Additional cleaning steps will be documented as the project progresses.

## Steps Performed in EDA

1. **Data Loading** - Read the dataset using Pandas.
2. **Data Cleaning** - Dropped unnecessary columns.
3. **Exploratory Analysis**:
   - Displayed first few rows using `.head()`.
   - Identified missing values (if any).
   - Checked dataset structure and data types using `.info()`.
   - Generated summary statistics using `.describe()`.
   - Calculated the percentage of patients at risk for a heart attack.
   - Analyzed heart attack risk by state and visualized the top 10 states with the highest risk using a bar plot.
   - Analyzed heart attack risk by gender and visualized the results using a bar chart.
   - Analyzed heart attack risk based on **previous heart attack history** and visualized the results using a bar chart.
   - Analyzed heart attack risk based on **diabetes status** and visualized the results using a bar chart.
   - Analyzed heart attack risk based on **hypertension status** and visualized the results using a bar chart.
   - Analyzed heart attack risk based on **obesity status** and visualized the results using a bar chart.
   - Analyzed heart attack risk based on **smoking habits** and visualized the results using a bar chart.
   - Analyzed heart attack risk based on **physical activity** and visualized the results using a bar chart.
     - Identified potential **outliers**, as results indicate that people who exercise regularly still show a higher risk of heart attack.
     - Further investigation is required to determine if other confounding factors are influencing this trend.
   - Analyzed heart attack risk based on **stress levels** and visualized the results using a count plot.
     - Helps understand the correlation between stress and heart attack risk.
   - Analyzed heart attack risk based on **air pollution exposure** and visualized the results using a bar chart.
     - Helps identify how environmental factors like air quality contribute to heart attack risk.
   - Analyzed **distribution of numerical variables** using histograms with KDE plots.
     - Visualized the distribution of key numerical features such as Age, Cholesterol Level, Blood Pressure, Diet Score, Stress Level, etc.
     - Helps in understanding the distribution, skewness, and presence of potential outliers in key numerical features.
     - Insights from distributions:
       - **Age distribution**: Detecting normality or skewness.
       - **Cholesterol and lipid levels**: Identifying extreme values that may impact heart health.
       - **Annual income**: Understanding its impact on health factors.
       - **Stress Level**: Checking if it's normally distributed or skewed towards high values.
   - **Age Group Analysis**:
     - Divided age into bins (`0-20`, `21-30`, `31-40`, `41-50`, `51-60`, `61-70`, `71-80`).
     - Calculated the average heart attack risk for each age group.
     - Visualized heart attack risk across different age groups using a bar plot.
     - Helps in understanding how age impacts the likelihood of a heart attack.
   - **Correlation Analysis**:
     - Computed the correlation matrix for numerical variables in the dataset.
     - Excluded categorical variables like `State_Name` and `Gender`.
     - Visualized the correlation matrix using a heatmap.
     - Helps identify relationships between key health indicators and heart attack risk.
   - **Pair Plot for Key Variables**:
     - Selected key variables (`Age`, `Cholesterol_Level`, `Systolic_BP`, `Heart_Attack_Risk`).
     - Created a pair plot to visualize relationships and distributions between these variables.
     - Differentiated between heart attack risk groups using color coding.

## Tools & Libraries Used

- Python
- Pandas
- NumPy
- Seaborn
- Matplotlib
- Jupyter Notebook

## Future Work

- Perform statistical analysis on key health indicators.
- Visualize relationships between features using plots.
- Identify and handle potential outliers in physical activity data.
- Analyze deeper correlations between stress levels, air pollution, and heart attack risk.
- Build a predictive model for heart attack risk assessment.

## How to Run

1. Install dependencies:
   ```bash
   pip install pandas numpy seaborn matplotlib jupyter
   ```
2. Open the Jupyter Notebook and execute the code cells sequentially.

## Contributors

- Tanishq Sharma-23112104

