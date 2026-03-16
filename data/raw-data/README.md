# raw-data

This folder contains synthetic datasets that mimic the structure of tables from the MIMIC-IV database (v3.1).
The data included here were generated for demonstration and analysis purposes and do not contain any real patient information.

## Source Inspiration

The synthetic datasets were designed to replicate the schema and general characteristics of the MIMIC-IV clinical database, which is a freely available de-identified clinical database from Beth Israel Deaconess Medical Center distributed through PhysioNet:

https://physionet.org/content/mimiciv/

## Why Synthetic Data Was Used

The original MIMIC-IV data cannot be redistributed publicly due to its data use agreement.
To allow this project to be shared on GitHub while maintaining the structure needed for analysis, synthetic data were generated that follow the same table formats and variable names as the original database.

The original dataset was also very large and would not be able to be uploaded to GitHub. The synthetic dataset is smaller to make analysis faster and easier.

These datasets allow code and workflows to be reproduced without requiring access to restricted clinical data.

## Access to Real MIMIC-IV Data

To obtain the actual MIMIC-IV dataset you must:

Create a PhysioNet account at https://physionet.org/

Complete the CITI "Data or Specimens Only Research" training

Sign the MIMIC-IV data use agreement

Download the files from the hosp module

## Files

The synthetic files included here replicate tables used in analyses:

patients.csv — synthetic patient demographics (gender, anchor age, date of death)

admissions.csv — synthetic hospital admission and discharge records

prescriptions.csv — synthetic medication orders per admission