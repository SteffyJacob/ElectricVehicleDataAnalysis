# ElectricVehicleDataAnalysis
Working with Electric Vehicle data and associated data sets to create some impactful data analysis (Power BI, Python, Excel)

## Introduction
Electric vehicles (EVs) are becoming increasingly popular as the world shifts towards more sustainable forms of transportation. This project aims to analyze various aspects of EV adoption, infrastructure, and market trends using publicly available data. By leveraging data analysis techniques, we can uncover insights into the factors driving EV adoption and the impact of EVs on the environment and infrastructure.

## Problem Statement
The main objectives of this project are to:

- Analyze trends in EV adoption over time and across different regions.
- Investigate the distribution and utilization of EV charging infrastructure.
- Assess the impact of EVs on local power grids.
- Segment the EV market based on consumer demographics and purchasing behavior.
- Evaluate the environmental benefits of EV adoption.
- Analyze the resale market trends for electric vehicles.
- Develop predictive models for EV maintenance requirements.

## Tools & Technologies

This project utilizes various tools and technologies to perform data collection, analysis, and visualization. The choice of tool depends on the specific requirements of each analysis task. 
- **Python:** 
  - Data Collection and Cleaning:
  Python scripts and libraries like pandas and numpy are used for data collection, preprocessing, and cleaning.
  - Exploratory Data Analysis (EDA):
  Python notebooks with matplotlib, seaborn, and plotly are used for initial data exploration and visualization.
  - Predictive Modeling:
  Machine learning models are developed using Python libraries such as scikit-learn.
- **Power BI:**
  - Interactive Dashboards:
  Power BI is used to create interactive dashboards for visualizing trends, geographic distributions, and other key metrics.
  - Data Integration:
  Power BI integrates data from various sources to provide comprehensive and interactive reports.
- **Excel:**
  - Data Inspection and Manual Analysis:
Excel is used for initial data inspection, manual data analysis, and simple visualizations.
  - Pivot Tables and Charts:
Excel's pivot tables and charts are used to summarize and visualize data quickly.

## Data Sources
The datasets used in this project are sourced from various public and open data platforms, including:
- Data.gov

## Project Structure
The project is organized into the following sections:
### 1. Data Collection & Data Cleaning
1. Electric_Vehicle_Population_Data. csv manually downloaded from Data.gov site. (File is attached)
2. Before starting, to check the data quality we used python scripts in Jupyter Notebook. (File is attached)
3. Cleaning of data is done based on the results and the irrelevant columns are kept as it is.
4. Modified file is opened in Excel for quick data inspection and manual analysis.

### 2. Data Analysis & Report generation
Given the dataset with columns related to electric vehicle (EV) population, here are some possible correlations you can explore as part of data analysis: 
- **1. Producer Correlations**
  - Used `Stacked Bar Charts` to show EV breakdown by Producer.
- **2. Geographical Correlations**
  - County/City/State vs. Electric Vehicle Type
    Analyze how the distribution of different types of EVs (e.g., Battery Electric Vehicles, Plug-in Hybrid Electric Vehicles) varies across different geographic regions.
  - County/City/State vs. Electric Range
    Investigate if there's a regional preference for EVs with specific electric ranges.
  - County/City/State vs. Clean Alternative Fuel Vehicle (CAFV) Eligibility
    Explore how eligibility for clean alternative fuel vehicle incentives varies by region.
  - County/City/State vs. Make/Model
    Study the popularity of different EV makes and models in various regions.
------------------------------------------------
The Sales Dashboard is designed to provide an in-depth analysis of sales data, focusing on various factors that influence sales performance. Key features include:

- **KPIs:** 
  - Total Sales
  - Total Quantity of Products
  - Total Profit
  - Average Delivery Time

- **Visualizations:**
  - **Stacked Area Charts:** Compare sales and profit across different years.
  - **Category Analysis:** Breakdown of sales by category and sub-category.
  - **Geographical Analysis:** Sales performance across different regions.
  - **Shipping Analysis:** Impact of different ship modes on sales.
  - **Segment Analysis:** Sales distribution across various customer segments.

### Sales Forecasting

The Sales Forecasting page utilizes time series analysis techniques to forecast future sales trends. This includes:

- **Time Series Decomposition:** Breaking down the sales data into trend, seasonal, and residual components.
- **Forecast Models:** Applying predictive models to provide accurate sales forecasts.

## Getting Started

### Prerequisites

- **Power BI Desktop:** Ensure you have the latest version of Power BI Desktop installed on your machine.
- **Superstore Sales Data:** Ensure you have the `superstore_sales.csv` file containing the sales data from 2020 to 2023.
  
### Steps to Create the Sales Dashboard
1. **Load the Data:**
   - Open Power BI Desktop.
   - Click on `Get Data` and select `Text/CSV`.
   - Navigate to the location of the `Superstore 2023.csv` file and load it into Power BI.

2. **Data Cleaning and Transformation:**
   - Go to the `Transform Data` option to open the Power Query Editor.
   - Check for any missing or inconsistent data and clean it as needed. Especially the date fields had a mix of mm/dd/yyyy and dd/mm/yyyy format entries. So I did the data transformation using M- Query to fix the data error.
   - Ensure data types are correctly set (e.g., dates as Date type, sales as Currency type).

3. **Create Relationships (if necessary):**
   - Here there was only one dataset. So, no relationships were created.

4. **Design the Sales Dashboard:**
   - **KPIs:** 
     - Use `Card` visualizations to display Total Sales, Total Quantity of Products, Total Profit, and Average Delivery Time.
   - **Stacked Area Charts:**
     - Created `Stacked Area Charts` to compare Sales and Profit year-over-year.
   - **Category Analysis:**
     - Used `Clustered Bar Charts` to show sales breakdown by Category and Sub-Category.
   - **Geographical Analysis:**
     - Used `Map` visualizations to display sales performance across different regions.
   - **Shipping Analysis:**
     - Created `Bar Charts` to analyze the impact of different Ship Modes on sales.
   - **Segment Analysis:**
     - Used `Donut Charts` to display sales distribution across various Customer Segments.

5. **Create the Sales Forecasting Page:**
   - Used `Line Charts` to visualize and analyze sales trends.
   - Applied `Forecasting` features available in Power BI to predict future sales.

6. **Finalize and Publish:**
   - Reviewed and finalized the dashboard layout and visualizations.
   - Saved the Power BI report file as `Retail Store Sales Dashboard.pbix`and uploaded to the repository.

### Snapshots of the report screens with visuals mentioned earlier
1. **Sales Dashboard**
   ![Screenshot 2024-06-06 190823](https://github.com/SteffyJacob/PowerBIDashboard-1/assets/69688793/f1385461-0cff-43ae-a1d8-b45db22c8931)
   
3. **Sales Dashboard-Region Slicer applied**
   ![Screenshot 2024-06-06 191522](https://github.com/SteffyJacob/PowerBIDashboard-1/assets/69688793/96bfdf61-2d72-4280-8487-1b4dc2d53f92)
   
5. **Sales Forecasting**
   ![Screenshot 2024-06-06 190922](https://github.com/SteffyJacob/PowerBIDashboard-1/assets/69688793/ebc8ba41-39d2-4df4-b222-4e389f931087)
