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
:exclamation: _Include background on the project, project description, and significance. This will be converted to your team's abstract by the end of the hackathon._ :exclamation:

### Sepsis: A silent killer
Sepsis is a life-threatening medical condition that demands immediate attention and action. It occurs when the body's immune response to an infection goes haywire, triggering a cascade of events that can lead to organ failure and death. Understanding the importance of early detection and recognizing its indicators is critical in the battle against this deadly condition.

### The Sepsis Menace: Why Detection Matters
Sepsis can affect anyone, from infants to the elderly, and it doesn't discriminate based on gender, race, or socioeconomic status. It is a leading cause of morbidity and mortality worldwide, responsible for millions of deaths each year. According to the World Health Organization (WHO), sepsis accounts for up to 30 million cases globally, with over 6 million deaths annually. This staggering figure highlights the gravity of the situation and underscores the urgency of early detection.

One of the primary reasons sepsis is so deadly is its rapid progression. It can develop within hours, catching both patients and healthcare professionals off guard. Without timely intervention, sepsis can lead to multiple organ failure and death. However, when identified and treated promptly, the chances of survival increase significantly. This is why recognizing the indicators of sepsis is of paramount importance.

## Data
"Prediction of Sepsis" dataset from Kaggle: https://www.kaggle.com/datasets/salikhussaini49/prediction-of-sepsis?resource=download

The dataset was obtained from two geographically distinct U.S. hospital systems: Beth Israel Deaconess Medical Center (hospital system A), Emory University Hospital (hospital system B). It consisted of a combination of hourly vital sign summaries, lab values, and static patient descriptions. In particular, the data contained 40 clinical variables: 8 vital sign variables, 26 laboratory variables, and 6 demographic variables. Altogether, these data included over 1.5 million hourly time windows.

Data extracted from the Electronic Medical Record (EMR) underwent a series of preprocessing steps prior to formal analysis and model development. All patient features were condensed into hourly bins simplifying model development and testing, e.g., multiple heart rate measurements in an hourly time window were summarized as the median heart rate measurement. Multiple Logical Observation Identifiers Names and Codes (LOINC) codes describing the same clinical parameter were condensed into a single variable, e.g., serum hemoglobin and arterial hemoglobin became hemoglobin. 

## Usage

:exclamation: _How will someone not involved in your project be able to run the code or use it._ :exclamation:

### Installation

:exclamation: _If installation is required, please mention how to do so here._ :exclamation:

Installation simply requires fetching the source code. Following are required:

- Git

To fetch source code, change in to the directory of your choice and run:

```sh
git clone -b main \
    git@github.com:u-brite/team-repo-template.git
```

### Requirements
:exclamation: _Note any software used (including Python or R packages), operating system requirements, etc. and its version so that your project is reproducible. It does not have to be in the below format_ :exclamation:

*OS:*

Currently works only in Linux OS. Docker versions may need to be explored later to make it useable in Mac (and
potentially Windows).

*Tools:*

- Anaconda3
    - Tested with version: 2020.02

### Activate conda environment
:exclamation: _Optional: Depends on project._ :exclamation:

Change in to root directory and run the commands below:

```sh
# create conda environment. Needed only the first time.
conda env create --file configs/environment.yaml

# if you need to update existing environment
conda env update --file configs/environment.yaml

# activate conda environment
conda activate testing
```

### Steps to run
:exclamation: _Optional: Depends on project._ :exclamation:

#### Step 1

```sh
python src/data_prep.py -i path/to/file.tsv -O path/to/output_directory
```

#### Step 2

```sh
python src/model.py -i path/to/parsed_file.tsv -O path/to/output_directory
```

Output from this step includes -

```directory
output_directory/
├── parsed_file.tsv               <--- used for model
├── plot.pdf- Plot to visualize data
└── columns.csv - columns before and after filtering step

```

**Note**: The is an example note with a [link](https://github.com/u-brite/team-repo-template).

## Methods
The dataset was downloaded as .csv file and loaded into Google Colab. The dataset contains 1,552,210 rows with 40 variables from 40,339 patients. 
## Results

## Team Members

|Name | Email | Role |
----|--|--|
|Phuong Quach               | phuong@uab.edu                   | Team Member |
|Van Huynh                  | vanhuynh@uab.edu                 | Team Member |
|Ana Chang                  | achang@pnwu.edu                  | Team Member |
|Yishu Qu                   | yishuqu2024@u.northwestern.edu   | Team Leader |
