
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

- `raw-synthetic-data.qmd` - creates a synthetic databases that resembles the MIMIC-IV CSV files
- `mimic-processing.qmd` — loads the raw MIMIC-IV CSV files, cleans and merges 
  tables, computes 30-day mortality, assigns medication classes, and saves 
  the final analytic dataset.
- `mimic-eda.qmd` - creates exploritory figures of the final analytic dataset


## Inputs

Raw data files from `data/raw-data/`:
- `patients_syn.csv`
- `admissions_syn.csv`
- `prescriptions_syn.csv`

## Output

- `data/processed-data/analysis_dataset.csv` — the final analytic dataset used 
  by all downstream scripts and the manuscript
- `products\manuscript\Manuscript.html` - final manuscript with results and figures


## How to Run
  In order:
  
    quarto render data\raw-data\raw-synthetic-data.qmd
    quarto render code\processing-code\mimic-processing.qmd
    quarto render code\eda-code\mimic-eda.qmd
    quarto render products\manuscript\Manuscript.qmd

