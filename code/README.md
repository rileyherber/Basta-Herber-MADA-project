# code
This folder contains all data cleaning and wrangling scripts for the project.

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

