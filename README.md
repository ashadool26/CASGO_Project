# Counter-Strike: Global Offensive (CS:GO) Data Analysis

A structured exploratory data analysis (EDA) project on CS:GO match/player statistics, built in Jupyter/Colab using Python data analysis and visualization libraries.

## Project Summary

This repository contains a notebook-based analytics workflow that:

- Loads and inspects a large CS:GO dataset.
- Performs foundational data quality checks (nulls, duplicates, schema review).
- Applies early feature-engineering steps.
- Uses visual analysis to explore relationships across gameplay variables.

The project is aimed at demonstrating practical EDA skills for gaming telemetry and performance datasets.

## Repository Contents

- `CSGO_Project_by_ashadool.ipynb` — Main notebook with end-to-end analysis.
- `README.md` — Project documentation.

## Dataset

The notebook references an external dataset (shared via Google Drive by the author).

- Dataset link (as documented in the notebook):
  - `https://drive.google.com/file/d/1PMoa51-JvNZ_ar8ACQSw_6g9RJJd2LOQ/view?usp=sharing`

> Note: Update local paths in the notebook (if needed) based on where you store the downloaded CSV.

## Tech Stack

- **Language:** Python
- **Environment:** Jupyter Notebook / Google Colab
- **Libraries:**
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `seaborn`

## Analysis Workflow

The notebook follows a standard analytics pipeline:

1. **Data Loading**
   - Import dataset into a DataFrame.
2. **Data Understanding**
   - Review dimensions, columns, data types, and descriptive statistics.
3. **Data Quality Validation**
   - Check for missing values and duplicate records.
4. **Data Cleaning**
   - Remove duplicates and ensure a clean working dataset.
5. **Feature Engineering**
   - Introduce/derive useful analytical fields.
6. **Visualization & Insights**
   - Generate plots to identify trends and relationships.

## How to Run

### Option 1: Google Colab

1. Open the notebook in Colab.
2. Upload/download the dataset and adjust the file path.
3. Run cells sequentially.

### Option 2: Local Jupyter Environment

1. Clone this repository:
   ```bash
   git clone <your-repo-url>
   cd CASGO_Project
   ```
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn notebook
   ```
3. Start Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
4. Open `CSGO_Project_by_ashadool.ipynb` and run all cells.

## Potential Extensions

- Build player-performance clusters (unsupervised learning).
- Add comparative analysis across maps/teams/roles.
- Create reusable dashboards (e.g., Plotly/Power BI/Tableau).
- Introduce predictive models for outcome/performance metrics.

## Author

**Ashadul Hasan**

Aspiring Data Analyst focused on practical data analytics, visualization, and real-world project development.

---

If you found this project helpful, consider starring the repository and sharing feedback.
