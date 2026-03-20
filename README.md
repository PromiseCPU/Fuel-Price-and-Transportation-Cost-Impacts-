# FUEL PRICE AND TRANSPORTATION COST IMPACTS 
## Overview:
This report presents a comprehensive data analytics study on the impact of fuel price fluctuations on transportation costs in the country. The analysis explores fuel consumption patterns, cost distribution, route performance, and carbon dioxide (CO2) emission trends across four major transport modes: Car, Bus, Truck, and Bike.
The project was built end-to-end: from raw data ingestion and cleaning, through exploratory analysis, to an interactive three-page Power BI dashboard (Fleet Overview, Fuel and Cost Analysis, and CO2 emissions and Efficiency). It is designed to demonstrate the application of data analytics skills: data wrangling, DAX calculations, storytelling with visuals, and actionable business intelligence.
The analysis was motivated by the real-world relevance of fuel subsidy removal, which has had cascading effects on transport affordability, logistics costs, and carbon footprints across the country.

## Sector:
### Industry:
Energy, Transport & Logistics 
### Currency:
NGN
### Period:
January 2023 - December 2025.

## Problem Statement:
Fuel subsidy removal caused petrol and diesel prices to surge to all-time highs, creating an acute cost crisis across the transport sector. Fleet operators, logistics companies, and transport agencies lacked structured, data-driven tools to:
* Understand how fuel price changes translate to per-trip and per-kilometre cost increases across different vehicle types.
* Quantify the variation in fuel efficiency between transport modes (Car, Bus, Truck, Bike).
* Identify which routes and vehicle age cohorts bear the highest operational and environmental cost.
* Measure CO2 emission trends by fuel type and transport mode to inform fleet decarbonisation decisions.
* Make evidence-based decisions on fleet composition, route optimisation, and fuel-type transitions.

This project addresses these gaps by building a structured analytical framework and visual dashboard that empowers stakeholders - from fleet managers to policy analysts - to make informed, data-backed decisions.

## Tools Used:
### MS Excel:
Data cleaning and Exploratory Data Analysis.

### Power BI (Power query, BI desktop, DAX):
BI Desktop (Dashboard & Visualization), Power Query ( Extract, Transform and Load (ETL))

### GitHub & Google Drive:
Portfolio Hosting

## Dataset:
An excel dataset downloaded from Kaggle. All data cleaning was carried out in MS Excel, while the dataset was transferred to Power BI for dashboard/ visualization purposes.

Dataset Summary: 1000 Total records, 15 Features/ columns , (2023 - 2025) Date range, 576 Unique features.

## Questions & KPIs:
### Questions:
* What is the total and average fuel cost across all transport modes and fuel types?
* Which transport mode consumes the most fuel and incurs the highest costs?
* How does vehicle age correlate with fuel consumption and CO2 emissions?
* Which routes record the highest total distance and cost burden?
* How have fuel costs and emissions trended over the 2023–2025 period?
* What is the CO2 emission profile by fuel type, and which type is most efficient?
* How does fuel cost distribute across cost bins (Extreme, Very High, High, Moderate, Medium, Low, Very Low)?

### KPI Metric:
* Total Fuel Consumed (40.84K litres/kWh)
* Total Fuel Cost (₦56M (approx.))
* Total CO2 Emissions (109.83K kg)
* Total Distance Traveled (335K km)
* Average Fuel Consumed (44.34 units/trip)
* Average Fuel Cost (₦60.98K / trip)
* Average CO2 Emissions (119.25 kg / trip)
* Maximum CO2 per km (11.50 kg/km)

## Process:
### Step 1 ~ Data Collection:
The dataset was sourced as a structured Excel file containing 1,000 trip records from road transport operations. It includes both commercial and private vehicles across multiple routes, spanning a three-year period with deliberate inconsistencies introduced to simulate real-world data quality challenges.

### Step 2 ~ Data Cleaning & Transformation
* Loaded data into Power Query (Power BI) and Microsoft Excel for parallel cleaning workflows.
* Standardised all categorical fields (Transport_Mode, Fuel_Type, Fuel_Unit, Distance_Unit) for uniformity.
* Converted all date formats to a consistent DD-MM-YYYY standard.
* Treated the single null Fuel_Consumed entry using median substitution per transport mode group.
* Created a corrected Fuel_Unit column distinguishing Electric (kWh) from conventional (Litres) vehicles.

