Multi-Dataset Cleaning and Transformation with Python

Project Overview

This project demonstrates data cleaning, filtering, transformation, formatting, and reporting techniques using Python and pandas. The analysis combines five parts of a BAN130 academic group assignment and works with multiple datasets originally stored in SAS format.

The project shows how raw data can be converted into structured, analysis-ready outputs through conditional filtering, new-variable creation, classification rules, sorting, formatting, and validation.

Project Type and Contribution

This was completed as a five-member academic group project. Each member was responsible for one section of the final analysis.

My primary contribution was Part 1: Exploring and Filtering EU Occupancy Data, which included:

Loading a SAS dataset with pandas

Inspecting the dataset structure and values

Decoding byte-string columns into readable text

Filtering monthly records to retain observations from 2016

Formatting hotel, short-stay, and camping values with thousands separators

Removing an unnecessary geographic-code column

Verifying the final structure and output

The remaining sections were completed collaboratively and assembled into the final group notebook.

Project Components

Part 1 — Exploring and Filtering EU Occupancy Data

The European occupancy dataset was cleaned and filtered to show 2016 tourism records. Text fields imported from SAS were decoded, selected accommodation measures were formatted for reporting, and the Geo column was removed from the final result.

Part 2 — Creating and Formatting National Park Variables

New analytical variables were created from the National Park summary data:

SqMiles converted park acreage into square miles.

Camping combined multiple camping-related measures.

Selected numerical values were formatted for readable reporting.

A processed CSV output was generated.

Part 3 — Transforming and Summarizing National Park Data

Conditional logic was used to classify National Park records into categories such as monument, park, preserve, seashore, river, and other. The transformed data was then summarized and visualized for reporting.

Part 4 — Customer Data Queries and Formatting

The customer dataset was filtered using multiple business conditions. Examples included:

Finding customers with a missing Bank ID and a credit score above 700

Sorting qualifying customers by income

Formatting income as currency

Converting SAS date values into standard dates

Identifying employed customers born before a specified date

Part 5 — Case-Based Customer Classification

Conditional rules were used to create new categorical variables, including:

Credit-score categories

Readable marital-status descriptions

The results were checked against the original fields to confirm that the transformations were applied correctly.

Tools and Technologies

Python

Jupyter Notebook

pandas

NumPy

Matplotlib

SAS datasets (.sas7bdat)

CSV output

Skills Demonstrated

Importing SAS data into Python

Data inspection and validation

Byte-string decoding

Conditional filtering

Data type conversion

Date conversion

Feature engineering

Case-based classification

Sorting and formatting

Missing-value filtering

Data aggregation

Exporting processed results

Collaborative notebook integration

Repository Structure

01-multi-dataset-data-transformation/
├── README.md
└── multi_dataset_data_transformation.ipynb

Data Availability

The original datasets are not included in this public repository because of file-size limitations, privacy considerations, and academic-use restrictions. In particular, the customer dataset contains sensitive-style personal and financial fields and is therefore excluded from the portfolio version.

The notebook retains the code and previously generated outputs so that the analytical workflow and results can be reviewed without distributing the original course data.

Reproducibility

The notebook cannot be executed from beginning to end without the original course datasets:

eu_occ.sas7bdat
np_summary.sas7bdat
customer.sas7bdat

Users with authorized access to these datasets can place them in the same directory as the notebook and run the cells from top to bottom. The following packages are required:

pip install pandas numpy matplotlib pyreadstat

Key Learning Outcomes

This project strengthened my ability to translate written data-processing requirements into reproducible Python operations. It also provided experience combining independently developed sections into a single group deliverable while preserving code, explanations, and analytical outputs.

Academic Integrity

This repository is presented as a portfolio record of an academic group assignment. The group nature of the work and my individual contribution are identified above. The material is shared for professional demonstration and learning purposes, not as a submission template for current students.

