# New Zealand Electricity Generation Analysis (2010–2025)

## Project Overview

This project analyses changes in New Zealand's electricity generation mix between 2010 and 2025 using monthly electricity generation data from Ember Energy.

The analysis investigates how electricity generation has changed over time, with a particular focus on the transition between renewable and fossil-fuel generation sources.

Python was used for data retrieval, cleaning, exploration, analysis and visualisation. The findings were also presented through an interactive Tableau dashboard.

## Research Question

How has New Zealand's electricity generation mix changed between 2010 and 2025, and what trends can be observed in renewable and fossil-fuel generation?

## Project Objectives

- Examine long-term trends in New Zealand's electricity generation.
- Compare generation from individual energy sources.
- Analyse changes in renewable and fossil-fuel generation.
- Measure changes in the renewable share of total electricity generation.
- Investigate the relationship between renewable and fossil-fuel generation.
- Communicate the findings through data visualisations and an interactive dashboard.

## Data Source

**Source:** Ember Energy API  
**Country:** New Zealand  
**Entity code:** NZL  
**Study period:** January 2010 – December 2025  
**Original data frequency:** Monthly  
**Measurement:** Terawatt-hours (TWh) and percentage share of generation.

The dataset includes generation from hydro, wind, solar, bioenergy, coal, gas and other generation sources.

## Tools and Technologies

- **Python:** Data retrieval, cleaning, analysis and visualisation.
- **Pandas:** Data manipulation and aggregation.
- **NumPy:** Numerical operations.
- **Matplotlib:** Data visualisation.
- **SciPy:** Pearson correlation analysis.
- **Jupyter Notebook:** Analysis workflow and documentation.
- **Tableau Public:** Interactive data dashboard.

## Methodology

The project followed these main steps:

1. **Data retrieval:** Obtained monthly electricity generation data through the Ember Energy API.
2. **Data cleaning:** Inspected data types, missing values, duplicate records and date coverage.
3. **Data preparation:** Separated individual generation sources from aggregate categories and prepared annual generation summaries.
4. **Trend analysis:** Examined annual generation trends and compared individual energy sources between 2010 and 2025.
5. **Renewable and fossil-fuel analysis:** Calculated annual generation and generation shares for renewable and fossil-fuel categories.
6. **Statistical analysis:** Used Pearson correlation to examine the relationship between annual renewable and fossil-fuel generation.
7. **Visualisation:** Created charts in Python and developed an interactive Tableau dashboard.

## Key Findings

### 1. Total Electricity Generation

Total annual electricity generation remained relatively stable over the study period.

- 2010: 41.77 TWh
- 2025: 41.57 TWh
- Overall change: approximately -0.48%.

### 2. Renewable Generation Share

The renewable share of electricity generation increased between 2010 and 2025.

- 2010: 74.79%
- 2025: 88.41%
- Increase: 13.61 percentage points.

### 3. Changes in Individual Generation Sources

Between 2010 and 2025:

- Other renewables increased by approximately 3.83 TWh.
- Wind generation increased by approximately 2.07 TWh.
- Gas generation decreased by approximately 4.26 TWh.
- Coal generation decreased by approximately 1.42 TWh.
- Hydro generation remained a major contributor to electricity supply.

Solar generation reached approximately 0.81 TWh in 2025. A direct comparison with 2010 was not possible because solar data was available from 2015 onwards.

### 4. Renewable and Fossil-Fuel Relationship

Pearson correlation analysis showed a strong negative association between annual renewable and fossil-fuel generation.

- Pearson correlation coefficient (r): approximately -0.974.
- p-value: approximately 2.22 × 10⁻¹⁰.

This indicates a strong negative linear association within the study period. The result is descriptive and does not establish causation.

## Data Visualisation

The analysis includes:

- Annual electricity generation trends.
- Generation by individual energy source.
- Renewable and fossil-fuel generation comparisons.
- Changes in generation between 2010 and 2025.
- Annual renewable generation share.
- Percentage changes in total annual generation.

## Interactive Tableau Dashboard

Explore the interactive dashboard:

[New Zealand Electricity Generation Dashboard (2010–2025)](https://public.tableau.com/app/profile/shivani.singh2458/viz/NewZealandElectricityGenerationDashboard20102025/Dashboard1#1)

## Data Quality and Limitations

- One monthly coal-generation observation was missing for September 2020. The missing value was retained rather than replaced with zero or an estimated value. Consequently, the 2020 annual coal total uses 11 available monthly observations.
- Solar generation data begins in January 2015, resulting in 132 monthly observations compared with 192 observations for the other sources.
- Small differences were identified when comparing the sum of individual generation categories with reported aggregate generation. The original values were retained without manual adjustment.
- The correlation analysis uses only 16 annual observations. The results should therefore be interpreted cautiously and should not be considered evidence of causation.

## Repository Contents

| File | Description |
|---|---|
| `EmberEnergy.ipynb` | Jupyter Notebook containing the data analysis and visualisations. |
| `NZ_annual_generation_summary.csv` | Annual electricity generation summary by source. |
| `.gitignore` | Excludes local and sensitive files from Git tracking. |

## How to Use This Project

1. Clone or download this repository.
2. Install the required Python libraries.
3. Open `EmberEnergy.ipynb` in Jupyter Notebook or JupyterLab.
4. To rerun the API data retrieval section, obtain your own Ember API key and configure it locally in `EmberKey.txt`.
5. Run the notebook cells in sequence.

**Important:** The API key is private and is not included in this repository.

## Conclusion

This project highlights the changes in New Zealand's electricity generation mix between 2010 and 2025. While total generation remained relatively stable, the renewable share increased, supported by growth in wind and other renewable generation sources.

The project demonstrates the application of Python-based data analysis, statistical techniques and visualisation to investigate trends in the New Zealand energy sector.