### Step 3 ~ Feature Engineering
* Created Vehicle_Age_Years bins: 0–4 yrs, 5–8 yrs, 9–12 yrs, 13–16 yrs, 17+ yrs.
* Created CO2 Emissions bins: (0–50), (51–100), (101–150), (151–200), (201–250), (251–300), (301–350).
* Created Fuel_Cost bins: Very Low, Low, Medium, Moderate, High, Extreme, Very High.
* Extracted Trip Year and Trip Date Bin (year-level grouping) from the Trip_Date column.
* Calculated CO2 emissions per km, fuel efficiency , fuel cost per km, as derived measures for efficiency comparison.

### Step 4 ~ Exploratory Data Analysis (EDA)
* Ran frequency distributions on transport mode, fuel type, and route.
* Analysed fuel consumption vs. distance scatter to detect outliers and patterns.
* Assessed CO2 emissions by fuel type and vehicle age to validate hypotheses on older vehicle inefficiency.
* Aggregated total distance travelled, and CO2 emissions by route for geographic insight.

### Step 5 ~ Dashboard Development
* Built a 3-page Power BI dashboard: Fleet Overview, Fuel & Cost Analysis, CO2 Emissions & Efficiency.
* Applied a consistent navy-and-orange brand theme for professional visual identity.
* Added slicers for Fuel Type, Fuel Unit, Transport Mode, and CO2 Emission Bins for interactive filtering.
* Embedded navigation buttons between pages for seamless user experience.
* Charts used:  Donut chart, cards, tree map, table, clustered bar chart, gauge, line chart, ribbon chart, stacked area chart, line & stacked column chart.

### Step 6 ~ Insight Extraction & Reporting
* Synthesised visual findings into narrative insights for each dashboard page.
* Produced actionable recommendations for fleet managers and policy stakeholders.
* Packaged report as a portfolio document for GitHub and Google Drive publication.

## Visualization/ Dashboard (snipping tool)
An interactive end-to-end 3-page Power BI dashboard developed on Power BI Desktop.

