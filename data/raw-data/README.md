# raw-data

This folder contains the original, unmodified CSV files from the MIMIC-IV database (v3.1).

## Source
MIMIC-IV is a freely available de-identified clinical database from Beth Israel 
Deaconess Medical Center, available via PhysioNet:
https://physionet.org/content/mimiciv/

## Access
To obtain these files you must:
1. Create a PhysioNet account at https://physionet.org/
2. Complete the CITI "Data or Specimens Only Research" training
3. Sign the MIMIC-IV data use agreement
4. Download the files from the `hosp` module

## Files
- `patients.csv` — patient demographics (gender, age, date of death)
- `admissions.csv` — hospital admission and discharge records
- `prescriptions.csv` — medication orders per admission

## Important
These files should not be distributed publicly or posted to public repositories. Redistribution of MIMIC-IV data in any form 
is prohibited. You must obtain your own access via PhysioNet and download the full database yourself.

The raw data files were too large to upload onto GitHub and would have to be downloaded locally. 
