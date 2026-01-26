# Power BI: Data Jobs Market Insights (2023–2025H1)

This repository contains two compact analytical dashboards exploring hiring trends, salary patterns and skills demand across the data & analytics job market (2023–2025H1).  
The dashboards were created as part of an internal research initiative supporting workforce planning, recruiter prioritisation, and market intelligence.

The analysis focuses on three practical business questions:

1. **How has demand for data roles evolved over the last 2.5 years?**  
2. **Which roles and skill sets command the strongest salary signals?**  
3. **Where are the highest-value opportunities for sourcing and training?**

Both dashboards use the same underlying dataset but serve different analytical needs.

---

## Download Files (PBIX & Dataset)

Power BI dashboards (.pbix) and the full dataset (.csv) are available in the project’s **Releases**:

**Dashboards:**  
https://github.com/Q-Lesh/PowerBI_Project_2/releases/tag/Dashboards_v1

**Dataset:**  
https://github.com/Q-Lesh/PowerBI_Project_2/releases/tag/Data_v1

> After downloading, update dataset file paths inside Power BI Desktop.

---

## 1. Dashboard — Market Overview (Executive View)

![Dashboard 1](Resources/images/D1.gif)

This single-page view provides a high-level, decision-friendly snapshot suitable for recruiters, HR business partners and workforce planners.

**Highlights:**
- Total job postings volume  
- Median yearly & hourly salary levels  
- Salary-based star index (normalised 1–5 rating)  
- Multi-year demand trend (2023 → 2025H1)  
- Role-level distribution of vacancies  
- Salary comparison by contract type (yearly vs hourly)

**Filters:** Year, job title

**Purpose:**  
Enable rapid orientation before deeper analysis — used during weekly hiring stand-ups and market updates.

---

## 2. Dashboard — Skills & Salary Exploration (Analyst View)

![Dashboard 2](Resources/images/D2.gif)

This dashboard provides deeper analytical flexibility for talent intelligence and operational recruiting teams.

**Key Analytical Components:**
- Skills-per-job & salary KPIs  
- Skill popularity (share/count toggle)  
- Salary medians by job type (yearly/hourly toggle)  
- Tooltip breakdown: role medians + vacancy counts  
- Dynamic measures controlled via parameter tables  
- Country, role and timeframe filtering for precise segmentation  

**Filters:** Year, job title, country, clear-slicers button

**Purpose:**  
Interactive exploration of which skills drive demand and salary variation, helping teams prioritise sourcing focus and training investments.

---

## 3. Data & Modelling (Short Technical Summary)

**Data model differences:**

- **Dashboard 1:**  
  Compact single-table schema optimised for fast slicing & high-level KPIs.

- **Dashboard 2:**  
Compact **star schema** featuring:
  - Date dimension  
  - Skill dimension  
  - Company dimension  
  - Schedule/contract-type dimension  
  - Skill bridge table (many-to-many)  

**Transformations:**
- Type cleaning  
- Harmonised role naming conventions  
- Standardised salary fields (yearly/hourly)  
- Normalised skill lists (tokenisation + expansion)

**DAX Highlights:**
- Salary medians (robust DIVIDE wrappers)  
- Weighted skill popularity metrics  
- Parameter-driven dynamic measure switching  
- Normalised salary star rating (1–5)

The model is intentionally lightweight, following Power BI best practices for small-to-medium analytical applications.

---

## 4. Notes & Positioning

This repository functions as a **supporting mini-case** within a broader BI/analytics portfolio.  
It demonstrates:

- clean PBI modelling,  
- interaction design,  
- multiple-schema thinking,  
- use of bridge tables,  
- and parameter-driven measures.

The scope is intentionally practical:  
**not a forecasting model, not an academic EDA — but a compact, business-applied market intelligence asset.**

