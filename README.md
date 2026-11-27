# New Zealand Electricity Generation Analysis (2010–2025)

An independent data analytics project examining changes in New Zealand's electricity generation mix between 2010 and 2025. Using monthly data from the Ember Energy API, this project explores generation trends by energy source, changes in renewable and fossil-fuel generation, and the development of New Zealand's renewable electricity share.

The analysis was conducted using Python and Pandas, with visualisations developed in Python and Tableau Public.

## Project Overview

New Zealand relies heavily on renewable electricity generation, particularly hydropower. However, the contribution of different generation sources changes over time due to variations in renewable availability, demand and the wider electricity system.

This project analyses historical electricity generation data to understand how New Zealand's generation mix has evolved and how the contributions of renewable and fossil-fuel sources have changed.

### Research Questions

- How has New Zealand's electricity generation mix changed between 2010 and 2025?
- How have renewable and fossil-fuel generation contributions changed over this period?
- How has the renewable share of total electricity generation evolved?
- What trends can be observed across individual electricity generation sources?

## Study Scope

| Item | Description |
|---|---|
| Country | New Zealand |
| Study period | 2010–2025 |
| Time resolution | Monthly |
| Main analysis | Annual generation trends and generation mix |
| Measurement units | TWh and percentage share |
| Data source | Ember Energy API |
| Tools | Python, Pandas, Matplotlib, SciPy and Tableau Public |

## Data Source

**Ember Energy API**

Historical electricity generation data for New Zealand was retrieved from the Ember Energy API.

The dataset contains monthly electricity generation information by source, which was used to investigate changes in the national generation mix.

The data was processed in Python before being aggregated into annual summaries for further analysis and visualisation.

## Methodology

The project followed the following analytical workflow:

1. Retrieved historical monthly electricity generation data for New Zealand using the Ember Energy API.
2. Inspected the dataset structure, time coverage, missing observations and data consistency.
3. Prepared the data for analysis and organised generation by energy source.
4. Aggregated monthly generation into annual totals.
5. Calculated the percentage contribution of generation sources to total electricity generation.
6. Compared renewable and fossil-fuel generation trends over the study period.
7. Used statistical analysis, including Pearson correlation, to explore relationships between annual generation measures.
8. Developed visualisations in Python and an interactive Tableau dashboard to communicate the findings.

## Key Findings

### 1. Growth in Renewable Electricity Share

New Zealand's renewable share of electricity generation increased from approximately **74.79% in 2010 to 88.41% in 2025**.

This represents an increase of approximately 13.6 percentage points over the study period.

### 2. Total Electricity Generation Remained Broadly Stable

Total annual electricity generation was approximately:

- **2010:** 41.77 TWh
- **2025:** 41.57 TWh

Despite changes in the generation mix, total annual generation remained broadly stable over the period.

### 3. Changes Across Generation Sources

The analysis identified several changes in the generation mix:

- Hydropower remained a major contributor to New Zealand's electricity generation.
- Wind and other renewable generation increased.
- Gas and coal generation decreased over the study period.
- Solar generation reached approximately 0.81 TWh in 2025.

Solar data was available from 2015 onwards, so a direct comparison with 2010 was not possible.

### 4. Statistical Analysis

Pearson correlation was used to investigate linear relationships between annual generation measures.

Correlation results describe statistical association and should not be interpreted as evidence of causation.

## Data Quality and Limitations

Data quality was considered throughout the analysis. The following limitations were identified:

- **Missing coal observation:** One monthly coal-generation observation was missing for September 2020. It was retained as missing rather than being replaced with zero or an estimated value.
- **Incomplete annual coal coverage:** The 2020 annual coal total therefore represents 11 available months.
- **Solar data coverage:** Solar observations begin in 2015, limiting comparisons across the full 2010–2025 period.
- **Data aggregation:** Small differences may occur between aggregated generation totals and source-reported totals. Original source values were retained rather than manually adjusted.

These limitations should be considered when interpreting annual comparisons and generation trends.

## Tools and Technologies

| Tool | Application |
|---|---|
| Python | Data retrieval and analysis |
| Pandas | Data cleaning, transformation and aggregation |
| Matplotlib | Data visualisation |
| SciPy | Statistical analysis |
| Ember Energy API | Historical electricity generation data |
| Tableau Public | Interactive dashboard development |
| Jupyter Notebook | Analysis workflow and documentation |

## Repository Contents

```text
nz-electricity-generation-analysis/
│
├── EmberEnergy.ipynb
│   └── Main notebook containing data retrieval,
│       data preparation, analysis and visualisation
│
├── NZ_annual_generation_summary.csv
│   └── Annual electricity generation summary
│
├── .gitignore
│   └── Excludes local and sensitive files
│
└── README.md
    └── Project documentation
```

## How to Use

1. Clone or download this repository.
2. Open `EmberEnergy.ipynb` using Jupyter Notebook or JupyterLab.
3. Configure your Ember API key locally, using the `EmberKey.txt` file expected by the notebook.
4. Run the notebook cells to retrieve and process the data and reproduce the analysis.

**Important:** The API key file is not included in the public repository. Keep your personal API credentials private and do not upload them to GitHub.

The annual summary CSV is included to provide the processed dataset used for the annual analysis.

## Interactive Dashboard

Explore the interactive Tableau dashboard:

**[View the Tableau Public Dashboard]** (https://public.tableau.com/app/profile/shivani.singh2458/viz/NewZealandElectricityGenerationDashboard20102025/Dashboard1)

The dashboard presents visual comparisons of New Zealand's electricity generation by source, including renewable and fossil-fuel trends over time.

## Project Focus

This project demonstrates the application of data analytics to the New Zealand electricity sector, combining historical data retrieval, data preparation, statistical analysis and visualisation to investigate long-term changes in electricity generation.
