
# Retail Sales Data Analysis
<img alt="CI logo" src="https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png">
---
This project delivers an end-to-end ETL (Extract, Transform, Load), analysis, and visualization pipeline for a US retail sales dataset. The workflow includes robust data cleaning, insightful exploratory analysis, effective feature engineering, predictive modeling, and both static and interactive visualizations. The goal is to uncover actionable insights for retail decision-making and to demonstrate best practices in reproducible data analytics.

## Dataset Content

This project uses the [Retail Sales Dataset](https://www.kaggle.com/datasets/manjeetsingh/retaildataset), which contains historical weekly sales data for 45 stores across different regions in the US. The dataset includes:
- Store information (type, size, region)
- Weekly sales by department and store
- Features such as holidays, promotional markdowns, temperature, fuel price, CPI, and unemployment

## Business Requirements

- Identify weekly, seasonal, and holiday sales patterns
- Evaluate the impact of promotional markdowns and holidays on sales
- Compare sales performance by store type, size, and department
- Deliver actionable recommendations for retail managers to optimize inventory and promotions
---

## Hypothesis and How to Validate

**Hypotheses:**
- Holiday Effect: Sales increase significantly during holiday weeks
Validation: Line plots and boxplots comparing holiday vs. non-holiday sales

- Promotional Impact: Markdowns drive higher sales, especially during holidays
Validation: Analyze periods before/after markdowns with time series and distribution plots

- Store Size/Type: Larger stores outperform in average sales
Validation: Grouped bar/violin plots and descriptive statistics by store type/size
---

## Project Plan
- ETL and Analysis Pipeline
Data Collection: Download from Kaggle and organize in /data/
Cleaning:
- Imputed missing values using median (for MarkDowns) and mean (for economic features)
Converted date fields
- Ensured data types and consistency
- Feature Engineering:
Added month/year columns
- Encoded categorical variables for modeling
Created holiday and markdown indicators
# Analysis:
Descriptive statistics and value counts
Comparative analysis by store, department, and event (holidays/markdowns)
# Modeling:
Random Forest regression
Baseline models vs. feature-engineered models
Evaluated with R², RMSE, and MAE
# Visualization:
Static (matplotlib, seaborn) and interactive (plotly) charts
Trend, distribution, and correlation plots

**Data Management:**  
Data was kept in CSV format, loaded and processed with pandas, and all transformations were documented in the notebook.

**Methodology Rationale:**  
A combination of descriptive and visual analytics was chosen for clarity and accessibility to both technical and non-technical stakeholders.
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

# Key Findings
- Strong Seasonality: Weekly and seasonal sales trends, with pronounced spikes during holidays
- Holiday & Markdown Impact: Both drive significant sales increases, especially when combined
- Store & Department Performance: Larger stores and certain departments consistently outperform others in both total and average sales
- Feature Engineering: Improved model accuracy and interpretability (higher R², better residual plots)
- Data Cleaning Matters: Median/mean imputation for missing values produced more realistic, actionable insights and improved all visualizations and model results
# Conclusion
- The improved ETL and analytic workflow enables more reliable, actionable insights for retail planning. Careful handling of missing values and thoughtful feature engineering substantially increased the accuracy of sales forecasts and the clarity of business insights. The model now more effectively captures spikes in sales during holidays and promotions, empowering managers to optimize inventory, staffing, and marketing strategies. This project demonstrates the importance of robust data cleaning, proper visualization, and reproducible analytics in retail data science.
## Visualizations & Dashboard Design
- Overview: Key metrics and weekly/seasonal sales trends
- Store & Department Comparison: Performance visualized with bar/violin plots
- Holiday & Markdown Analysis: Distribution and trend plots for event-driven sales
- Correlation Analysis: Heatmaps and pair plots for variable relationships
- Interactivity: Plotly dashboards allow filtering by time, store, department
## Main Libraries Used
- pandas, numpy, matplotlib, seaborn, plotly, scikit-learn
## Ethical Considerations
- No personal or sensitive data used
- All data is public and compliant with Kaggle’s terms
-  Analyses checked for fairness and bias
## Development Roadmap
- Continue refining modeling (cross-validation, hyperparameter tuning)
- Develop and deploy an interactive dashboard (Plotly Dash/Streamlit)
- Explore region- and department-level predictive models

## Credits
- Dataset from [Kaggle](https://www.kaggle.com/datasets/manjeetsingh/retaildataset)
Inspiration: Open-source tutorials, official documentation, and Code Institute community
Logo: Code Institute
