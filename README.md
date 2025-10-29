🩺 Patient Outcomes of Injectable (Insulin) Therapies
Analysis of 5,000 Hospital Encounters — UCI Diabetes Dataset (1999–2008)

Author: Jyotirmoy Banerji

📘 1. Objective

The objective of this analysis is to investigate how insulin therapy (injectable treatment) influences patient outcomes, particularly hospital readmissions, and to identify other factors such as age, gender, and medication count that correlate with patient outcomes.

🧠 2. Dataset Overview

Source: UCI Machine Learning Repository — Diabetes 130-US Hospitals Dataset

Sample Size: 5,000 randomly selected patient encounters

Key Variables
Variable	Description
insulin	Type of insulin therapy (None, Up, Down, Steady)
readmitted	Hospital readmission status (<30 days, >30 days, or No readmission)
age, gender, race	Patient demographics
num_medications	Number of medications prescribed
time_in_hospital	Length of hospital stay
number_inpatient, number_outpatient, number_emergency	Hospital utilization metrics
⚙️ 3. Methodology
1. Data Cleaning

Replaced missing values (?) with NaN

Removed invalid entries for gender and race

2. Feature Engineering
New Feature	Description
readmitted_flag	Numeric variable (1 = readmitted, 0 = not readmitted)
readmit_label	Categorical variable (Readmit <30d, Readmit >30d, No Readmit)
insulin_flag	Binary variable (1 = insulin therapy, 0 = no insulin)
3. Exploratory Data Analysis (EDA)

Computed summary statistics and variable distributions

Visualized relationships between:

Readmission rates and insulin type

Readmission by age group

Number of medications vs. hospital stay

4. Dashboard Development

Created an interactive dashboard using Google Looker Studio (formerly Data Studio)

The dashboard summarizes key metrics and enables exploration of patient outcome patterns

📊 4. Key Findings
Finding	Insight
Overall readmission rate	~38%
Insulin therapy effect	Patients on insulin showed slightly higher readmission rates
Age factor	Older patients (>60) experienced more frequent readmissions
Treatment intensity	More medications correlated with longer hospital stays
🔍 5. Detailed Insights
5.1 Readmission by Insulin Type

Patients on insulin were slightly more likely to be readmitted within 30 days.

Suggests that closer monitoring of insulin-treated patients may reduce early readmissions.

5.2 Age and Readmission

Patients aged 60–79 had the highest readmission frequency.

Younger patients (<40) had lower readmission rates, even with insulin therapy.

5.3 Medication Count vs Hospital Stay

Patients on more medications had longer hospital stays.

This trend was more pronounced among insulin users, suggesting polypharmacy may impact recovery time.

✅ 6. Conclusion

This analysis of 5,000 hospital encounters provides actionable insights into the outcomes of injectable therapies:

Insulin therapy, age, and number of medications are all correlated with hospital readmissions.

The interactive Looker Studio dashboard helps clinicians identify high-risk patients and optimize care plans for improved outcomes.

🧩 7. Tools & Technologies

Python (Pandas, NumPy, Matplotlib, Seaborn)

Google Looker Studio — for interactive data visualization

UCI Diabetes 130-US Hospitals Dataset

📈 8. Dashboard Access

The interactive dashboard (Looker Studio) summarizes patient outcome metrics.
(Include the dashboard link here once available.)

📂 9. Citation

Dataset Citation:

Strack, B. et al. (2014). Impact of HbA1c Measurement on Hospital Readmission Rates: Analysis of 70,000 Clinical Encounters. UCI Machine Learning Repository.
