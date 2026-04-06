# data

The folders inside this folder should contain all data at various stages.

This data is being loaded/manipulated/changed/saved with code from the `code` folders.

You should place the raw data in the `raw-data` folder and not edit it. Ever!

The `raw-data` folder contains a synthetic dataset that mimics the real database of MIMIC-IV and is generated using the `data\raw-data\raw-synthetic-data.qmd` file and outputed into the `raw-data` folder.

The `processed-data` folder contains the collective, clean dataset that is used for analysis. The processed data is produced by the file `code\processing-code\mimic-processing.qmd`