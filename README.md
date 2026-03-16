
# assets
This folder contains references that have been used for the project.

# code
This folder contains all data cleaning and wrangling scripts for the project.

# data
This folder contains the raw data and the processed data (raw data with edits made.

# products
This folder contains manuscript and report. The manuscript includes the written introduction, methods, results, and discussion. 

# results 
This folder contains figures, large files, output, and tables. This is where all the results produced by the code will be.

## Files

- `mimic-processing.qmd` — loads the raw MIMIC-IV CSV files, cleans and merges 
  tables, computes 30-day mortality, assigns medication classes, and saves 
  the final analytic dataset.

## Inputs

Raw data files from `data/raw-data/`:
- `patients.csv`
- `admissions.csv`
- `prescriptions.csv`

## Output

- `data/processed-data/analysis_dataset.csv` — the final analytic dataset used 
  by all downstream scripts and the manuscript

## How to Run

From the project root:

    quarto render code\processing-code\mimic-processing.qmd

## Notes

- This script must be run before the EDA script and before the manuscript
- The sampling block near the top of the script limits the data to 10,000 
  admissions for development speed. Comment it out to run on the full dataset.
