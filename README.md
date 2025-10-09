# ATMS 523 Module 3

## Overview
This project analyzes historical weather data from the Global Historical Climatology Network (GHCN) to calculate temperature statistics and create visualizations comparing record temperatures, 30-year averages, and actual daily temperatures for Bloomington, IN, 1999.

## Assignment Details
- **Course**: ATMS 523 (Atmospheric Sciences)
- **University**: University of Illinois at Urbana-Champaign (UIUC)
- **Student**: Zachary Torstrick
- **Semester**: Fall 2025
- **Assignment**: Module 3 Project

## Project Components

### Part 1: Temperature Statistics Function
Developed a function `get_ghcn_station_stats()` that:
- Downloads GHCN Daily weather data from Amazon Web Services
- Calculates record high and low temperatures for each calendar day
- Computes 30-year average high and low temperatures (1991-2020 period)
- Returns a pandas DataFrame with temperature statistics by day of year

### Part 2: Interactive Weather Visualization
Created a Bokeh plot that displays:
- **Record Range**: Historical extremes (light blue shaded area)
- **Average Range**: 30-year climate normals (medium blue shaded area)
- **Actual Temperatures**: Daily observations for a specific year (dark blue bars)

## Data Source

### Global Historical Climatology Network (GHCN) Daily
- **Source**: National Centers for Environmental Information (NCEI), NOAA
- **Dataset**: GHCN Daily Data
- **Access Method**: Amazon Web Services S3 bucket
- **URL**: `s3://noaa-ghcn-pds/csv/by_station/`
- **Citation**: 
  > Menne, M.J., I. Durre, R.S. Vose, B.E. Gleason, and T.G. Houston, 2012: An overview of the Global Historical Climatology Network-Daily Database. Journal of Atmospheric and Oceanic Technology, 29, 897-910, doi:10.1175/JTECH-D-11-00103.1

### Data Format
- **Temperature Units**: Tenths of degrees Celsius (converted to degrees Celsius in analysis)
- **Time Period**: Historical data from 1900s to 2020
- **Elements**: TMAX (maximum temperature), TMIN (minimum temperature)
- **Quality Flags**: M_FLAG, Q_FLAG, S_FLAG for data quality assessment

### Station Information
- **Primary Station**: USC00120784 (Bloomington, Indiana University)
- **Location**: Bloomington, Indiana, USA
- **Station Type**: University weather station
- **Data Availability**: Varies by element and time period

## License
This project is for educational purposes as part of ATMS 523 coursework at UIUC.

---
*Last updated: October 2025*