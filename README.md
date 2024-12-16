# HCM Legionella Project

As a final project for a Healthcare Database Management class at New York University (NYU), this project explores deidentified relational databases to investigate case and treatment trends for legionella pneumonia at NYU Langone Health Center (NYULHC) in New York City (NYC).

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Notebook Outline](#notebook-outline)
- [Usage](#usage)
- [Contributers](#contributers)


## Introduction
Legionella is a type of bacteria that can cause pneumonia which is some cases is potentially fatal. 
Legionella thrives in cool damp climates, such as cooling towers in New York City (NYC).
This project examines legionella case characteristics at NYU Langone Health with cooling tower survelliance by NYC Department of Health (DOH).

## Installation
To install the necessary dependencies, run the following command:
```bash
pip install -r requirements.txt
```

## Notebook Outline
The organization of the notebook for all code is provided below
1. Importing necessary libraries

2. Creation of cleaned databases from the data downloaded from NYULHC database registry. This downloaded data has been previously filtered using SQL on Apache Impala. The cleaned and normalized regional databases created include:

- `abs.csv`: Legionella serum antibody test results and dates of testing
- `diagnosis.csv`: Admission diagnosis for patients tested for legionella
- `enc_id_pt_id.csv`: Encounter IDs matched with patient IDs
- `encounter.csv`: Encounter IDs matched with year and admission status
- `healthcare_data.db`: Consolidated database on sqlite3 incuding information all other datatables referenced
- `inspection.csv`: NYC DOH cooling town violation citations with citation code
- `medication.csv`: Anti-infective medications prescribed during hospitalization
- `patient.csv`: Patient IDs with demographic characteristics
- `pcr.csv`: Respiratory legionella PCR test results and dates of testing
- `urine_antigen.csv`: Legionella urine antigen and dates of testing

3. Mapping legionella positive results aggregrate by year and my time of year averaged for 14 years with visualizations

4. Mapping legionella yearly positive results with number of NYC DOH issued violations for lack of legionella testing in a cooling tower with visualizations

5. Investigation if patients positive for legionella were given the correct antibiotic for the correct lenght of time with visualizations

6. Correlation between positive and negative results between urine antigen, PCR, and antibodies with confusion martrix visualizations

7. Characteristics among  patients with legionella compared to those without legionella when the diagnosis  is pneumonia

8. Characteristics of patients admitted to the hospital with legionella and those as outpatients

## Usage

All needed databases and codes are contanted in provided directory "Group_3_HCM_Legionella_Project"

## Contributers
This project was completed for at NYU for the Healthcare Data Management Fall 2024 Course. Contributers as follows:
- Luke O'Donnell, MD
- Dusk Shin
- Nwe Ni Aung
