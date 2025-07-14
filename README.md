# Road Crash Analysis – Exploratory Data Analysis (EDA)
Author: Ashutosh Behera
Project Type: Exploratory Data Analysis (EDA)
Dataset: Crash_new_dataset2.csv
Tools: Python, Jupyter Notebook, Pandas, Seaborn, Matplotlib, Plotly

## Introduction
Road traffic accidents remain a major global concern, with significant implications for public health, traffic management, and urban planning. According to the World Health Organization (WHO, 2018), road injuries are among the top 10 causes of death globally. The aim of this project is to analyze crash data to better understand patterns of incidents, their contributing factors, and severity levels. Through a structured Exploratory Data Analysis (EDA), this project provides visual insights into critical time-based and environmental crash patterns.

## Dataset Description
The dataset used for this analysis, Crash_new_dataset2.csv, contains structured crash report records. It includes variables such as:

Hour – the hour when the crash occurred (0–23)

Weekday – day of the week

Injury Severity – level of injury sustained

Surface Condition – dry, wet, icy, etc.

Driver Fault – whether the driver was at fault

Additional contextual and environmental factors

The data was pre-cleaned prior to analysis to remove missing or inconsistent values.

## Analysis Highlights
### Driver Fault vs Surface Condition
Most at-fault crashes occur on dry roads, likely due to higher traffic volumes.

Wet or icy roads, although less frequent, show a higher proportional risk of driver fault.

This supports existing research on reduced traction and visibility increasing crash risk (Evans, 2004).

🔍 Visualized using a heatmap showing fault distribution across surface types.

 ### Hour of Day vs Injury Severity
Severe injuries are more common during evening hours (5–9 PM), potentially due to fatigue, impaired driving, or higher speeds.

Minor injuries dominate during daylight hours.

🔍 Visualized through a stacked bar chart (both static and interactive with Plotly).

### Crashes by Hour and Weekday
Crashes cluster around weekday peak traffic hours, especially morning (7–9 AM) and evening (4–7 PM).

Weekends show relatively lower crash densities.

🔍 Visualized as a heatmap with annotated crash counts per weekday-hour cell.

## Tools and Technologies
- Python 3.9+

- Jupyter Notebook

- Libraries:

- pandas, numpy – data manipulation

- matplotlib, seaborn – static plotting

- plotly.express – interactive visualizations

## Key Takeaways
Environmental and temporal factors have a compounding effect on crash severity.

Interactive charts enhance understanding and communication of traffic trends.

This kind of EDA can support policy development, road safety improvements, and public awareness campaigns.

## Repository Structure
bash
Copy
Edit
├── Crash_new_dataset2.csv          # Cleaned dataset
├── Ashutosh_Behera_EDA.ipynb       # Jupyter notebook with all analysis
├── README.md                       # Project documentation
🔧 Getting Started
## Clone the Repository:

bash
Copy
Edit
git clone https://github.com/your-username/road-crash-eda.git
cd road-crash-eda
Install Required Packages:

bash
Copy
Edit
pip install -r requirements.txt
Open the Notebook:

bash
Copy
Edit
jupyter notebook Ashutosh_Behera_EDA.ipynb
## Future Work
Add spatial visualizations using geopandas or folium

Integrate real-time crash feeds (e.g., open traffic APIs)

Deploy findings into a public dashboard (e.g., using Streamlit)

## References
World Health Organization. (2018). Global status report on road safety 2018.
https://www.who.int/publications/i/item/9789241565684

Evans, L. (2004). Traffic Safety. Science Serving Society.

## Contact
Ashutosh Behera
📧 your.email@example.com
🔗 LinkedIn
