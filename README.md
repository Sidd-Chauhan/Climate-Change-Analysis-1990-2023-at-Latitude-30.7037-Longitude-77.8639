# Climate-Change-Analysis-1990-2023-at-Latitude-30.7037-Longitude-77.8639

## Introduction

This repository is created for a detailed climate change analysis from **01/01/1990 to 12/30/2023** at **Latitude: 30.7037, Longitude: 77.8639** based on the use of data sources including **NASA/POWER CERES/MERRA2 Native Resolution Daily Data** for temperature changes, precipitation patterns, changes in wind speed, and changes in the wind direction pattern and their impact on local climate.

This study is intended to identify:
- **Temperature Trends and Anomalies**: Changes in land surface and air temperatures.
- **Precipitation and Drought Analysis**: Trends in annual and seasonal precipitation and droughts.
- **Wind Speed and Direction Trends**: Long-term changes in wind velocity and direction.

The data file will contain all the Python code, visualization, and analysis steps that will allow for a comprehensive look at the climate shifts in the region over the last three decades.

---

## Data Source

The dataset is retrieved from the sources NASA/POWER CERES/MERRA2 Native Resolution Daily Data under these parameters:
Temperature at 2 Meters (T2M)
Earth Skin Temperature (TS)
Specific Humidity at 2 Meters (QV2M)
Precipitation Corrected (PRECTOTCORR)
Wind Speed at 10 Meters (WS10M)
Wind Direction at 10 Meters (WD10M)
 
### Data Summary:
Period: 01/01/1990 - 12/30/2023
Location: Latitude 30.7037, Longitude 77.8639
Elevation: 1403.86 meters from MERRA-2
Missing Data Value: `-999`
 
------

## Analysis & Methodology

The analysis has three fundamental divisions, each focusing on different facets of climate change:

### 1. Temperature Trends and Anomalies

#### Goal
Long-term warming and cooling trends.
Seasonal changes, heat waves or cold snaps, and temperature anomalies throughout the years.

#### Procedures
Annual and Monthly Trends: Analyze annual and monthly averages of both T2M (Temperature at 2 Meters) and TS (Earth Skin Temperature).
**Temperature Anomalies**: Determine changes in temperatures over a yearly time scale.
 **Anomalies Detection**: Identify temperature anomalies based on statistical methods, such as the use of z-scores.

#### Code:
Python code for analyzing temperature trends and producing graphs is available in `temperature_analysis.py`.

#### Key Takeaways
 Determined if the region was warming up and calculated the magnitude of temperature variations.

### 2. Precipitation and Drought Analysis

##### Objective
Assess changes in precipitation and identify shifts in wet and dry seasons.
To identify drought events using **SPI**
Detect extreme precipitation events.

Procedure
Annual and Seasonal Accumulations of Precipitation.
Compute the annual and seasonal accumulations of precipitation.
Identify Drought Events. Compute the SPI to assess the level of drought occurrence.
Extreme Events. Utilize precipitation percentiles, such as the 95th percentile, to identify extreme events of rainfall.
Precipitation and drought analysis codes are in `precipitation_analysis.py`.

Primary Findings:
- Trends in precipitation regimes: for example, dramatic change in wet/dry seasons and increased or decreased drought conditions

### 3. Changes in Wind Speed and Direction

Objective:
- Research wind speed over time and find whether extreme wind events have been increasing.
- Research changes in predominate wind directions.

Procedures:
- **Wind Speed Trends**: Calculate annual and monthly averages of wind speed.
- **Wind Direction Patterns**: Show the patterns of wind direction as a wind rose.
- **Extreme Wind Events**: Determine extreme winds using the 95th percentile as a cutoff value.

#### Code:
- Python code for analyzing wind speed and direction can be found in `wind_analysis.py`.

#### Key Results:
- Long-term trends of changes in wind patterns, including growth in extreme wind events or shifts in dominant directions.
---
## Conclusion

The resulting plots show strong trends for climate condition over time:
1. Temperature: Shows a clear warming trend, with more frequent occurrences of extreme heat.
2. Precipitation: Has increased occurrences of drought-like conditions, while extreme rainfall events have recently slightly increased in frequency.
3. **Wind**: The wind speed has been constant in the past, though there is a certain variability in the wind direction regime.

This study helps reveal how the regional climate is changing with time and, therefore its consequences on local ecosystems, agriculture, and weather patterns.
