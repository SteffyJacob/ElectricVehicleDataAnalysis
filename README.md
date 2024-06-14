# ElectricVehicleDataAnalysis
Working with Electric Vehicle data and associated data sets to create some impactful data analysis (Power BI, Python, Excel)

## Introduction
Electric vehicles (EVs) are becoming increasingly popular as the world shifts towards more sustainable forms of transportation. This project aims to analyze various aspects of EV adoption, infrastructure, and market trends using publicly available data. By leveraging data analysis techniques, we can uncover insights into the factors driving EV adoption and the impact of EVs on the environment and infrastructure.

## Problem Statement
The main objectives of this project are to :

- Identify and measure some of the relevant KPIs.
- Analyze trends in EV adoption over time and across different regions.

## Tools & Technologies

This project utilizes various tools and technologies to perform data collection, analysis, and visualization. The choice of tool depends on the specific requirements of each analysis task. 
- **Python:** 
  - Data Analysis and Validation:
  Python scripts and libraries like pandas are used for data collection, preprocessing, and cleaning.
- **Power BI:**
  - Interactive Dashboards:
  Power BI is used to create interactive dashboards for visualizing trends, geographic distributions, and other key metrics.
  - Data Integration:
  Power BI integrates data from various sources to provide comprehensive and interactive reports.
- **Excel:**
  - Data Inspection and Manual Analysis:
 Excel is used for initial data inspection, manual data analysis, and simple visualizations.

## Data Sources
The datasets used in this project are sourced from various public and open data platforms, including:
- Data.gov\
- AFDC Fuel Station Locator - https://afdc.energy.gov/data_download

## Project Steps
The project is organized into the following sections:
### 1. Data Collection & Data Cleaning
1. Electric_Vehicle_Population_Data. csv manually downloaded from Data.gov site. Search for EV Population data in the site (File is not attached)
2. Before starting, to check the data quality we used python scripts in Jupyter Notebook. (File is attached)
3. Cleaning of data is done based on the results and the irrelevant columns are kept as it is.
4. Modified file is opened in Excel for quick data inspection and manual analysis.

### 2. Data Analysis & Report generation

Given the dataset with columns related to electric vehicle (EV) population, here are some metrics & possible correlations that I tried to explore as part of data analysis:
- **1. KPIs**
  - Used Card visuals to show the below relevant Key Performance metrices.
    ![image](https://github.com/SteffyJacob/ElectricVehicleDataAnalysis/assets/69688793/216340d4-9461-4274-aaeb-716cef36e891)

- **2. EV Adoption over the years**
  - To display the growth of EV adoption over the years, line chart visualization is used.
    ![image](https://github.com/SteffyJacob/ElectricVehicleDataAnalysis/assets/69688793/61090d4d-98ad-48e5-83f0-5af8e5da8815)
    
- **3. Adoption rates of BEVs versus PHEVs over the years**
  - To highlight how the adoption of different types of electric vehicles (e.g., BEV - Battery Electric Vehicles, PHEV - Plug-in Hybrid Electric Vehicles) has changed over      time, we have used line chart visual
    ![image](https://github.com/SteffyJacob/ElectricVehicleDataAnalysis/assets/69688793/fc4e0c07-6a4f-4522-82bb-cc19eaf6e8d2)

- **4. EVs by Maker & Model**
  - To compare counts of EVs across different makers over the years, we have used a stacked column chart. From this visual, it is evident that TESLA has been the leading        with even a drill down to specifically show the number of vehicles per model each year.
    ![image](https://github.com/SteffyJacob/ElectricVehicleDataAnalysis/assets/69688793/2afe1ecd-27b5-457b-bfeb-e87a7884b649)

- **5. Price & Range relationships of different EVs**
  - To explore the relationship between the price and range of different EVs, I used scatter plot where Electric Range reported on the x-axis, Base MSRP on the y-axis, with 
    points colored by Make. This visual shows that Tesla offers the highest range even though it’s base MSRP is still same to many other manufactures, in a way proving why 
    Tesla is the most popular EV in the market.
    ![image](https://github.com/SteffyJacob/ElectricVehicleDataAnalysis/assets/69688793/fdaa18bd-5c34-4991-926b-21ddb8f43473)

- **6. Distribution of Electric Vehicles & Charging Stations**
  - From the EV Population data file, by parsing the Vehicle Location field into Latitude and Longitude, I used map visual to show spatial distribution of EV vehicles.          Similarly, I used a data file downloaded from public site to get AFDC Fuel Station Locator data, which is then filtered just for US to show some insights on the  
    distribution of EV charging station across different states in US.
    ![image](https://github.com/SteffyJacob/ElectricVehicleDataAnalysis/assets/69688793/2f0708d9-7f60-43f5-81e4-9ad617671494)
