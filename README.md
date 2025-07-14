# Drivers Crash Analysis in Maryland (USA)

## Project Overview

This project conducts an **Exploratory Data Analysis (EDA)** on traffic crash data from Maryland, USA, to uncover patterns and insights that can enhance road safety. The analysis focuses on understanding the impact of environmental conditions (weather, road surface, lighting) and temporal factors (hour, weekday) on crash severity and driver fault. The goal is to provide actionable insights for traffic authorities, urban planners, and policymakers to design preventive measures and improve public awareness.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Analysis](#analysis)
- [Conclusions and Suggestions](#conclusions-and-suggestions)
- [Next Steps](#next-steps)
- [References](#references)
- [Versioning](#versioning)

## Introduction

Traffic accidents are a significant public safety concern, with thousands of crashes occurring annually in Maryland. This project aims to:
- Analyze how **weather**, **surface conditions**, and **time factors** affect crash severity and driver responsibility.
- Identify when crashes are most likely to occur and assess their severity.

The analysis is performed using Python in a Jupyter Notebook environment, leveraging libraries such as Pandas, NumPy, Matplotlib, Seaborn, and Plotly for data processing and visualization.

## Dataset

The dataset is sourced from [data.montgomerycountymd.gov](https://catalog.data.gov/dataset/crash-reporting-drivers-data) and contains thousands of traffic crash records from Maryland. Each record includes details such as:
- Crash date and time
- Location (latitude, longitude, road name)
- Environmental conditions (weather, surface condition, lighting)
- Driver details (substance abuse, distraction, fault)
- Crash outcomes (injury severity, vehicle damage)

**Key Features:**
- **Rows**: 196,043
- **Columns**: 39
- **Format**: CSV
- **Source**: Montgomery County, Maryland (accessed June 5, 2025)

## Installation

To run the analysis, ensure you have Python 3.12 or later installed. Follow these steps:

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   
2. Install Required Libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly

3. **Prepare the Dataset**:
   - Download the dataset (`Crash_Reporting_-_Drivers_Data.csv`) from the source.
   - Place it in the project directory or update the file path in the notebook (`Ashutosh_Behera_EDA.ipynb`).

## Usage Instructions

1. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook Ashutosh_Behera_EDA.ipynb
   ```

2. **Run the Notebook**:
   - Execute the cells in sequence to:
     - Load and preprocess the dataset.
     - Conduct exploratory data analysis (e.g., view data shape, column names, and data types).
     - Generate visualizations such as heatmaps, bar charts, and pie charts.
     - Answer key research questions about environmental and temporal factors.
   - Modify code or visualizations for custom analysis as needed.

3. **Dependencies**:
   - Python libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `plotly`, `python-dateutil`, `datetime`.

## Analysis Overview

The analysis is organized into the following sections:

1. **Data Acquisition and Loading**:
   - Loaded the CSV dataset using Pandas.
   - Displayed basic data characteristics, including shape (196,043 rows, 39 columns) and column names.

2. **Data Preprocessing**:
   - Handled missing values by filling string-based columns with "NA".
   - Parsed and standardized datetime fields into separate columns: Crash Date, Crash Time, and Hour.
   - Dropped irrelevant or inconsistent columns to streamline analysis.
   - Converted data types as needed (e.g., ensured Hour is an integer).

3. **Exploratory Data Analysis**:
   - Visualized crash patterns using:
     - **Heatmaps**: To show crash frequency by hour and weekday.
     - **Bar and Pie Charts**: To explore relationships between weather, surface conditions, lighting, and crash severity.
   - Used libraries like Seaborn and Plotly for interactive and clear visualizations.

4. **Research Questions**:
   - **Question 1**: How do weather and surface conditions affect the severity of traffic crashes and driver responsibility?
   - **Question 2**: When are crashes most likely to occur, and how severe are they?

## Key Findings and Recommendations

### Research Question 1: Impact of Environmental Conditions
- **Findings**:
  - Adverse weather (e.g., rain, snow) and poor road surface conditions (e.g., wet or icy roads) are associated with increased crash severity.
  - Poor lighting conditions (e.g., nighttime or dusk) correlate with higher driver fault rates.
- **Recommendations**:
  - Enhance **road maintenance** during adverse weather to improve surface conditions.
  - Implement **real-time driver alerts** via mobile apps or signage to warn of hazardous conditions.
  - Enforce **temporary speed limits** during poor weather or low-visibility periods.

### Research Question 2: Temporal Patterns of Crashes
- **Findings**:
  - Crashes are most frequent during **peak commuting hours** (e.g., 7–9 AM, 4–7 PM) on weekdays, particularly Monday through Friday.
  - Crash severity tends to increase in the **evening hours**, likely due to fatigue, reduced visibility, or higher traffic density.
- **Recommendations**:
  - Optimize **traffic signal timings** to reduce congestion during peak hours.
  - Increase **police patrols** during high-risk periods (e.g., evening commuting hours).
  - Launch **public awareness campaigns** to promote safe driving practices during evenings.

## Future Work

- **Time-Series Forecasting**: Develop machine learning models to predict future crash trends based on historical data.
- **Geospatial Analysis**: Use latitude and longitude data to map crash hotspots and identify high-risk areas.
- **Expanded Data Integration**: Incorporate additional datasets, such as traffic volume or driver demographics, for a more comprehensive analysis.
- **Causal Analysis**: Explore causal relationships between variables using statistical or machine learning techniques.

## References

1. Montgomery County, Maryland. *Crash Reporting - Drivers Data*. Available at: [https://catalog.data.gov/dataset/crash-reporting-drivers-data](https://catalog.data.gov/dataset/crash-reporting-drivers-data) (Accessed: June 5, 2025).

## Version History

- **Version 1.0** (July 2025): Initial release of the EDA, including data loading, preprocessing, visualization, and insights on environmental and temporal factors.
- **Future Updates**: Planned enhancements include predictive modeling, geospatial analysis, and integration of additional datasets.
