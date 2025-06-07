
## Retool Dashboard to analyse the cause of the missing encounters while importing Patient information

---

2 CSV files are given.

- [Sample DB data](https://github.com/Mahinkhan007/Data_Science_Portfolio/blob/main/Retool%20Dashboard%20for%20missing%20encounters/Ops%20Case%20Study%20Dataset%20-%20Sample%20EHR%20Data%20(2).csv)
- [Sample EHR data] (https://github.com/Mahinkhan007/Data_Science_Portfolio/blob/main/Retool%20Dashboard%20for%20missing%20encounters/Ops%20Case%20Study%20Dataset%20-%20Sample%20EHR%20Data%20(2).csv)

---

Each dataset contains information about Patient Name, Date of Service, and Rendering Provider, which together form a unique id for an encounter, alongside procedure-level details.

Some encounters in the client’s EHR may not be present in our database, and the task is to identify these missing encounters and come to a conclusion as to why the encounters weren’t imported.

---

## Dashboard Summary:

Potential issues based on EHR vs DB comparison:

Extra spaces in patient_name or provider_name (e.g., "John Doe " vs "John Doe")
Date formatting differences:
EHR: "07/24/2024" or "2024-07-24"
DB: standardized format (DATE)
Case sensitivity:
"john doe" vs "John Doe"
✅ Actionable Insight: Add data normalization steps (e.g., trimming, standard casing, unified date format) in the import pipeline.
✅ I have trimmed the both datasets and maintained uppercase letters and same formats for Dates.

Missing encounters were not random.
Spikes occurred on specific dates (e.g., Sep 25), likely due to failed or incomplete imports.
The majority of missing encounters are tied to a few providers, possibly due to template or formatting issues.
Formatting mismatches in names and dates may have caused false "non-matches" during import.
🛠️ Next Steps:
Normalize names (trim, lowercase)
Standardize date formats
Review data entry practices for top providers
Check logs on spike days for system errors.

---

##Snapshots: 

-![Banner]()
-![Banner]()

##Deliverables:
-Retool Dashboard
-SQL Queries
