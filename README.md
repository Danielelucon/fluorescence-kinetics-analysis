# Fluorescence Kinetics Analysis

This repository provides a downstream analysis pipeline for fluorescence data obtained from intact algae or spinach-extracted thylakoids. 

The pipeline parses raw fluorometer outputs (similar to standard DUAL-PAM measurements), handles kinetic visualisation and standard deviation calculations, and automates multi-panel grid generation.

## Repository Contents

*   `YII_kinetic_pipeline.ipynb`: The primary Jupyter Notebook pipeline.
*   `YII_kinetic_pipeline.py`: A standalone Python script version of the pipeline.
*   `dummy_ETR.xlsx`: An anonymised dataset for local testing.

## Mandatory Data Structure

Your Excel column headers must follow this exact syntax: `Species_Condition_Replicate`.

**Examples:**
*   `Chlamy_Control_1`
*   `Chlamy_CD_500_mM_3`
*   `SpeciesA_10_uM_2`

## Local Execution

### 1. Install Dependencies
Install the required libraries via your terminal:
`pip install numpy pandas matplotlib openpyxl`

### 2. Run the Code
**Option A: Using standard Python**
Open `YII_kinetic_pipeline.py` in your preferred IDE, update the `EXCEL_FILE` and sheet name variables at the top of the script, and execute.

**Option B: Using Jupyter Notebook**
Launch the notebook environment from your terminal:
`jupyter notebook`
Open `YII_kinetic_pipeline.ipynb`, modify the `EXCEL_FILE` and sheet name in the first cell, and run the notebook.
