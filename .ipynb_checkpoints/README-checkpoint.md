# Survival Analysis of Eye Cancer Patients

This is a survival analysis project using both traditional data analysis and machine learning techniques. Preprocessing values and creating dummy values where needed. 

Data source: 

https://www.kaggle.com/datasets/ak0212/eye-cancer-patient-records?resource=download#

### About data

The dataset provides detailed medical and demographic information for 5,000 patients diagnosed with various types of eye cancer, including Melanoma, Retinoblastoma, and Lymphoma. It includes fields such as:

Patient Demographics: Age (1–90), Gender, Country

Clinical Details: Cancer type, Laterality (Left/Right/Bilateral), Stage at diagnosis

Diagnosis & Treatment: Date of diagnosis, Type of treatment (Surgery, Radiation, Chemotherapy), Treatment intensity (e.g., radiation dose in Gy, number of chemo sessions)

Outcomes: Survival time in months, Outcome status (In Remission, Active, Deceased)

Genetics & History: Genetic markers (e.g., BRAF mutation), Family history of eye cancer

## Explanatory Data Analysis and Cox Proportional Hazards Model (cancer_a.ipynb)

### EDA

Analysing the effect of BRAF mutation on the sutvival of the patients. 

Visualized feature distributions and survival times.

Plotted Kaplan-Meier survival curves stratified by treatment type, cancer stage, and gender.

Found no strong predictors of survival.

### Cox Model

Time Column: Survival_Time_Months

Event Column: event_occurred

Results:
Most features were not statistically significant.

Model is random guessing.

## ML with Random Survival Forest (cancer_ml.ipynb)

Tried with multiple different parameters. 

Model is random guessing. 


## Findings 
The concordance index is low for both models. The database might not contain the truly relevant key data for the subject. In conclusion, we couldn't manage to build a reliable model. 

