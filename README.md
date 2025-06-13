
# Retail Sales Data Analysis
<img alt="CI logo" src="https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png">
---

## Dataset Content

This project uses the [Retail Sales Dataset](https://www.kaggle.com/datasets/manjeetsingh/retaildataset), which contains historical weekly sales data for 45 stores across different regions in the US. The dataset includes:
- Store information (type, size, region)
- Weekly sales by department and store
- Features such as holidays, promotional markdowns, temperature, fuel price, CPI, and unemployment

All files are under 100MB and suitable for GitHub repository storage.

---

## Business Requirements

- Identify sales trends and seasonal patterns
- Assess the impact of holidays and promotional markdowns on sales
- Compare sales performance across stores and departments
- Provide actionable insights for retail managers to optimise promotions and inventory

---

## Hypothesis and How to Validate

**Hypotheses:**
1. Sales increase significantly during holiday weeks.
2. Promotional markdowns lead to higher sales, especially during holidays.
3. Larger stores (by size/type) have higher average sales.

**Validation:**
- Use descriptive statistics, boxplots, and time series analysis to compare sales during holidays vs. non-holidays.
- Analyse sales before and after markdown events.
- Compare average sales by store type and size.

---

## Project Plan

- **Data Collection:** Downloaded and organised the dataset from Kaggle.
- **Data Processing:** Cleaned missing values, converted data types, and engineered features (e.g., holiday flag).
- **Analysis:** Performed exploratory data analysis and visualisation.
- **Interpretation:** Summarised findings and mapped them to business requirements.
- **Presentation:** Documented the process and results in a Jupyter notebook and this README.

**Data Management:**  
Data was kept in CSV format, loaded and processed with pandas, and all transformations were documented in the notebook.

**Methodology Rationale:**  
A combination of descriptive and visual analytics was chosen for clarity and accessibility to both technical and non-technical stakeholders.

---

## Mapping Business Requirements to Data Visualisations

| Business Requirement                        | Visualisation Type                | Rationale                                      |
|----------------------------------------------|-----------------------------------|------------------------------------------------|
| Identify sales trends                        | Line plot of weekly sales         | Shows seasonality and trends over time         |
| Impact of holidays/markdowns                 | Boxplot, bar chart                | Compares sales distributions                   |
| Compare store/department performance         | Bar chart, violin plot            | Highlights top/bottom performers               |
| Correlation between features and sales       | Heatmap, pair plot                | Reveals relationships between variables        |

---

## Analysis Techniques Used

- **Descriptive statistics** for summarising sales data
- **Time series analysis** for trend detection
- **Boxplots and violin plots** for distribution comparison
- **Correlation heatmaps and pair plots** for feature relationships
- **Interactive visualisations** using Plotly for deeper exploration

**Limitations:**  
- Data is limited to historical records and may not reflect future trends.
- Some features may have missing or zero values, which could affect analysis.

**Alternative Approaches:**  
- Predictive modelling (not covered in this project)
- More granular analysis by region or department

**Use of Generative AI:**  
- Used AI tools for ideation, code optimisation, and documentation drafting.

---

## Ethical Considerations

- No personal or sensitive data is present in the dataset.
- Analysed data for fairness and checked for potential bias in store types or regions.
- All data used is publicly available and complies with Kaggle’s terms of use.

---

## Dashboard Design

- **Overview Page:** Key metrics and sales trends
- **Store Comparison:** Sales by store and type
- **Holiday Impact:** Sales during holidays vs. non-holidays
- **Markdown Analysis:** Effect of promotions on sales
- **Interactivity:** Filters for date range, store, and department

**Communication:**  
Visualisations are designed with clear titles, labels, and tooltips to make insights accessible to both technical and non-technical audiences.

---

## Unfixed Bugs

- No major unfixed bugs at this time.
- Some minor display issues may occur with very large datasets in the dashboard.
- Feedback from peers led to improvements in data cleaning and visualisation clarity.

---

## Development Roadmap

- **Challenges:** Handling missing values, merging datasets, and ensuring visual clarity.
- **Strategies:** Iterative cleaning, regular code reviews, and peer feedback.
- **Next Steps:** Explore predictive modelling and deploy an interactive dashboard.

---

## Deployment

- The project is not deployed as a web app, but all code and notebooks are available in this repository.
- For large datasets, users should download data from Kaggle and place it in the `data/` folder as described above.

---

## Main Data Analysis Libraries

- `pandas` for data manipulation
- `numpy` for numerical operations
- `matplotlib` and `seaborn` for static visualisations
- `plotly` for interactive charts

**Example:**
```python
import pandas as pd
sales = pd.read_csv('data/sales_data.csv')
```

---

## Credits

**Content:**  
- Dataset from [Kaggle](https://www.kaggle.com/datasets/manjeetsingh/retaildataset)
- Code examples and visualisation ideas inspired by official documentation and open-source tutorials

**Media:**  
- CI logo from Code Institute

**Acknowledgements:**  
- Thanks to instructors, peers, and the Code Institute community for support and feedback.

---