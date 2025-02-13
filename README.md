# Water Quality Analysis Dataset

## Description
This repository contains a dataset focused on water quality parameters across various monitoring stations in India. The dataset includes environmental metrics such as temperature, dissolved oxygen, pH levels, conductivity, biochemical oxygen demand (B.O.D.), nitrate/nitrite concentrations, and coliform bacterial counts. The data spans multiple years and locations, making it suitable for temporal and spatial analysis of water quality trends.

## Dataset Overview
The dataset is structured as a tabular file (e.g., CSV or Excel) with the following columns:

| Column Name                          | Description                                                                 |
|--------------------------------------|-----------------------------------------------------------------------------|
| `STATION CODE`                       | Unique identifier for the monitoring station.                               |
| `LOCATIONS`                          | Geographic area or name of the monitoring site.                             |
| `STATE`                              | Indian state where the station is located.                                  |
| `Temp`                               | Temperature of the water (°C).                                              |
| `D.O. (mg/l)`                        | Dissolved oxygen concentration in milligrams per liter.                     |
| `PH`                                 | pH level of the water (acidity/alkalinity).                                 |
| `CONDUCTIVITY (µmhos/cm)`            | Electrical conductivity of the water (corrected to `CONDUCTIVITY`).         |
| `B.O.D. (mg/l)`                      | Biochemical Oxygen Demand, measuring organic pollution.                     |
| `NITRATENAN N+ NITRITENANN (mg/l)`   | Combined nitrate and nitrite nitrogen concentrations.                       |
| `FECAL COLIFORM (MPN/100ml)`         | Fecal coliform bacteria count (Most Probable Number per 100ml).             |
| `TOTAL COLIFORM (MPN/100ml)`         | Total coliform bacteria count (MPN/100ml).                                  |
| `Mean`                               | Mean value of measurements (context-dependent, e.g., annual average).       |
| `year`                               | Year of data collection.                                                    |

## Potential Use Cases
- **Environmental Monitoring**: Track water quality trends over time.
- **Public Health Research**: Correlate coliform levels with health outcomes.
- **Pollution Studies**: Analyze B.O.D. and nitrate/nitrite concentrations.
- **Geospatial Analysis**: Map water quality parameters by state/location.

## Usage
### Loading the Data
```python
import pandas as pd

df = pd.read_csv("water_quality_data.csv")
print(df.head())
