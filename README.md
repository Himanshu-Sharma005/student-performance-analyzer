# Student Performance Analyzer

A comprehensive Python-based data science project that generates synthetic student records, cleans the data, integrates it with an SQLite database, conducts advanced statistics using Pandas, and generates visualization charts alongside an automated HTML dashboard summary report.

---

## Features

- **Synthetic Data Generation**: Creates a realistic student dataset (200 records + duplicate entries for cleaning) using NumPy normal and uniform distributions.
- **Deduplication & Validation**: Standardizes types, scans for null values, and drops duplicates to ensure data integrity.
- **SQL Database Integration**: Loads data into an SQLite database to perform relational queries (e.g., gender averages, bottom/top performers, passing students with low attendance).
- **Pandas Analytical Metrics**: Computes Pearson correlation coefficients, at-risk classifications, and value counts.
- **Polished Visualizations**: Exports 6 distinct matplotlib and seaborn plots (including bar charts, histograms, scatter plots, pie charts, and correlation heatmaps) saved at high resolution.
- **Automated HTML Dashboard Report**: Automatically generates a clean, styled HTML report displaying key metrics and embedding the visualization plots.

---

## Repository Structure

```text
├── Student_Performance_Analyzer.ipynb  # Main Jupyter Notebook
├── students.csv                        # Raw dataset with duplicates
├── student_records.db                  # Cleaned SQLite database
├── summary_report.html                 # Automatically generated HTML dashboard
├── .gitignore                          # Exclusions for cache and DB files
├── README.md                           # Project documentation
└── *.png                               # Exported visualization plots
```

---

## Technology Stack

- **Language**: Python 3.11+
- **Data Engineering**: `numpy`, `pandas`
- **Database Engine**: `sqlite3` (built-in)
- **Data Visualization**: `matplotlib`, `seaborn`
- **Notebook Environment**: `jupyter`, `ipykernel`

---

## Setup & Installation

Follow these steps to run the project locally:

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPO.git
cd YOUR-REPO
```

### 2. Install Dependencies
Ensure you have Python installed, then run:
```bash
pip install pandas numpy matplotlib seaborn notebook ipykernel
```

### 3. Open the Jupyter Notebook
Start Jupyter Notebook to run or edit the analysis:
```bash
jupyter notebook Student_Performance_Analyzer.ipynb
```
Alternatively, you can open the folder in **VS Code** and open the `.ipynb` file using the VS Code Jupyter extension.

---

## Viewing the Live Report

After running the notebook, a self-contained dashboard report named **`summary_report.html`** is compiled in your workspace directory. You can open this file directly in any web browser (Chrome, Firefox, Edge, Safari) to view:
- Key KPI metrics (Overall pass percentage, top performing subject, count of at-risk students).
- A styled descriptive statistics table of the dataset.
- All 6 interactive visualization plots.
