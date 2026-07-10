# fluorescence-kinetics-analysis

FLUORESCENCE KINETICS ANALYSIS PIPELINE

Welcome to my first independent repository. This project is focused on the downstream analysis of fluorescence data obtained from either intact algae or spinach-extracted thylakoids for a rapid processing and plotting

The measurement types are similar to standard DUAL-PAM outputs. The fluorometer natively processes the raw data, and the Python notebooks in this branch handle the kinetic visualisation, standard deviation calculations, and automated multi-panel grid generation.

REPOSITORY CONTENTS

YII_kinetic_pipeline.ipynb: The primary universal pipeline to parse traces and generate grids.

dummy_ETR.xlsx: An anonymised dummy dataset to test the pipeline locally.

MANDATORY DATA STRUCTURE

For the script to work, your Excel column headers must follow this exact syntax with underscores: Species_Condition_Replicate

Examples:

Chlamy_Control_1

Chlamy_CD_500_mM_3

SpeciesA_10_uM_2

LOCAL EXECUTION

Install the required libraries in your terminal by typing:

pip install numpy pandas matplotlib seaborn scipy statsmodels jupyter notebook openpyxl

Download or clone this repository to your computer.

Launch Jupyter Notebook in your terminal by typing:
jupyter notebook

Open the notebook, change the EXCEL_FILE name at the top to match your file, and run the cells.
