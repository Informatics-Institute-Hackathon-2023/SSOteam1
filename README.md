# SSOteam
# Sepsis: Know the Signs, Act in Time
## Table of Contents
- [SSOteam](#SSOteam)
    - [Background](#Background)
    - [Data](#data)
    - [Methods](#methods)
    - [Results](#results) _Optional depending on project_
    - [References] (#References)
    - [Team Members](#team-members)

## Background
Sepsis is a life-threatening medical condition that requires immediate attention and action. It is a leading cause of morbidity and mortality worldwide. According to the World Health Organization (WHO), sepsis accounts for 31 million cases globally, contributing to 5.3 million deaths worldwide per year. Sepsis is characterized by dysregulated immune response to infection, which triggers a cascade of events that can lead to organ failure and death. Although our understanding of the pathophysiology has made progress during the last decades, specific and sucessful interventions are still lacking. Fluid resusciation and early administration of broad-spectrum antibiotics are the only interventions that may reduce mortality. Without timely intervention, sepsis can lead to multiple organ failure and death. Therefore, recognizing the indicators of sepsis for early detection is of paramount importance.

**Project description**
Here, we used a publicly available dataset from patients admitted to hospitals who did or did not develop sepstic shock and utilize the physiological variables  for machine learning to identify early signs of septic, contributing to effort for the early detection of this deadly condition.

## Data
"Prediction of Sepsis" dataset from Kaggle: https://www.kaggle.com/datasets/salikhussaini49/prediction-of-sepsis?resource=download

The dataset was obtained from two geographically distinct U.S. hospital systems: Beth Israel Deaconess Medical Center (hospital system A), Emory University Hospital (hospital system B). It consisted of a combination of hourly vital sign summaries, lab values, and static patient descriptions. In particular, the data contained 40 clinical variables: 8 vital sign variables, 26 laboratory variables, and 6 demographic variables. Altogether, these data included over 1.5 million hourly time windows.

Data extracted from the Electronic Medical Record (EMR) underwent a series of preprocessing steps prior to formal analysis and model development. All patient features were condensed into hourly bins simplifying model development and testing, e.g., multiple heart rate measurements in an hourly time window were summarized as the median heart rate measurement. Multiple Logical Observation Identifiers Names and Codes (LOINC) codes describing the same clinical parameter were condensed into a single variable, e.g., serum hemoglobin and arterial hemoglobin became hemoglobin. 

## Methods
The dataset was downloaded as .csv file and loaded into Google Colab, which contains 1,552,210 rows with 40 variables from 40,339 patients, in which 2,932 developed sepsis and 37,404 did not. Among septic patients, 426 had sepsis before ICU admission and therefore were excluded from the analysis. Exploratory data analysis shows missing values in a number of variables, and therefore value imputation was implemented (bfill and ffill) to fill the missing data. The cleaned data was then used for k-means unsupervised clustering algorithm (KMeans from sklearn.cluster) and visualized using principal component analysis (PCA from sklearn.decomposition).     

## Results


## References
1. Deng HF, Sun MW, Wang Y, Zeng J, Yuan T, Li T, Li DH, Chen W, Zhou P, Wang Q, Jiang H. Evaluating machine learning models for sepsis prediction: A systematic review of methodologies. iScience. 2021 Dec 20;25(1):103651. doi: 10.1016/j.isci.2021.103651. PMID: 35028534; PMCID: PMC8741489.
2. 

## Team Members

|Name | Email | Role |
----|--|--|
|Phuong Quach               | phuong@uab.edu                   | Team Member |
|Van Huynh                  | vanhuynh@uab.edu                 | Team Member |
|Ana Chang                  | achang@pnwu.edu                  | Team Member |
|Yishu Qu                   | yishuqu2024@u.northwestern.edu   | Team Leader |
