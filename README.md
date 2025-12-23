# PowerBI: Data Jobs Dashboard (2023-2025H1)

## Overview

This repository contains two Power BI dashboards built on a shared, updated dataset (**2023 - 2025H1**) of data-related job postings.
The dashboards are designed to provide a clear, practical view of the data job market, focusing on job volume, skills demand, and compensation trends.

Both dashboards use the same underlying data model, but serve different analytical purposes.

## Dataset

**Time range**: January 1, 2023 – June 30, 2025.

**Coverage**: job titles, salaries (yearly & hourly), skills, locations, platforms, work format, benefits

A future update will extend the dataset to cover three full calendar years.
To make temporal analysis easier, year-based filter buttons were added, allowing quick switching between years without manual slicer adjustments.

## Dashboards

1. **Data Jobs Dashboard 1**

![Dashboard 1](Resources/images/D1.gif)

**Purpose:**
High-level market overview.

**Key characteristics:**
- Single-page dashboard (the drill-through page was intentionally removed)
- Focus on:
   - Total job volume
   - Median salaries
   - Job distribution by title
   - Trends over time
- Optimized for fast exploration and comparison

This version is intentionally simple and compact, suitable as an entry point or executive-style overview.

2. **Data Jobs Dashboard 2**

![Dashboard 2](Resources/images/D2.gif)

**Purpose:**
Deeper analytical exploration with richer interaction.

**Key characteristics:**

- Single focused page with extended interactivity
- Includes:
    - Skills popularity (by share and absolute count)
   - Salary comparison across job titles
   - Dynamic measure switching
   - Country and job title filtering
- Designed for hands-on analysis rather than summary reporting

This version prioritizes analytical flexibility while keeping the layout readable and structured.

## Data Model & Approach

- Star-schema–based model
- Separate fact and dimension tables
- Transformations handled in Power Query
- Metrics calculated using DAX measures
- Shared logic across both dashboards to ensure consistency


## Skills & Features Used

This project applies a focused set of Power BI capabilities to turn a large dataset of job postings into clear, actionable insights.

- **Data Transformation (Power Query):** 
Cleaned and structured the raw dataset by fixing data types, standardizing fields, removing inconsistencies, and preparing dimensions and fact tables.

- **Measures (DAX):** 
Created essential measures for analysis, including Median Yearly Salary, Median Hourly Salary, Skills Per Job, and Job Count.

- **Core Visualizations:** 
Used Bar, Column, Line, and Scatter charts to explore job volume, skills demand, temporal trends, and compensation patterns.

- **KPI Cards & Tables:** 
Displayed key metrics using Cards and detailed job-level breakdowns using Tables.

- **Layout & Design:** 
Built a clean, structured dashboard layout optimized for clarity, readability, and fast interpretation of trends.

- **Interactive Controls:** 
   - Slicers for filtering by Job Title, Year, Country, and other key fields.
   - Buttons for switching views and clearing filters.


---

## Conclusion

These dashboards demonstrate how structured data modeling, Power Query transformations, and effective visualization choices can convert raw job posting records into a practical analytical tool. Users can filter, explore, and compare roles, salaries, skills, and trends across multiple time periods with minimal friction.

