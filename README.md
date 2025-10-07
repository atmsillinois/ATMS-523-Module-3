# Weather Station Analysis

A Python tool for analyzing historical weather data from GHCN stations, creating temperature statistics and interactive visualizations.

## Overview

This script downloads weather data from AWS and calculates:
- All-time temperature records for each calendar day
- 1991-2020 normal period averages
- Interactive plots comparing records, averages, and actual data

## Data Source

**NOAA Global Historical Climatology Network Daily (GHCN-D)**
- DOI: [10.7289/V5D21VHZ](https://doi.org/10.7289/V5D21VHZ)
- Hosted on AWS S3: `s3://noaa-ghcn-pds/csv/by_station/`
- Global coverage of daily weather observations

## Requirements

```bash
pip install pandas matplotlib numpy bokeh
```

## Usage

1. Open `HW3_weather_analysis.ipynb` in Jupyter
2. Run all cells to analyze:
   - Champaign, IL (USC00118740)
   - Berlin, Germany (GM00010393)

### Custom Stations

```python
# Find and analyze any GHCN station
stats = analyze_weather_station('STATION_ID')
```

## Output

- **Matplotlib plots**: Static temperature analysis with record ranges and actual data
- **Bokeh plots**: Interactive visualizations with zoom, pan, and hover tooltips
- **Temperature statistics**: Daily records and 1991-2020 averages for each calendar day

## Author

**Stephen Allen**

ATMS 523 - University of Illinois