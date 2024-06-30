# Citi Bike Demand Forecast and Allocation Project

## Overview
This project is part of the MGT 585 Fundamentals of Business Analytics course. The goal is to determine the optimal initial allocation of bikes to Citi Bike stations in New York City to maximize the number of daily bike trips. The project involves descriptive, predictive, and prescriptive analytics on a sample dataset from Citi Bike.

## Data Description
The dataset contains information about bike trips taken from June 1, 2017, to May 31, 2018. It includes demographic, economic, and weather information from various sources:
- **Citi Bike System Data**: Information about demand (number of trips) between different stations.
- **American Community Survey**: Demographic and economic data matched by zip code to each Citi Bike station address.
- **NOAA National Centers for Environmental Information**: Historical weather data collected at the Central Park, NYC weather station and matched by date and time to Citi Bike trips.

### Key Fields
- **Trip Information**: `DemandDate`, `DemandTime`, `DayOfWeek`, `Month`, `Demand`
- **Station Information**: `StartStationId`, `StartStationName`, `StartStationLatitude`, `StartStationLongitude`, `StartNeighborhood`, `EndStationId`, `EndStationName`, `EndStationLatitude`, `EndStationLongitude`, `EndNeighborhood`
- **Trip Metrics**: `TripDurationMinutes`, `DistanceMiles`, `MilesPerHour`
- **Commute Information**: `StartCommuteTime`, `EndCommuteTime`
- **Weather Information**: `Temperature`, `DailySnow`, `DailyPrecipitation`
- **Economic and Demographic Information**: `StartPerCapitaIncome`, `EndPerCapitaIncome`, `StartPctHouseholdsNoVehicle`, `EndPctHouseholdsNoVehicle`

## Case Study Instructions

### Objective
To find the number of bikes to stock in each station at the beginning of the day to maximize the number of daily bike trips.

### Steps
1. **Plan**
   - Identify the number of trips between stations (demand) every day.
   - Determine the number of bikes to allocate to each station.

2. **Collect and Prepare**
   - Download and examine the dataset.
   - Compute summary statistics and visualize the data.
   - Check for missing data and outliers.

3. **Analysis**
   - **Descriptive Analytics**: Identify demand patterns.
   - **Predictive Analytics**: Forecast demand between stations using linear regression.
   - **Prescriptive Analytics**: Determine the optimal number of bikes to stock in each station.

4. **Report**
   - Prepare a presentation summarizing the findings and recommendations.

## R Scripts and Analysis

### 1. Data Preparation
- Load and clean the dataset.
- Compute summary statistics.
- Handle missing data and outliers.

### 2. Descriptive Analysis
- Compute univariate statistics (e.g., mean, standard deviation).
- Compute bivariate statistics (e.g., correlation).
- Visualize the data using `ggplot2`.

### 3. Predictive Analysis
- Develop a linear regression model to forecast daytime and evening demand for selected stations.
- Collect data for future dates and predict demand.

### 4. Prescriptive Analysis
- Use optimization techniques to determine the initial allocation of bikes to maximize trips.

