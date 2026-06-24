<img width="1352" height="601" alt="Screenshot 2026-06-22 213324" src="https://github.com/user-attachments/assets/67c33991-4de1-423d-a459-c28faf7c687b" /># HR Employee Attrition Analysis

## Project Overview
This repository contains the **HR Employee Attrition Analysis** project developed as part of the **Naan Mudhalvan Arts Internship Program 2026** in collaboration with AdroIT Technologies, Innovative Solutions Pvt Ltd, and Oracle University.

The primary objective of this project is to perform an **Exploratory Data Analysis (EDA)** on an HR Employee dataset (`HRR.csv`) to identify the core factors influencing employee turnover (attrition). Using data-driven insights, this analysis provides actionable recommendations to help HR managers enhance employee retention and workplace satisfaction.

---

## Student Profile
* **Student Name:** M.Muthulakshmi
* **Academic Year:** 2026-2027
* **Department:** BSc Computer Science (Semester IV)
* **Roll No:** 24081091802112117
* **NMID:** 2ff24138b0a13c08f704036f2e02f2a1@nm2026.in
* **College Code:** 109
* **College Name:** Manonmaniam Sundaranar University College, Govindaperi

---

## Problem Statement
High employee turnover (attrition) leads to significant financial and operational losses for organizations. Companies often struggle to pinpoint the hidden reasons behind employee resignations. This project leverages systematic data analysis to uncover underlying workplace patterns—such as salary structures (DailyRate) and business travel frequencies—that push employees to quit, allowing management to make informed policy adjustments.

---

## Objectives
1. Analyze the corporate employee database to uncover the roots of employee attrition.
2. Apply Python aggregation techniques (`groupby`, `min`, `max`, `mean`) to evaluate corporate metrics.
3. Sort and identify high-value and low-value salary brackets across different company departments.
4. Provide data-driven insights to improve workforce retention.

---

## Technologies Used
* **Development Environment:** Google Colab
* **Programming Language:** Python
* **Libraries Used:**
  * **Pandas:** Data loading, dataframe manipulation, row filtering, and `groupby` summaries.
  * **NumPy:** Vectorized numerical operations and handling structural null value statistics.
  * **Matplotlib & Seaborn:** Generating clear exploratory data plots (Bar charts, Pie charts, Histograms, and Countplots).

---

## Project Application Flow
1. **Load Dataset:** Read local `HRR.csv` via Pandas `pd.read_csv()`.
2. **Data Profiling:** Inspect structures using `.info()` and locate missing fields via `.isnull().sum()`.
3. **Statistical Summary:** Extract central indicators with `.describe()` and custom multi-level `.groupby()` aggregations.
4. **Data Sorting:** Isolate trend extremes using `.sort_values()` for both salary heights and lows.
5. **Data Visualization:** Render graphical assets to establish final business metrics.

---

## Expected Output & Execution Results

### 1. Data Analysis Outputs
Below are the key execution data values generated directly from the Google Colab Notebook data summary steps:

#### A. Descriptive Statistical Analysis (`Age` & `DailyRate` by Attrition)
```text
Age Stats grouped by Attribution:
   Attribution  min  max       mean  count
0           No   21   59  35.869565     23
1          Yes   28   41  34.666667      6

DailyRate Stats grouped by Attribution:
   Attribution  min   max        mean
0           No  153  1392  817.869565
1          Yes  103  1373  936.666667
### B.SORTING HIGHEST LOWEST DAILY RATE ETRICS
Top 5 Highest Revenue Earning Employees:
    EmployeeNumber  Age               Department  DailyRate
5               33   37  Research & Development       1392
15              28   29  Research & Development       1389
2                4   37  Research & Development       1373
7               11   38  Research & Development       1358
13              18   34  Research & Development       1346

Top 5 Lowest Revenue Earning Employees:
    EmployeeNumber  Age               Department  DailyRate
14              19   28  Research & Development        103
11              15   29  Research & Development        153
12              16   38  Research & Development        216
1                2   49  Research & Development        279
16              21   32  Research & Development        334
###  Department-Wise Average Daily RatE
Department Average Daily Rate
Sales 1057.58
Research & Development 888.64
### Graphical Reports Summary
​The analysis script successfully renders the following data visualization charts:
​BAR CHART: Visualizes that the Sales department holds a higher average daily rate compared to Research & Development.
​Pie Chart (Overall Employee Attribution Percentage): Confirms an employee status distribution showing 79.3% No (Retained) and 20.7% Yes (Attributed).
​Histogram Chart: Captures the age variance showing high cluster densities around the 30-35 age bracket.
​Count Plot: Maps employee educational distribution, demonstrating a higher concentration in Life Sciences and Medical fields.
​###Challenges Faced & Learning Outcomes
​Challenges Faced
​Column Name Mismatch Error: Encountered a KeyError inside Python when trying to reference the target column index because of a slight typographical mismatch error between the terms Attrition and Attribution.
​Resolution: Corrected by utilizing .info() to carefully review the dataframe structural schema parameters and adjusting dictionary definitions to map the exact string keyword index Attribution.
​###Learning Outcomes
​Technical Proficiency: Gained strong hands-on experience in Pandas for advanced indexing, multi-level calculations, categorical data summaries, and Google Colab execution environments.
​Practical Experience: Learned to dissect raw business data variables, identify operational corporate issues, and turn numerical metrics into valuable HR retention models.
