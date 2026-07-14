# Nijiwa Water Project — Power BI Dashboard

## 📌 Overview
This project analyses water infrastructure and access data for a national water programme covering **28 million people** across **5 provinces**. Using Power BI, I cleaned, modelled, and visualised the data to surface insights on water access, project delivery performance, and budget management — with the goal of helping decision-makers identify where to intervene and where resources are being spent inefficiently.

The dashboard is split into two connected views:
- **Home / Cost Dashboard** — high-level KPIs on population access, project completion, and cost breakdowns by province and improvement type
- **Report Dashboard** — deeper cost analysis by province, location type (rural vs. urban), and budget vs. actual spend

## 🎯 Objectives
- Assess what proportion of the population has access to basic drinking water
- Track project completion rates and identify delivery bottlenecks
- Compare cumulative cost against budget to flag overspend
- Break down cost and access by province and by rural/urban location
- Identify which infrastructure improvements (e.g. drilling wells, installing filters) drive the most spend

## 🗂️ Dataset
The raw data comes from a multi-table water infrastructure dataset, including:

| Table | Description |
|---|---|
| `water_source` | Source ID, type of water source, number of people served |
| `location` | Location ID, town, province, and rural/urban classification |
| `project_progress` | Project status, improvement type, vendor, cost, start/completion dates |
| `infrastructure_cost` | Unit cost per improvement type |
| `vendors` | Vendor details for completed works |
| `visits` | Queue times and visit records at water sources |
| `well_pollution` | Contamination test results for wells |
| `water_source_related_crime` | Incident records linked to water sources |

Data was cleaned and modelled in Excel and Power BI, with relationships built across tables to enable province-, location-, and improvement-level analysis.

## 🛠️ Tools & Skills
- **Power BI** — data modelling (star schema), DAX measures, interactive visuals, drill-through navigation
- **Excel** — initial data cleaning and validation
- **Power Query** — data transformation and shaping

## 📊 Key Insights
- Only **47.8%** of the population has access to basic drinking water, despite 13M+ people already served
- Just **21.6%** of planned projects are complete, with **20K** projects still outstanding
- Cumulative cost (**£33.8M**) has already exceeded the total budget (**£30.5M**) — a ~10% overrun
- **Banjira province** accounts for the largest share of total cost (32.8%, £11.1M)
- **Installing RO filters** is the most expensive improvement type overall (£14M)
- Rural interventions cost noticeably more per project than urban ones, even though total rural and urban spend is nearly split evenly (£17.0M vs. £16.8M)

## 📷 Dashboard Preview
Screenshots of the Home Dashboard and Report Dashboard are included in this repository (`/screenshots`).

## 🚀 How to Use
1. Download `Md_water_services_data_2.xlsx` and the `.pbix` Power BI file
2. Open the `.pbix` file in Power BI Desktop
3. Use the slicers and navigation buttons (Home Page / Report Page) to explore the data by province, location type, and improvement category

## 🙋 About Me
I'm an MSc Public Health student with a background in data analytics (SQL, Power BI, Python, Excel, GIS). This project reflects my interest in applying data analysis to real-world public health and infrastructure challenges. Feel free to connect or reach out if you'd like to discuss the approach or findings.
