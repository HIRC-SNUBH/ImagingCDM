# Project Overview

## Introduction
This repository contains a Python-based solution for extracting data from DICOM (Digital Imaging and Communications in Medicine) files, transforming this data into the Observational Medical Outcomes Partnership Common Data Model (OMOP CDM) format, and subsequently storing it in a SQL database. This process is crucial for facilitating medical research and healthcare analytics by standardizing medical data for easy access and analysis.

## Background
DICOM is the standard format for storing and utilizing medical imaging information and related data. OMOP CDM, on the other hand, is a widely adopted standard for representing healthcare data for observational research. The transformation of DICOM to OMOP CDM and the efficient storage of this data in a SQL database is an essential step in leveraging healthcare data for research and analytical purposes.

## Objective
The primary goal of this project is to provide a seamless, automated pipeline for converting medical imaging data from the DICOM format into the OMOP CDM format and then storing this transformed data into a SQL database. This facilitates researchers and healthcare professionals in conducting various types of analyses, including population health studies, treatment effectiveness research, and safety surveillance.

# Features
- **DICOM Data Extraction**: The code extracts essential information from DICOM files, which includes patient demographics, imaging metadata, and diagnostic information.
- **Data Transformation**: Converting the extracted data into the OMOP CDM format, ensuring it adheres to the required standards for consistency and compatibility with observational research tools.
- **SQL Database Integration**: The transformed data is then efficiently loaded into a SQL database, allowing for robust data management and easy retrieval for analysis.

# How it Works
1. **Data Extraction**: The Python script reads DICOM files and extracts relevant data.
2. **Data Transformation**: The extracted data is then mapped and transformed into the OMOP CDM format using a predefined schema.
3. **Database Storage**: The OMOP CDM formatted data is loaded into a SQL database, ensuring data integrity and security.

# Usage
To use `DICOMtoRCDMtable.py`, you must first configure the SQL connection. This involves setting up the connection parameters in the script:
```python
conn = psycopg2.connect(database='[DATABASE_NAME]', user='[USERNAME]', password='[PASSWORD]', host='localhost', port='[PORT]')
```
Replace `[DATABASE_NAME]`, `[USERNAME]`, `[PASSWORD]`, and `[PORT]` with your specific SQL database information.

# Contribution
This research was supported by a grant of the Korea Health Technology R&D Project through the Korea Health Industry Development Institute (KHIDI), funded by the Ministry of Health & Welfare, Republic of Korea (grant number : HI22C0471).

# Contact
For any queries or suggestions, please contact [hyerim1606@gmail.com].

