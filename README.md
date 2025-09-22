# Task-1---Data-Cleaning
## Netflix Dataset – Data Cleaning Process

## Overview
This document explains the **data cleaning and preprocessing steps** performed on the Netflix dataset using **Excel Power Query**. The goal was to prepare the dataset for analysis by handling missing values, normalizing multi-valued fields, and ensuring consistency.

## Steps Performed

### 1. downloaed the netflix movies dataset from kaggle
### 2. loaded the csv file in excel power query editor
### 3. using the data preview tab in power query, viewed the column quality , column profile and distribution, i got to know that there are missing values in the cast, director and country columns
### 4. - Replaced all `null` values with `"Unknown"` for better readability and consistency.
### 5. Removing Irrelevant Rows
- Some rows had `Director`, `Cast`, and `Country` all missing (i.e., `"Unknown"` in all three columns).
- Such rows were removed since they provided no useful information.

### 6. Splitting Multi-Valued Columns
- Columns affected: `Country`, `Genre`.
- These columns contained multiple values in a single cell separated by commas (`,`)

### 7. Split Column by Delimiter → Into Rows** in Power Query.
- This normalized the data, ensuring **each row represents one Title – one Country – one Genre**.

### 8. Duplicated Titles (Expected Behavior)
- After splitting, some movie/show titles appear multiple times.
- This is intentional and correct, as one title may belong to multiple countries or genres.

### 9. removed the description column 
### 10. used auto detect feature in power query to detect the date types


