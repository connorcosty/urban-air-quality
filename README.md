# Air Quality Analysis: Marylebone vs Rochester

University Coursework analysis of long-term particulate matter (PM10 and PM2.5) pollution across two contrasting UK monitoring sites, using Python.

**Stack:** Python, pandas, NumPy, matplotlib, scipy

## Overview

This project examines what drives fine particulate pollution and why two very different monitoring sites behave differently. It compares a busy central-London roadside location against a quieter site outside the city, working through the full data-science lifecycle: cleaning raw sensor data, exploratory analysis, statistical testing, and a written report aimed at a non-specialist reader.

The central challenge was separating genuine pollution events from sensor faults during cleaning, since over-aggressive outlier removal risks deleting the real spikes the analysis exists to study.

Graded a 78% by examiner.

## Data

- **Source:** DEFRA monitoring network (UK AURN) 
- **Pollutants:** PM10 and PM2.5
- **Frequency:** Hourly readings
- **Period:** 2018-2022 
- **Volume:** 27,720 readings across both sites
- **Sites:**
  - Marylebone Road - urban roadside
  - Rochester - rural background

## Methods

- **Cleaning:** IQR-based outlier handling and removal of suspect readings, with manual checks to distinguish sensor faults from genuine pollution events
- **Exploratory analysis:** diurnal (time-of-day) patterns and seasonal variation in particulate concentrations
- **Statistical analysis:** Spearman rank correlation to link pollution levels to meteorological drivers
- **Reporting:** condensed into a 7-page report with 12 figures

## Key findings

- Excess is commuter-driven, not simply "urban" due to peaks in the morning (08:00-10:00) and evening (17:00-21:00), along with weekday/weekend contrast in peaks
- Tilling dust from dry spring soils correlates with April peaks of 21µg/m^3 contrasted with a 12µg/m^3 summer baseline  
- European/Easterly winds lift pollutant concentrations to 20µg/m^3 as opposed to the baseline
- Effects of Wet deposition are significant and PM2.5 mirrors PM10. 

## Author

**Connor Costello** - BSc Data Science, University of Bristol
