# Power BI: Data Jobs Dashboards (2023–2025H1)

Two compact Power BI dashboards analysing the data job market across 2023–2025H1.  
Both dashboards are built on the same dataset and focus on job volumes, salary levels, and skill demand.  
This repository serves as a supporting mini-case in the portfolio.

---

**Download Dashboards & Dataset**

You can download the Power BI dashboard files (.pbix) and the full dataset (.csv) from the project’s Release section:

Dashboards (PBIX files):
[https://github.com/Q-Lesh/PowerBI_Project_2/releases/tag/Dashboards_v1](https://github.com/Q-Lesh/PowerBi_Project_1/releases/tag/Dashboards_v.1)

Dataset (CSV files):
[https://github.com/Q-Lesh/PowerBI_Project_2/releases/tag/Data_v1](https://github.com/Q-Lesh/PowerBi_Project_1/releases/tag/Data_v.1)

**Important!**
After downloading the dataset, update the file paths in Power BI Desktop.

---

## Dashboard 1 — Market Overview

![Dashboard 1](Resources/images/D1.gif)

A single-page, high-level view showing:

- Total job count  
- Median yearly & hourly salaries  
- Salary-based star rating  
- Job trend over time  
- Job volume by role  
- Salary comparison (yearly vs hourly)

**Filters:** job title, year buttons (2023–2025)

Designed for fast orientation before deeper analysis.

---

## Dashboard 2 — Skills & Salary Exploration

![Dashboard 2](Resources/images/D2.gif)

Built on a star-schema model with date, skill, company, and schedule dimensions.

Key interactive elements:

- Skills-per-job and salary KPIs  
- Skill popularity (share or count, switchable)  
- Salary medians by role (yearly or hourly, switchable)  
- Tooltips with role-level medians and job counts  
- Dynamic measure selection for both major visuals  

**Filters:** year, job title, country, clear-slicers button

---

## Under the Hood (short version)

- Dashboard 1 uses a single-table model  
- Dashboard 2 uses a compact star-schema with a skill bridge table  
- Data preparation: basic type cleaning (Promoted Headers, Changed Type, Renamed Columns)  
- DAX: standard measures (COUNTROWS, MEDIAN, DIVIDE) and simple parameter tables for interactive switching  
- One custom measure adds a normalized 1–5 salary-based star rating

---

## Notes

This project is intentionally scoped as a **supporting mini-case**.  
It demonstrates practical Power BI modelling, clean visuals, and interactive analysis without excessive complexity.


