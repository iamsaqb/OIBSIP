# OIBSIP Task 1: Exploratory Data Analysis on Retail Sales

## Project Overview
This project focuses on exploring retail sales data to identify sales trends, understand product performance, examine profitability, and study relationships between numerical variables.

The analysis was completed using Python in Jupyter Notebook as part of the Oasis Infobyte Internship Program (OIBSIP).

## Objectives
- Analyze monthly sales trends.
- Compare total sales across product categories.
- Examine profit across product sub-categories.
- Investigate correlations between sales, quantity, discount, and profit.
- Communicate findings through data visualizations.

## Tools and Technologies
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Project Structure
- `notebooks/` — Jupyter Notebook containing the analysis.
- `data/` — Dataset, if redistribution is permitted.
- `visuals/` — Exported charts, if included.
- `requirements.txt` — Required Python libraries.

## Key Findings
- November 2017 recorded the highest monthly sales in the analyzed dataset, at approximately **118,447.82**.
- February 2014 recorded the lowest monthly sales, at approximately **4,519.89**.
- Sales and profit had a moderate positive correlation of **0.48**.
- Discount and profit had a weak negative correlation of **-0.22**.
- Sales and discount had a near-zero correlation of **-0.03**.

*Note: Correlation indicates association, not causation. The results do not establish that discounts directly caused changes in profit.*

## Methodology
1. Loaded the retail sales dataset using Pandas.
2. Inspected the data structure and checked data quality.
3. Converted order dates to datetime format.
4. Grouped sales by month and product category.
5. Aggregated profit by product sub-category.
6. Calculated correlations among selected numerical variables.
7. Created charts using Matplotlib and Seaborn.
8. Interpreted the results to identify potential business insights.

## How to Run
1. Clone or download this repository.
2. Install the required libraries:
   `pip install -r requirements.txt`
3. Open the notebook in Jupyter Notebook or JupyterLab.
4. Ensure the dataset is available at the path used in the notebook.
5. Run the notebook cells in order.

## Conclusion
This project demonstrates how exploratory data analysis can turn retail transaction data into meaningful insights. The analysis provides an overview of monthly sales patterns, product performance, profitability, and relationships between key numerical variables.

## Internship
**Program:** Oasis Infobyte Internship Program (OIBSIP)  
**Task:** Task 1 — Exploratory Data Analysis on Retail Sales Data

