📌 Overview
This project presents a comprehensive spatiotemporal and predictive analysis of four hazardous air pollutants — Benzene, Formaldehyde, Nitrogen Dioxide (NO₂), and Ozone (O₃) — in Texas, USA.
It integrates ground-level monitoring data from the U.S. Environmental Protection Agency (EPA) with satellite observations from NASA’s Aura/OMI mission to identify long-term trends, hotspot regions, pollutant correlations, and future forecasts.
The work applies data science techniques — from large-scale data preprocessing to machine learning forecasting models — to generate actionable insights for environmental monitoring, public health policy, and sustainability planning.


🎯 Objectives
Analyze long-term pollutant trends from 1990–2025 (Benzene & Formaldehyde) and 2004–2025 (NO₂ & O₃).
Visualize pollutant concentrations spatially (heatmaps) and temporally (time-series).
Forecast future pollutant levels using Linear Regression and Random Forest models.
Assess correlations among pollutants to identify shared sources or atmospheric interactions.
Provide policy-relevant recommendations for Texas’s high-risk industrial and urban zones.


📂 Project Structure
├── notebooks/
│   ├── Benzene_Formaldehyde_Analysis.ipynb
│   ├── NO2_Analysis.ipynb
│   ├── O3_Analysis.ipynb
├── data/  # (Not included due to large size)
├── figures/
│   ├── hotspot_maps/
│   ├── time_series_plots/
│   ├── correlation_matrices/
├── Capstone_Project_Final_Report.pdf
├── Final_Presentation.pdf
└── README.md


🗂 Data Sources
EPA AMTIC Hazardous Air Pollutants Archive
https://www.epa.gov/amtic/amtic-ambient-monitoring-archive-haps
(Benzene, Formaldehyde — Ground monitoring stations)
EPA Air Quality System (AQS)
https://www.epa.gov/aqs
NASA GES DISC Aura/OMI Satellite Data
https://acdisc.gesdisc.eosdis.nasa.gov
(NO₂, O₃ — Level-3 and Level-2G products)
🛠 Tools & Technologies
Python: pandas, numpy, matplotlib, seaborn, scikit-learn
GIS: ArcGIS, QGIS for geospatial mapping
Panoply: For .he5 file visualization
Jupyter Notebooks: Workflow development & documentation


🔍 Methodology
Data Acquisition & Conversion
.accdb → .csv (EPA)
.he5 → .NetCDF (NASA)
Filtering & Cleaning
Subset data for Texas
Remove anomalies & missing values
Exploratory Data Analysis (EDA)
Time-series trend analysis
Hotspot detection via geospatial mapping
Modeling & Forecasting
Linear Regression (LR)
Random Forest (RF) for nonlinear trends
Correlation Analysis
Pearson correlation between pollutants
Visualization & Insights
Heatmaps, scatterplots, forecast curves


📊 Key Findings
Benzene & Formaldehyde: Overall decline over decades, but persistent industrial hotspots remain.
NO₂: Post-2020 rebound in levels, likely linked to increased industrial and transportation activity.
O₃: Seasonal peaks in summer due to photochemical reactions.
Correlations: Strong positive relationship between Benzene–Formaldehyde & Benzene–NO₂; moderate Benzene–O₃ link.

📈 Forecast Results
Random Forest models captured nonlinear environmental trends better than Linear Regression.
Predictive outputs can serve as early warning tools for policymakers.

🚧 Challenges & Solutions
Large datasets (~600GB) → Batched processing & cloud storage.
File format incompatibility → Conversion with Panoply & Python libraries.
Data sparsity in rural Texas → Focused on metropolitan & industrial zones.

📌 Future Work
Expand to PM2.5, SO₂, and VOCs.
Integrate health impact data for exposure-risk mapping.
Apply deep learning (LSTM, CNN) for improved forecasting.
Deploy interactive dashboards for public & regulatory access.

📜 Citation
If you use this work, please cite:
@misc{adhikari2025hazardouspollutants,
  author       = {Nawaraj Adhikari},
  title        = {Spatiotemporal and Predictive Analysis of Hazardous Air Pollutants in Texas Using EPA and NASA Data},
  year         = {2025},
  institution  = {University of Texas at Arlington},
  note         = {Capstone Project under guidance of Dr. Yunyao Li}
}
📧 Contact
Author: Nawaraj Adhikari
📩 Email: nxa6298@mavs.uta.edu / nwa.adhikari@gmail.com


