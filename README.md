<h1 style="text-align: center;">
NYC Summer 2025 Taxi Data Analysis
</h1>

<p style="text-align: center; font-style: italic;">
An analysis of the 2025 nyc taxi data, for the NYU Accelerated Certificate in Data Analytics Capstone Project.
</p>

<!-- shields -->
[![GitHub Watchers](https://img.shields.io/github/watchers/drod75/nyc_taxi_analysis?style=flat-square)](https://github.com/drod75/nyc_taxi_analysis/watchers)
[![GitHub Stars](https://img.shields.io/github/stars/drod75/nyc_taxi_analysis?style=flat-square)](https://github.com/drod75/nyc_taxi_analysis/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/drod75/nyc_taxi_analysis?style=flat-square)](https://github.com/drod75/nyc_taxi_analysis/forks)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-David%20Rodriguez-blue?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/david-rodriguez-nyc/)

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Project Overview](#project-overview)
- [Repository Structure](#repository-structure)
- [Data Sources](#data-sources)
- [References](#references)

## Project Overview

Every summer tens of thousands travel across the city via taxi, whether that be for vacation, work, or anything else. Based on this, what are the frequent taxi travel patterns within the summer of 2025, such as common destinations, peak travel times, and common trends among riders?

The project aims to look at rider trends and inform target audiences about taxi trends so they understand where different people in the city are headed. The target audience consists of the NYC Taxi and Limousine commissioner, Midori Valdivia, and the taxi drivers who make rides possible. The goal of addressing the taxi commissioner is to help identify frequent taxi patterns, and the goal of informing taxi drivers is to alert them of possible destinations they may be headed to to help them plan ahead of time. This project serves as the basis for serving riders more efficiently by understanding trends that drivers and the commission learn from to apply new and more efficient practices when needed, thus improving reliability and trips.

## Repository Structure

- `assets/`: Contains the dashboards and data used in the project.
- `assets/dashboards/`: Contains the Tableau dashboard used for data visualization.
- `assets/data/`: Contains some of the datasets used for analysis.
- `notebooks/`: Contains the Jupyter notebooks used for data analysis and visualization.

## Data Sources

Two main datasets were used within this analysis, one being the “2025 Yellow Taxi Trip Data” (2025 Yellow Taxi Trip Data, 2026, #), which contains the Yellow Taxi records from the year 2025, and the other being the “NYC Taxi Zones” (NYC Taxi Zones, 2025, #), which contains data responding to each pickup and dropoff zone within the taxi trip data. The source of each dataset is the Taxi and Limousine Commission (TLC), which was provided via the NYC Open Data platform. 

When working with the 2025 Yellow Taxi Trip Data (2026, #), the period chosen within the data to analyze was the period of summer from 2025, which was taken as June 21st to September 21st. Important limitations are that the dataset contains columns that are not clear on their purpose; this needs the use of the Data Dictionary provided via (NYC Taxi Zones, 2025, #).  Key variables within this dataset include variables such as but not limited to tpep_pickup_datetime, tpep_dropoff_datetime, PULocationID, DOLocationID, and more. These variables in particular include information about where and when a trip started and ended; this is the backbone of our analysis, as without these variables there would not be a way to determine frequent patterns. 

Our next dataset, which can be seen via (NYC Taxi Zones, 2025, #), contains the data regarding each zone that the trip data (2025 Yellow Taxi Trip Data, 2026, #) refers to via the location ID columns. This dataset is relatively smaller, at 6 columns, each of which is important, with about half being geography columns and the rest being information for each taxi zone, such as borough.

A final dataset, one created solely within the project, was the ‘trip_data.csv’ set; this set contains all the unique trips within the summer 2025 period. The dataset was made with the purpose of recording the unique trips and if they traveled out of the borough of origin. Limitations were that this dataset was created with particularly summer 2025 data, so outside that period there may be the possibility of trips not being present.


## References

- NYC Taxi & Limousine Commission. (n.d.). nyc.gov. https://www.nyc.gov/site/tlc/about/about-tlc.page
- NYC Taxi Zones [TLC trip records contain a field corresponding to the location of the pickup or drop-off of the trip called a taxi zone. Taxi Zones are roughly based on NYC Department of City Planning’s Neighborhood Tabulation Areas (NTAs) and are meant to approximate nei]. (2025, June 9). NYC Open Data. https://data.cityofnewyork.us/Transportation/NYC-Taxi-Zones/8meu-9t5y/about_data
- Rodriguez, D. (2026). capstone_workbook [The dashboard linked to the Capstone Project]. In Summer 2025 Taxi Data. Tableau Public. https://public.tableau.com/app/profile/david.rodriguez1513/viz/capstone_workbook_17949641206260/NYC
- Rodriguez, D. (2026, November). nyc_taxi_analysis [An analysis of the 2025 nyc taxi data, for the NYU Accelerated Certificate in Data Analytics Capstone Project.]. Github. https://github.com/drod75/nyc_taxi_analysis
- 2025 Yellow Taxi Trip Data [These records are generated from the trip record submissions made by yellow taxi Technology Service Providers (TSPs). Each row represents a single trip in a yellow taxi. The trip records include fields capturing pick-up and drop-off dates/times, pick-up an]. (2026, September 29). NYC Open Data. https://data.cityofnewyork.us/Transportation/2025-Yellow-Taxi-Trip-Data/irx2-vgm4/about_data
