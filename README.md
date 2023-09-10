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
Prediction of Sepsis data set from Kaggle: https://www.kaggle.com/datasets/salikhussaini49/prediction-of-sepsis?resource=download

## Usage

:exclamation: _How will someone not involved in your project be able to run the code or use it._ :exclamation:

### Installation

:exclamation: _If installation is required, please mention how to do so here._ :exclamation:

Installation simply requires fetching the source code. Following are required:

- Git

To fetch source code, change in to directory of your choice and run:

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

## Results

## Team Members

|Name | Email | Role |
----|--|--|
|Phuong Quach               | phuong@uab.edu                   | Team Member |
|Van Huynh                  | vanhuynh@uab.edu                 | Team Member |
|Ana Chang                  | achang@pnwu.edu                  | Team Member |
|Yishu Qu                   | yishuqu2024@u.northwestern.edu   | Team Member |
