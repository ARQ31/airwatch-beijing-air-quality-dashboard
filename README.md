# AirWatch: Beijing Air Quality Analytics Dashboard

AirWatch is an interactive data analytics dashboard built with Streamlit to explore air pollution patterns in Beijing from March 2013 to February 2017. This project analyzes air quality data from 12 monitoring stations and focuses on PM2.5 pollution, seasonal trends, station-level differences, and the relationship between pollutant concentration and meteorological factors.

## Live Demo

[Open Streamlit App](https://le4rn132.streamlit.app/)

## Project Overview

Air pollution is one of the most important environmental issues in urban areas. Beijing has experienced severe air quality problems, especially during winter periods. This project aims to transform raw air quality data into an interactive dashboard that helps users understand pollution trends, identify high-risk periods, compare monitoring stations, and generate data-driven recommendations.

The dashboard is designed to answer two main analytical questions:

1. How does PM2.5 concentration vary across seasons and monitoring stations?
2. How do meteorological factors such as wind speed, temperature, and humidity relate to PM2.5 concentration?

## Key Features

* Interactive Streamlit dashboard
* Station and season filters
* KPI cards for PM2.5, PM10, CO, active stations, and percentage of hours above the PM2.5 threshold
* Seasonal PM2.5 comparison
* Station-level PM2.5 ranking
* Correlation heatmap between pollutants and weather variables
* PM2.5 analysis based on wind speed groups
* Air quality clustering by monitoring station
* Final insights and policy recommendations

## Tech Stack

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Streamlit

## Dataset

This project uses the Beijing Multi-Site Air Quality Dataset, which contains hourly air quality measurements from 12 monitoring stations in Beijing between March 2013 and February 2017.

The dataset includes several pollutant and meteorological variables, such as:

* PM2.5
* PM10
* SO2
* NO2
* CO
* O3
* Temperature
* Pressure
* Dew point
* Rainfall
* Wind speed
* Station name
* Season

## Dashboard Sections

### 1. Overview Metrics

The dashboard shows key indicators such as average PM2.5, average PM10, average CO, number of active stations, and the percentage of measurement hours where PM2.5 exceeds the selected threshold.

### 2. Seasonal and Spatial PM2.5 Trend

This section compares PM2.5 concentration across seasons and monitoring stations. The analysis shows that winter tends to have the highest PM2.5 level, while summer tends to have better air quality.

### 3. Meteorological Factor Analysis

This section explores the relationship between pollutants and weather conditions using a correlation heatmap. It also highlights how wind speed is related to PM2.5 concentration.

### 4. Station-Level Air Quality Clustering

Each monitoring station is grouped into air quality categories based on average PM2.5 concentration. This helps identify which stations are more exposed to unhealthy air quality conditions.

### 5. Insights and Recommendations

The dashboard provides final conclusions and recommendations related to seasonal policy, early warning systems, and priority intervention areas.

## Key Insights

* Winter has the highest average PM2.5 concentration compared to other seasons.
* Summer has relatively better air quality due to weather conditions such as rain and stronger wind.
* Several urban monitoring stations show higher PM2.5 levels than suburban stations.
* CO has a strong positive relationship with PM2.5, indicating that combustion-related emissions may be an important pollution source.
* Higher wind speed is associated with lower PM2.5 concentration because wind helps disperse air pollutants.

## How to Run This Project Locally

### 1. Clone this repository

```bash
git clone https://github.com/ARQ31/airwatch-beijing-air-quality-dashboard.git
cd airwatch-beijing-air-quality-dashboard
```

### 2. Install the required libraries

```bash
pip install -r requirements.txt
```

### 3. Run the Streamlit dashboard

```bash
streamlit run dashboard.py
```

## Project Structure

```text
airwatch-beijing-air-quality-dashboard/
│
├── data/
│   ├── PRSA_Data_Aotizhongxin_20130301-20170228.csv
│   ├── PRSA_Data_Changping_20130301-20170228.csv
│   ├── PRSA_Data_Dingling_20130301-20170228.csv
│   ├── PRSA_Data_Dongsi_20130301-20170228.csv
│   ├── PRSA_Data_Guanyuan_20130301-20170228.csv
│   ├── PRSA_Data_Gucheng_20130301-20170228.csv
│   ├── PRSA_Data_Huairou_20130301-20170228.csv
│   ├── PRSA_Data_Nongzhanguan_20130301-20170228.csv
│   ├── PRSA_Data_Shunyi_20130301-20170228.csv
│   ├── PRSA_Data_Tiantan_20130301-20170228.csv
│   ├── PRSA_Data_Wanliu_20130301-20170228.csv
│   └── PRSA_Data_Wanshouxigong_20130301-20170228.csv
│
├── dashboard.py
├── main_data.csv
├── requirements.txt
└── README.md
```

## Future Improvements

Several improvements can be added in the future:

* Add machine learning model to predict PM2.5 concentration
* Add anomaly detection for extreme pollution events
* Add interactive time-series visualization using Plotly
* Add downloadable filtered data
* Add station map visualization
* Improve dashboard responsiveness for mobile devices

## Author

**Ariq Marwan Permana**

This project was created as a data analytics portfolio project to demonstrate skills in data cleaning, exploratory data analysis, data visualization, and dashboard development using Python and Streamlit.
