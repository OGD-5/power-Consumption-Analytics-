# Morocco Electricity Consumption and Environmental Factors Analysis

## Project Overview

This project explores electricity consumption patterns and their relationship with environmental factors across three geographical zones in Morocco.

The analysis uses 10-minute electricity consumption and weather records covering January 1 to December 30, 2017, comprising 52,416 observations.

The project was completed as part of the **AnalystLab Africa Experience Lab Internship Programme, Week 5, Data Analytics Track**.

The primary objective was to understand how electricity demand varies across geographical zones, time periods, seasons, and changing weather conditions, and translate those patterns into useful recommendations for energy management.

## Business Problem

Understanding electricity demand is essential for effective grid management, infrastructure planning, and reliable energy distribution.

However, demand does not remain constant. It changes throughout the day, across weekdays and weekends, between seasons, and under different environmental conditions.

This project investigates these patterns to help an energy management organisation:

- Understand electricity consumption across different geographical zones.
- Identify periods of peak and low electricity demand.
- Examine seasonal and weekly demand variations.
- Investigate relationships between electricity consumption and weather variables.
- Identify potential grid management challenges.
- Develop practical recommendations for demand management and infrastructure planning.

## Dataset Description

The dataset contains 10-minute electricity consumption and weather observations across three geographical zones in Morocco.

| Attribute | Description |
|---|---|
| Country | Morocco |
| Coverage period | January 1 – December 30, 2017 |
| Observations | 52,416 |
| Geographical coverage | Three zones |
| Data frequency | 10-minute intervals |
| Data categories | Electricity consumption and environmental variables |

### Repository Contents

- `Morocco_Electricity_Consumption_Analysis.ipynb`: Complete Jupyter Notebook containing the analytical workflow.
- `powerconsumption.csv`: Original dataset.
- `powerconsumption_datadictionary.csv`: Variable definitions.
- `cleaned_powerconsumption.csv`: Processed dataset with additional time-based features and derived measures.
- `charts/`: High-resolution visualisations generated during the analysis.
- `Morocco_Electricity_Consumption_Report.pdf`: Executive analytical report.

## Tools and Technologies

| Tool | Purpose |
|---|---|
| Python | Main programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical operations |
| Matplotlib | Data visualisation |
| Seaborn | Statistical visualisation |
| Plotly | Interactive visualisation |
| Jupyter Notebook | Analysis environment |

## Analytical Workflow

### 1. Data Inspection and Understanding
- Examined the dataset structure and variable definitions.
- Reviewed data types, missing values, and general data quality.
- Investigated the distribution of consumption and weather variables.

### 2. Data Cleaning and Preparation
- Processed timestamps into appropriate datetime formats.
- Reviewed and prepared the dataset for analysis.
- Created additional calendar-related variables.
- Prepared the data for zone-level and time-based comparisons.

### 3. Feature Engineering

Created additional features to support deeper analysis, including:

- Year
- Month
- Day
- Hour
- Day of Week
- Date
- Total grid demand
- Derived 10-minute energy consumption measures

### 4. Exploratory Data Analysis

Investigated:

- Electricity consumption across the three geographical zones.
- Hourly and daily consumption patterns.
- Weekday versus weekend demand.
- Monthly and seasonal consumption variations.
- Relationships between electricity demand and environmental variables.

### 5. Statistical and Correlation Analysis

Used descriptive statistics and Pearson correlation analysis to investigate relationships between electricity demand, temperature, humidity, and wind speed.

### 6. Visualisation and Reporting

Developed visualisations to communicate consumption patterns, zone-level differences, seasonal changes, and environmental relationships.

The analysis was also summarised in an executive report with practical recommendations.

## Key Findings

### 1. Zone 1 Accounts for the Largest Share of Electricity Demand

Zone 1 recorded the highest average demand, contributing approximately 45.41% of total grid demand. Zone 2 accounted for 29.54%, while Zone 3 contributed 25.04%.

