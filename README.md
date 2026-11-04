Data-Driven Sales Demand Analysis for Inventory Planning and Operational Efficiency

Project Overview

This project analyses historical point-of-sale data from Melt Gelato, a retail gelato and café business in Navan, Ireland.

The objective was to understand sales demand patterns, identify important products, evaluate forecasting methods, and develop data-driven recommendations for inventory planning and operational efficiency.

The project was completed as part of the IIT Madras Business Data Management Capstone.

Objectives

* Analyse historical sales trends and customer demand patterns.
* Examine relationships between weather conditions and daily sales.
* Develop and compare daily revenue forecasting models.
* Identify high-revenue products using ABC classification.
* Explore frequently purchased product combinations.
* Evaluate demand variability across product categories.
* Translate analytical findings into practical business recommendations.

Tools and Technologies

Programming: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

Business Intelligence: Power BI

Methods: Exploratory Data Analysis, Correlation Analysis, Ridge Regression, Time-Series Forecasting, ABC Classification, Market Basket Analysis

Project Structure

The analysis is organised into seven Jupyter notebooks:

Notebook	Description
01 - Data Understanding	Examines the dataset structure, completeness and initial data quality.
02 - Data Cleaning	Prepares sales records and handles payment, refund and void transactions.
03 - Exploratory Data Analysis	Investigates sales patterns across dates, hours, weekdays and product categories.
04 - Weather and Sales Analysis	Examines relationships between historical weather conditions and daily revenue.
05 - Sales Forecasting	Compares forecasting models using chronological training and testing data.
06 - Product and Inventory Analysis	Performs product rankings, ABC classification, market basket analysis and category demand variability analysis.
07 - Business Recommendations	Converts analytical findings into practical operational recommendations.

Key Findings

Sales Forecasting

Three forecasting approaches were evaluated:

Model	WAPE
Calendar Ridge Regression	12.74%
Calendar + Observed Weather Ridge	15.03%
Seasonal Naïve	18.83%

Calendar Ridge Regression achieved the lowest forecasting error on the test period.

Product Revenue Concentration

ABC classification identified a concentration of revenue among a relatively small group of products.

* Category A: 44 products contributing 80.45% of payment revenue.
* Category B: 61 products contributing 14.58%.
* Category C: 282 products contributing 4.97%.

Operational Insights

The analysis identified recurring weekly demand patterns, differences in category-level revenue variability, and product combinations that may be useful for operational planning.

Business Recommendations

The project explored opportunities to:

* Prioritise monitoring of high-revenue products.
* Use historical demand patterns to support staffing and inventory planning.
* Adjust preparation levels for categories with variable demand.
* Evaluate potential product combinations and promotional opportunities.
* Introduce further testing before implementing forecasting models in daily operations.

Data Confidentiality

The original point-of-sale dataset contains confidential business information and is not included in this repository.

Raw data, processed transaction-level files, and other sensitive business records are excluded.

The notebooks are provided to demonstrate the analytical methodology and project workflow. They may require access to the original private datasets to execute successfully.

Limitations

The analysis was based primarily on historical sales data.

Inventory quantities, product costs, wastage and staffing records were not available for directly measuring the financial impact of the recommendations.

The forecasting results were evaluated on a historical test period and would require further validation before operational deployment.

Author

Aakriti Abhay Singh

MSc Data & Computational Science, University College Dublin

B.Tech Data Science & Engineering, Manipal University Jaipur

BSc Data Science & Programming, IIT Madras