# Deloitte-Australia-Data-Analytics-Job-Simulation

[![Forage](https://img.shields.io/badge/Forage-Job%20Simulation-blue)](https://www.theforage.com/)
[![Tableau](https://img.shields.io/badge/Tableau-Dashboard-green)](https://www.tableau.com/)
[![Excel](https://img.shields.io/badge/Excel-Data%20Analysis-brightgreen)](https://www.microsoft.com/en-us/microsoft-365/excel)

This repository contains a summary of my work and learnings from completing the **Deloitte Australia - Data Analytics Job Simulation** on Forage. The simulation provided a realistic experience of working as a data analyst for a Big 4 consulting firm, tackling real-world data challenges for a global industrial client.

## Project Overview

The project was divided into two core tasks, focusing on using data to solve business problems related to operational efficiency and workplace equality.

**Task 1: Telemetry Data Analysis & Visualization**
The goal was to analyze 160,000+ machine telemetry records from Daikibo's four global factories to identify which location and machines had the highest downtime.

**Task 2: Gender Pay Equality Analysis**
The goal was to classify gender pay equality scores across job roles and locations to assist in a forensic investigation into internal complaints of gender inequality.

## Task 1: Telemetry Data & Tableau Dashboard

### Objective
To help the client, Daikibo, answer two critical questions:
1.  In which location did machines break the most?
2.  What are the machines that broke most often in that location?

### Process
1.  **Data Import:** Imported a large JSON file containing telemetry data for 9 machine types across 4 factories (Tokyo, Osaka, Berlin, Shenzhen) into Tableau Desktop.
2.  **Data Transformation:** Created a calculated field named `Unhealthy` with a value of 10. This represented the 10-minute interval between messages, indicating potential downtime for each "unhealthy" status received.
3.  **Visualization:** Designed two distinct bar charts within Tableau:
    - **Sheet 1 (Downtime Per Factory):** A high-level view to compare total downtime across all locations.
    - **Sheet 2 (Downtime Per Device Type):** A detailed breakdown to see which specific machines are failing.
4.  **Interactive Dashboard:** Combined both charts into a single, interactive dashboard. I configured a filter action so that selecting a factory on the first chart dynamically updates the second chart to show only the machine data for that specific location.
5.  **Analysis & Insight:** The dashboard immediately highlighted that the **Meiyo (Tokyo)** factory had the highest downtime, and the **Laser Welder** was the most frequent point of failure.

### Tools & Technologies
- Tableau Desktop
- JSON Data Processing

### Key Findings
| Factory | Location | Total Downtime (Units) | Top Failing Machine |
| :--- | :--- | :--- | :--- |
| **Daikibo Factory Meiyo** | Tokyo, Japan | **480** | Laser Welder |
| Daikibo Factory Seiko | Osaka, Japan | - | - |
| **Daikibo Shenzhen** | Shenzhen, China | **390** | Laser Cutter |
| Daikibo Berlin | Berlin, Germany | **20** | (Most Stable) |

**Conclusion:** Operational risks are heavily concentrated in laser-based machinery. The Tokyo factory is a critical area for immediate intervention and maintenance.

### Dashboard Screenshot
![Task 1 Dashboard](https://github.com/dee8864/Deloitte-Australia-Data-Analytics-Job-Simulation/blob/main/%23VISUALS%20Deloitte-Australia-Data-Analytics-Job-Simulation.png)

## Task 2: Gender Pay Equality Classification

### Objective
To support the Forensic Tech team in investigating internal complaints by classifying a "level of gender pay equality" score into actionable categories.

### Process
1.  **Data Review:** Analyzed an Excel file (`Equality Table.xlsx`) containing three columns: `Factory`, `Job Role`, and `Equality Score`.
2.  **Data Classification:** Created a new column named `Equality Class`. I used Excel to categorize the score based on the following logic:
    - `Fair`: Scores within the range of -10 to +10.
    - `Unfair`: Scores less than -10 or greater than +10.
    - `Highly Discriminative`: Scores less than -20 or greater than +20.
3.  **Outcome:** This simple classification transformed a raw integer score into a clear, business-friendly category that allows leadership to quickly identify problematic roles and locations for further investigation.

### Tools & Technologies
- Microsoft Excel

### Example Table
| Factory | Job Role | Equality Score | Equality Class |
| :--- | :--- | :--- | :--- |
| Daikibo Berlin | Engineer | -9 | Fair |
| Daikibo Shenzhen | Supervisor | 30 | Highly Discriminative |

## Skills Demonstrated

- **Data Analysis**
- **Data Visualization (Tableau)**
- **Forensic Technology**
- **Spreadsheet Skills (Excel)**
- **Data Modeling & Transformation**
- **Log Analysis**
- **Data Storytelling & Formal Communication**

## About This Repository

This repository serves as a portfolio piece to showcase my practical data analytics skills and my ability to deliver business-focused solutions using industry-standard tools. The project was completed as part of a job simulation with Deloitte Australia on the Forage platform.

*Note: All data used is sample data provided by the simulation platform. The findings are for demonstrative purposes only.*

# Author

**Deepanshu Sharma**

MBA (Business Analytics)

[LinkedIn](https://www.linkedin.com/in/deepanshu-sharma-8864ds/)

[GitHub](https://github.com/dee8864)

![Task 1 Dashboard](https://github.com/dee8864/Deloitte-Australia-Data-Analytics-Job-Simulation/blob/main/%23CERTIFICATE%20Deloitte-Australia-Data-Analytics-Job-Simulation.png)
