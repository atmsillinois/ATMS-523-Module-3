# Module 3 Project: Daily Climatology and Weather Plot

**Student Name:** Nathan Makowski  
**Course:** ATMS 523 / Weather and Climate Data Analytics 
**Date:** 2025-10-08  

---

## Project Overview

This project demonstrates how to:

1. **Download daily GHCN station data** from Amazon Web Services (AWS) for a selected station.
2. **Compute daily climatology** for the 1991–2020 period, including:
   - Record high and low temperatures
   - Average high and low temperatures for each calendar day
3. **Extract actual daily temperatures** for a specific year (2024 in this case).
4. **Visualize the data** using `matplotlib` with a plot that shows:
   - Actual daily high and low temperatures
   - Climatological average high and low temperatures
   - Record high and low temperatures
5. Excludes leap day (February 29) from all calculations.

---

## Files

- `M3N2_final_hw_njm.ipynb` — The Jupyter Notebook containing all code, checks, and plots.
- `README.md` — This file explaining the project and its contents.

---

## How to Run

1. Ensure Python 3.10+ and the required packages are installed:
   ```bash
   pip install pandas numpy matplotlib pyarrow