### Page 1 ~ Fleet Overview
The Fleet Overview page provides a high-level executive summary of fleet operations. It features four headline KPI cards, a fuel types donut chart, the top 9 routes by total distance, a trip activity bar chart by year, transport mode tiles, and a vehicle age distribution treemap. Together, these visuals deliver a comprehensive operational picture at a glance.
![image alt](https://github.com/PromiseCPU/Fuel-Price-and-Transportation-Cost-Impacts-/blob/6a6880ee736a9cae02e55cdaa15b9110597c03e4/sFleet.png)

### Page 2 ~ Fuel & Cost Analysis
The Fuel & Cost Analysis page focuses on the economics of fleet operations. It shows average fuel consumption and cost KPIs, a speedometer gauge for fuel consumption range, a fuel cost distribution by bin (bar chart), a scatter plot of fuel consumption vs. distance, and a horizontal bar chart of total fuel consumed by transport mode.

### Page 3 ~ CO2 Emissions & Efficiency
The Emissions & Efficiency page examines the environmental footprint of the fleet. It displays emission KPIs, a route-level CO2 emissions table, a time-series bar chart of CO2 by fuel type (2023–2025), an area chart of total vehicle age by emission bin, a scatter of average CO2 per km vs. distance, and interactive transport mode and emission bin filters.

## Key Insights:
### Fleet Overview:
* The fleet is balanced across four transport modes — each accounting for roughly 25% of trip records — with Car (26.49 %) and Truck (25.1%) slightly leading Bus (25.1%) and Bike (23.5%).
* Trip volumes peaked in 2024 with 394 recorded trips, compared to lower activity in 2023, suggesting fleet growth or improved data capture over time.
* The route Zaria-Owerri recorded the highest total distance at 1,027 km in the top routes analysis, followed by Zaria-Oyo (798 km) and Zaria-Ondo (618 km).
* Vehicles in the 0–4 year age bracket dominate the vehicle age distribution (value: 2.02K), suggesting a relatively modern fleet or high vehicle turnover.

### Fuel & Cost Analysis:
* Total fuel cost reached approximately ₦56 million across 1,000 trips, with an average cost of ₦60,980 per trip — a figure that underscores the cost burden on commercial operators post-subsidy removal.
* Cars consume the most total fuel (11.1K units), followed by Buses, Trucks, and Bikes — consistent with higher car volume in the dataset.
* The fuel cost distribution is left-skewed: the majority of trip costs fall in the 'Very High' bin (₦12M), with a steep decline toward 'Very Low' (₦1M), indicating most trips are expensive.
* Average fuel consumed per trip is 44.34 units, with a wide range of 3.00 to 99.90, suggesting extreme variability in trip length, vehicle efficiency, and load factors.
* The scatter of fuel consumption vs. distance shows a non-linear relationship — short routes occasionally record disproportionately high consumption, pointing to urban stop-start driving as a fuel inefficiency driver.

### CO2 Emissions & Efficiency:
* Diesel-powered vehicles in 2024 recorded the highest cumulative CO2 emissions (~22K kg), making diesel the largest contributor to the fleet's carbon footprint.
* Electric and Hybrid vehicles show markedly lower emission profiles across both 2023 and 2024, validating the environmental case for fleet electrification.
* The maximum CO2 per km across the fleet is 11.50 kg/km, significantly above typical benchmarks, suggesting some older or overloaded vehicles are highly inefficient.
* The Zaria-Owerri route alone accounts for 317.80 kg of CO2 emissions — the highest single route in the table — reflecting its outsized distance and likely heavy vehicle deployment.
* Vehicles in the (0–50) CO2 emissions bin have the highest associated vehicle age (2K years total), suggesting newer vehicles produce less CO2 per trip despite more miles covered.
* Average CO2 emissions per trip stand at 119.25 kg, with total fleet emissions of 109.83K kg — a figure that carries significant policy implications for the transport decarbonisation agenda.

## Conclusion:
This data analytics project successfully demonstrates the application of end-to-end analytical skills - data cleaning, transformation, EDA, KPI design, and visual storytelling - to a high-relevance real-world problem: the economic and environmental impact of fuel price escalation in the transport sector. 

The analysis reveals that the road transport fleet is operationally diverse but economically stressed. The post-subsidy fuel price spike has pushed average trip fuel costs to nearly ₦61,000, with the bulk of costs concentrated in the 'Very High' cost bin. Cars bear the greatest aggregate fuel burden, while Trucks account for the longest routes and highest CO2 per route. 

Diesel remains the dominant and most polluting fuel type, even as the data shows Electric and Hybrid vehicles beginning to enter the fleet.
From a sustainability view, the fleet's average CO2 emission of 119 kg per trip is considerable, and the Zaria corridor routes (Zaria-Owerri, Zaria-Oyo, Zaria-Ondo) emerge as both high-distance and high-emission corridors deserving priority attention.

The Power BI dashboard built in this project provides a decision-support tool that fleet managers, logistics planners, and transport policy analysts can use to monitor performance, model cost scenarios, and prioritise decarbonisation interventions. The three-page structure: Fleet Overview, Fuel & Cost Analysis, and Emissions & Efficiency, ensures that both operational and strategic perspectives are served.

## Recommendation:
### For Fleet Operators:
* Prioritise the retirement of vehicles aged 13 years and above, which are associated with the highest CO2 emission bins (201–350 kg range), and replace them with Hybrid or Electric alternatives.
* Introduce route-level fuel efficiency benchmarks for the top 10 highest-cost routes (particularly the Zaria corridors) and enforce driver compliance targets.
* Shift Urban Car fleets — the highest total fuel consumers — toward Compressed Natural Gas (CNG), Hybrid (the combination of petrol/diesel engine and electric + battery), or Electric Vehicles options where fuel station infrastructure permits, to reduce both cost and emissions.

### For Transport Policy Analysts & Government Agencies:
* Invest in Electric Vehicle (EV) charging infrastructure along high-frequency freight corridors (Lagos-Ibadan, Abuja-Keffi, Zaria-Owerri) to accelerate fleet electrification.
* Introduce tiered fuel taxation that rewards low-emission vehicles while creating fiscal incentives for fleet operators to transition away from diesel.
* Develop a national Transport Emissions Dashboard — a public-facing version of this analysis — to create transparency and accountability around the transport sector's CO2 contribution.

### For Data & Analytics Teams:
* Expand the dataset to include GPS-level route data to enable geospatial analysis of fuel consumption hotspots and congestion-linked inefficiency zones.
* Incorporate fuel pump price data from the NNPC (Nigeria National Petroleum Corporation) to enable dynamic cost modelling as prices continue to fluctuate.
* Build predictive models (regression or time-series) to forecast quarterly fuel cost exposure at the fleet and route level, enabling proactive budgeting (Data Science).
* Automate the Power BI dashboard refresh pipeline using Power BI Service and scheduled gateway refresh, converting this static report into a live operational monitoring tool.

(Q.E.D)

