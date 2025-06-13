<img alt="CI logo" src="https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png">

# Data Analytics with AI: Python ETL and Visualisation

## Project Overview

This project analyses retail sales data from 45 stores across different regions. The aim is to identify sales trends, understand the impact of promotional markdowns and holidays, and compare store performance. The insights will help retail managers and analysts make data-driven decisions.

**Data Source:**  
[Retail Sales Dataset on Kaggle](https://www.kaggle.com/datasets/manjeetsingh/retaildataset)

---

## Project Steps

### 1. Ideation & Project Proposal
- **What:** The project focuses on analysing historical sales data to uncover trends and the effects of promotions and holidays.
- **Why:** Retailers need to understand how events and markdowns affect sales to optimise inventory and marketing strategies.
- **How:** I chose this project because it aligns with my interest in retail analytics and my goal to become a data analyst.

### 2. Data Extraction (ETL - Extract)
- **What:** Loaded three CSV files: `stores_data.csv`, `features_data.csv`, and `sales_data.csv`.
- **Why:** These files contain all the necessary information about stores, weekly sales, and additional features like markdowns and holidays.
- **How:** Used `pandas.read_csv()` to import the datasets into DataFrames for analysis.

### 3. Data Cleaning & Transformation (ETL - Transform)
- **What:** Checked for missing values, converted date columns, and ensured correct data types.
- **Why:** Clean data is essential for accurate analysis and visualisation.
- **How:** Filled missing values with zeros, converted `Date` columns to datetime, and created a holiday flag for analysis.

### 4. Data Loading (ETL - Load)
- **What:** Stored the cleaned and transformed data in DataFrames and saved them as new CSV files.
- **Why:** This ensures the data is ready for analysis and can be reused or shared.
- **How:** Used `DataFrame.to_csv()` to save cleaned data and kept DataFrames in memory for further steps.

### 5. Exploratory Data Analysis & Basic Visualisations
- **What:** Calculated average sales per store and department, and plotted total weekly sales over time.
- **Why:** To get an initial understanding of the data and spot any trends or anomalies.
- **How:** Used `groupby()` for aggregation and `matplotlib`/`seaborn` for plotting line and bar charts.

### 6. Advanced Visualisations
- **What:** Created a correlation heatmap, pair plots, violin plots by store type, and interactive sales trends.
- **Why:** These visualisations help uncover deeper relationships and present findings in an engaging way.
- **How:** Used `seaborn` for static advanced plots and `plotly` for interactive charts.

### 7. Documentation & Presentation
- **What:** Documented each step of the ETL and analysis process, and summarised key findings.
- **Why:** Good documentation ensures reproducibility and clear communication of insights.
- **How:** Maintained this README, added comments in the code, and prepared a summary presentation with screenshots of key visualisations.

### 8. Version Control & Project Management
- **What:** Used GitHub for version control and a Kanban board for task management.
- **Why:** To track progress, manage tasks, and ensure transparency.
- **How:** Committed code regularly to GitHub and used GitHub Projects to organise user stories and milestones.

---

## How to Reproduce

1. Clone this repository.
2. Install dependencies from `requirements.txt`.
3. Place the raw data files in the `data/` directory.
4. Open and run the Jupyter notebook step by step.

---

## Key Findings

- Sales tend to spike during holiday weeks, especially when promotional markdowns are applied.
- Certain store types consistently outperform others in terms of weekly sales.
- There is a strong correlation between markdown events and increased sales volume.
- Some departments are more sensitive to promotions and holidays than others.

---

## References

- [Retail Sales Dataset on Kaggle](https://www.kaggle.com/datasets/manjeetsingh/retaildataset)

---

## Contact

For questions, contact [Midaso] at [midasobona@yahoo.com].