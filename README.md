# COVID-19 Clinical Trials — EDA (Pandas)

Short project summary
---------------------
This repository contains a Jupyter Notebook that performs exploratory data analysis (EDA) on a CSV extract of COVID-19 clinical trials (source: ClinicalTrials.gov). The notebook cleans the data, performs basic validation and imputations, and produces visualizations to summarize trial status, gender inclusion, country distribution, enrollment distribution, trial phase comparisons, and temporal trends.

How the project works
---------------------
- Load the dataset from `COVID clinical trials.csv` into a pandas `DataFrame`.
- Inspect the schema and basic statistics with `df.info()` and `df.describe()`.
- Handle missing values: drop very sparse columns, impute selected categorical columns, impute `Enrollment` with median, and replace remaining missing values (the notebook currently uses a blanket fill which should be limited to object columns).
- Derive helpful columns (e.g., `Country`, `Start_Month`) and compute aggregates like top countries and monthly start counts.
- Create visualizations using `matplotlib` and `seaborn` for distribution and comparison plots.
- Include short textual insights after each visualization.

Files in this folder
--------------------
- `covid19_clinical_trials.ipynb` — main notebook containing the EDA and plots.
- `COVID clinical trials.csv` — dataset used by the notebook (CSV extract).
- `README.md` — this file.
- `requirements.txt` — Python package list for reproducibility.

Requirements
------------
Install the packages below (recommended in a venv or conda env):

```bash
pip install -r requirements.txt
```

Minimum packages used:

- pandas
- numpy
- matplotlib
- seaborn

How to run
----------
1. Open the Jupyter Notebook `covid19_clinical_trials.ipynb` in JupyterLab or Notebook.
2. Ensure `COVID clinical trials.csv` is in the same folder.
3. Run the cells top-to-bottom. Inspect outputs and saved figures (cells display plots inline).


Contact / Author
----------------
Author: Mohammad Iqbal Hurrah

License / Attribution
---------------------
Dataset source: ClinicalTrials.gov (CSV extract) — cite appropriately when submitting.
