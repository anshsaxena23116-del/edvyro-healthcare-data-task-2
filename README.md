# Edvyro Healthcare & Data Analytics Internship — Task 2

## Healthcare Data Governance and Cleaning

### Objective
Create a privacy-aware data dictionary and clean de-identified patient records using reproducible validation rules.

### Dataset
`Cleaned_Patient_Records.csv` contains the supplied synthetic patient records. No clinical values were changed because the validation checks found no data-quality exceptions.

### De-identification statement
The sample uses coded Patient IDs (for example, PAT-201) and does not include direct identifiers such as patient names, phone numbers, email addresses, street addresses, or dates of birth. The remaining fields are demographic and clinical attributes used for analytics.

### Validation performed
- Patient ID format and uniqueness
- Missing-value check
- Data types
- Age validation (0–120 integer validation range)
- Gender category consistency
- Positive numeric dosage
- Positive integer treatment duration
- Readmission category consistency
- Blood-pressure structural validation
- Positive numeric cholesterol value

### Results
- Records: 10
- Missing values: 0
- Duplicate Patient IDs: 0
- Validation exceptions: 0

### Cleaning approach
The cleaning process is conservative. It does not invent, estimate, or overwrite clinical values. When an exception is present, it should be logged and reviewed rather than silently replaced. For this supplied sample, no corrections were required.

### Files
- `Cleaned_Patient_Records.csv` — cleaned/de-identified records
- `Data_Dictionary.csv` — field classifications, privacy rationale, and validation rules
- `Quality_Exception_Log.csv` — validation results
- `Validation_Rules.txt` — reproducible rules used
- `README.md` — submission summary

### Submission
Place this folder in a GitHub repository or a view-only Google Drive folder and submit one public/view-only link, as required by the Edvyro task instructions.