Zone 3, despite having the lowest annual average, experienced considerable seasonal variation.

### 2. Evening Hours Record the Highest Electricity Demand

Demand followed a consistent daily pattern, with the lowest average recorded around 6:00 AM.

Consumption increased throughout the day, reaching its highest average around 8:00 PM.

This highlights the importance of understanding evening peak-demand periods when planning grid capacity.

### 3. Weekly Consumption Patterns Differ Across Zones

Overall demand was higher during the working week and declined towards the weekend.

Zones 1 and 2 experienced more noticeable Sunday reductions, while Zone 3 maintained relatively stable weekend demand.

These differences suggest that the zones may have distinct consumption profiles and require tailored demand-management strategies.

### 4. Electricity Demand Increases During the Summer Months

July and August recorded the highest average electricity demand, while November and December experienced lower demand levels.

This seasonal variation highlights the importance of preparing for increased grid pressure during hotter months.

### 5. Temperature Has the Strongest Weather Relationship with Electricity Demand

Temperature recorded a moderate positive Pearson correlation with total demand (r = 0.488).

Humidity showed a weak negative relationship (r = -0.299), while wind speed had a relatively weak positive relationship (r = 0.222).

The analysis also showed higher average demand under hotter temperature conditions.

These relationships indicate that environmental conditions are relevant to electricity demand, although correlation alone does not establish causation.

## Business Implications

The findings suggest several important considerations for energy management:

- Grid capacity planning should account for geographical differences in electricity demand.
- Evening peak periods require particular attention.
- Seasonal demand variations should inform infrastructure and maintenance planning.
- Temperature information can support demand forecasting and reserve planning.
- Different geographical zones may require different demand-management approaches.

## Recommendations

### 1. Introduce Time-of-Use Tariffs and Peak-Shaving Incentives

Consider demand-management incentives that encourage flexible electricity users to shift consumption away from the evening peak period, particularly between 7:00 PM and 9:00 PM.

### 2. Schedule Preventive Grid Maintenance Strategically

Where operational conditions permit, schedule routine maintenance during periods of lower electricity demand and avoid unnecessary infrastructure downtime during high-demand summer periods.

### 3. Introduce Temperature-Triggered Summer Reserve Planning

Incorporate weather forecasts into energy planning, particularly during the summer months, to anticipate potential increases in electricity demand.

### 4. Standardise Data Logging Definitions

Ensure that metering systems clearly document measurement units, sampling intervals, and variable definitions.

In particular, distinguish between average power demand measured in kW and energy consumption measured in kWh. This helps prevent errors in energy calculations and future forecasting models.

## Key Learning Outcomes

Through this project, I strengthened my practical understanding of:

- Data cleaning and preprocessing with Pandas.
- Feature engineering using datetime variables.
- Exploratory data analysis.
- Statistical summaries and correlation analysis.
- Time-based and geographical comparisons.
- Data visualisation with Matplotlib, Seaborn, and Plotly.
- Translating analytical findings into business recommendations.

## How to Reproduce the Analysis

### Prerequisites

Install Python 3.10 or later.

Install the required libraries:

```bash
pip install notebook pandas numpy matplotlib seaborn plotly
```

### Run the Notebook

1. Clone or download this repository.
2. Ensure the dataset files are in the appropriate project directory.
3. Open the Jupyter Notebook:

```bash
jupyter notebook
```

4. Open `Morocco_Electricity_Consumption_Analysis.ipynb`.
5. Run the notebook cells sequentially.

## Conclusion

This project demonstrates how exploratory data analysis can uncover meaningful patterns in electricity consumption and environmental data.

By examining demand across geographical zones, time periods, and weather conditions, the analysis provides useful insights that can support energy planning, grid management, and more informed operational decisions.

**Project completed as part of the AnalystLab Africa Experience Lab Internship Programme, Week 5, Data Analytics Track.**
