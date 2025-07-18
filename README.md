# Synergy2 Kinetics Parser

This repository contains a Jupyter notebook (`Synergy2_kynetics.ipynb`) designed to extract and normalize fluorescence time-lapse data from **Synergy 2** multiwell plate reader experiments.

## What it does

- Reads `.xlsx` files exported from **Synergy 2**
- Extracts fluorescence data for each well over time
- Organizes data into tidy format
- Calculates baseline-normalized fluorescence (F/F₀)
- Exports to `.csv` and `.xlsx`

## Requirements

- `pandas`
- `openpyxl`
- Jupyter Lab/Notebook (for interactive use)

Install with:

```bash
pip install pandas openpyxl

## Parameters to set

Inside the notebook, adjust the following:
filename: name of your input Excel file
location: full path to the folder containing your file
fecha: experiment date (used for export file names)
tdelta: time between reads (in seconds)
jump: time (in minutes) used to define the baseline window for normalization

## Output

Two files (optional; you can uncomment these lines in the notebook):
YYYYMMDD_Synergy.csv
YYYYMMDD_Synergy.xlsx
