Patient Outcomes of Injectable (Insulin) Therapies
Analysis of 5,000 Hospital Encounters — UCI Diabetes Dataset (1999–2008)
Author: Jyotirmoy Banerji
￼
1. Objective
The goal of this analysis is to investigate how insulin therapy (injectable treatment)
affects patient outcomes, particularly hospital readmissions, and to identify other factors
such as age, gender, and medication count that correlate with patient outcomes.
￼
2. Dataset Overview
• Source: UCI Machine Learning Repository — Diabetes 130-US Hospitals
dataset
• Sample size for this analysis: 5,000 random patient encounters
• Key Variables:
o insulin – type of insulin therapy
o readmitted – hospital readmission status (<30 days, >30 days, or no
readmission)
o age, gender, race – patient demographics
o num_medications, time_in_hospital, number_inpatient,
number_outpatient, number_emergency – treatment intensity and
utilisation
￼
3. Methodology
1. Data Cleaning: Replaced missing values (?) with NaN and removed invalid
gender/race entries.
2. Feature Engineering:
o Created numeric readmitted_flag (1 = readmitted, 0 = no readmission)
o Created readmit_label categorical column (Readmit <30d, Readmit
>30d, No Readmit)
o Created insulin_flag numeric column (1 = patient used insulin therapy,
0 = no insulin)
3. Exploratory Data Analysis (EDA):
4. o Summary statistics and distributions of variables
o Visualisations of readmission by insulin type, age group, and number of
medications
Dashboard: The summarised dataset was uploaded to Google Looker Studio
(formerly Data Studio) to create an interactive, one-page dashboard for key
patient outcome metrics.
￼
4. Key Findings
• Overall readmission rate: ~38%
• Patients on insulin showed slightly higher readmission rates than those not on
insulin
• Age influence: Older patients (>60) tend to have more frequent readmissions
• Treatment intensity: Patients with higher numbers of medications generally
have longer hospital stays
￼
5. Detailed Insights
5.1 Readmission by Insulin Type
• Patients on insulin were slightly more likely to be readmitted within 30 days
compared to non-insulin patients.
• Suggests careful monitoring of insulin-treated patients may help reduce early
readmissions.
5.2 Age and Readmission
• Patients aged 60–79 showed the highest frequency of readmission.
• Younger patients (<40) had lower readmission rates, even with insulin therapy.
5.3 Medication Count vs Hospital Stay
• Patients on more medications tend to have longer hospital stays.
• Trend is more pronounced among insulin users, suggesting poly pharmacy
impacts patient recovery time.
￼
6. Conclusion
This analysis of 5,000 hospital encounters provides actionable insights into patient
outcomes of injectable therapies: - Insulin therapy, age, and number of medications are
correlated with readmissions. - An interactive Looker Studio dashboard allows clinicians
to identify high-risk patients and optimise care.
￼
