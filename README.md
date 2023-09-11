# SSOteam
# Sepsis: Know the Signs, Act in Time
## Table of Contents
- [SSOteam](#SSOteam)
    - [Background](#Background)
        - [Sepsis: A silent killer](#sepsis-A-silent-killer) 
    - [Data](#data)
    - [Usage](#usage)
        - [Installation](#installation)
        - [Requirements](#requirements) _Can be named Dependencies as well_
        - [Activate conda environment](#activate-conda-environment) _Optional_
        - [Steps to run ](#steps-to-run) _Optional depending on project_
            - [Step-1](#step-1)
            - [Step-2](#step-2)
    - [Methods](#methods)
    - [Results](#results) _Optional depending on project_
    - [Team Members](#team-members)

## Background

**Sepsis: A silent killer**
Sepsis is a life-threatening medical condition that demands immediate attention and action. It occurs when the body's immune response to an infection goes haywire, triggering a cascade of events that can lead to organ failure and death. Understanding the importance of early detection and recognizing its indicators is critical in the battle against this deadly condition.

**The Sepsis Menace: Why Detection Matters**
Sepsis can affect anyone, from infants to the elderly, and it doesn't discriminate based on gender, race, or socioeconomic status. It is a leading cause of morbidity and mortality worldwide, responsible for millions of deaths each year. According to the World Health Organization (WHO), sepsis accounts for up to 30 million cases globally, with over 6 million deaths annually. One of the primary reasons sepsis is so deadly is its rapid progression. It can develop within hours, catching both patients and healthcare professionals off guard. Without timely intervention, sepsis can lead to multiple organ failure and death. However, when identified and treated promptly, the chances of survival increase significantly. This is why recognizing the indicators of sepsis for early detection is of paramount importance.

**Project description**
Here, we used a publicly available dataset from patients admitted to hospitals who did or did not develop sepstic shock and utilize the physiological variables collected within 6-12 hours before sepsis onset for unsupervised and supervised clustering to identify early predictors of septic risk. 

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
