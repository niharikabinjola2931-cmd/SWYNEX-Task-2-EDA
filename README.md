# Hospital Readmission Analytics – Exploratory Data Analysis

## Project Overview

This project was completed as part of the SWYNEX Technologies Data Analyst Internship – Task 2: Exploratory Data Analysis.

The objective was to explore hospital admission data, identify important patterns related to 30-day patient readmission, and communicate the findings through statistical analysis and visualizations.

## Dataset

The analysis was performed using the cleaned dataset prepared during Task 1.

The dataset contains **120,000 hospital admissions** along with information related to:

* Admission and discharge details
* Length of stay
* Admission type
* Ward type
* Patient comorbidity
* Hospital information
* Treatment-related information
* Readmission indicators
* Billing and admission cost

## Tools Used

* Python
* Pandas
* Matplotlib
* Jupyter Notebook

## Exploratory Data Analysis

The following areas were analyzed:

* Overall 7-day and 30-day readmission rates
* Length of stay
* Admission type
* Ward type
* Discharge type
* Charlson Comorbidity Index
* Total admission cost
* Out-of-pocket expenses
* Hospital capacity
* Relationships between selected variables

The overall **30-day readmission rate was 11.84%**, while the **7-day readmission rate was 0.84%**. The average length of stay was **6.85 days**.

## Key Insights

### 1. Length of Stay and Readmission

The 30-day readmission rate increased as length of stay increased:

* 1–3 days: **6.53%**
* 4–7 days: **9.32%**
* 8–14 days: **16.48%**
* 15+ days: **28.80%**

This shows a strong association between longer hospital stays and higher 30-day readmission rates.

### 2. Ward Type and Readmission

The 30-day readmission rate varied considerably across ward types:

* General: **7.90%**
* HDU: **13.31%**
* ICU: **23.76%**
* NICU: **16.61%**

ICU admissions had a substantially higher observed readmission rate than General ward admissions.

### 3. Charlson Comorbidity Index and Readmission

Readmission rates increased progressively with the Charlson Index:

* Index 0: **5.59%**
* Index 3: **15.14%**
* Index 6: **29.62%**

Patients with higher comorbidity scores showed higher observed 30-day readmission rates.

### 4. Total Admission Cost and Readmission

Higher-cost admissions were associated with higher 30-day readmission rates:

* < ₹10k: **5.96%**
* ₹10k–50k: **8.89%**
* ₹50k–100k: **13.20%**
* ₹100k–500k: **19.86%**
* ₹500k+: **30.31%**

The results suggest a strong association between admission cost and readmission. This does not establish that higher cost causes readmission.

### 5. Discharge Type and Readmission

The observed 30-day readmission rates were:

* LAMA: **17.80%**
* Referred: **11.92%**
* Recovered: **11.78%**
* Expired: **0.00%**

LAMA cases had the highest observed readmission rate among the discharge categories that can meaningfully be followed for subsequent readmission. The 0% rate for Expired patients is not interpreted as a favorable outcome because patients who died cannot subsequently be readmitted.

## Conclusion

The exploratory analysis identified several important patterns associated with hospital readmission. Longer hospital stays, higher Charlson Index values, ICU admission, and higher admission costs were all associated with higher 30-day readmission rates.

These findings can help identify areas for further investigation and can be used as a foundation for developing a hospital readmission analytics dashboard.

## Project Files

* `EDA_Hospital_Readmission.ipynb` – Python exploratory data analysis
* `visualizations/` – EDA charts
