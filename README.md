# Project Overview

The Tableau Sales Dashboard is an interactive business intelligence solution designed to analyze sales performance, profitability trends, and customer behavior over multiple fiscal years. Organizations often struggle to identify the exact drivers of profit and loss due to isolated, fragmented raw transaction logs. This project solves that problem by transforming granular sales and customer metrics into unified, actionable visualizations. It enables executives, sales managers, and marketing teams to evaluate key performance indicators (KPIs), detect seasonal anomalies, and perform deep-dive subcategory analyses to drive data-backed strategic decisions.

### LINK : https://public.tableau.com/views/Dashbaord-Sales_17809534096610/Dashboard1?:language=en-US&:sid=&:redirect=auth&publish=yes&showOnboarding=true&:display_count=n&:origin=viz_share_link


## Requirements 

#### System Dependencies

Tableau Desktop Professional Edition or Tableau Public Desktop (Version 2023.1 or higher recommended)

Operating System: Microsoft Windows 10 


## Software Versions and Prerequisites 

Data Source Compatibility: Structured relational data files (e.g., Microsoft Excel .xlsx,  extracts connecting to Sample - Superstore data models)

Active internet connection if publishing to or sync-testing with Tableau Public / Tableau Cloud

## Hardware and Software Limits

Minimum 4 GB RAM (8 GB or higher recommended for smooth rendering of complex Level of Detail expressions)

Dashboard layout configured with fixed dimensions to guarantee alignment and visual structure across standard desktop resolutions


## Tools and Technologies

Business Intelligence & Visualization: Tableau Desktop / Tableau Public

Data Organization: Relationships and logical layer configuration for multi-table linking

Analytical Expressions: Level of Detail (LOD) Expressions, custom calculated fields, and conditional parameters

Design & Layout Production: Presentation software (for customized dashboard backgrounds) and coordinate-based floating/tiled layout structures


## Challenges Faced

Date Equalization for Year-over-Year (YoY) Comparisons: Raw date values across separate historical years made it difficult to map matching seasonal weeks accurately. This was overcome by building robust logical calculations that normalized date fields to a standardized relative timeframe, allowing a perfectly aligned chronological comparison between the current year and the previous year.

Complex Multi-Metric Layout Density: Fitting comprehensive product performance, sales metrics, weekly trend indicators, and profitability calculations into a single workspace threatened to clutter the user interface. This challenge was resolved by separating the analysis into dedicated Sales and Customer dashboards, leveraging interactive parameter-based navigation actions so users could cleanly toggle between distinct focal points.

Automating Dynamic Threshold Highlights: Designing an automated way to highlight weeks that fell below or above organizational benchmarks without hardcoding static numbers was highly difficult. This was overcome by writing dynamic calculations to isolate individual data points and applying discrete color encoding rules to instantaneously flag profit and loss variances.


## Key Insights
Dashboard:

![image alt](https://github.com/rt5899-art/Tableau-Sales-Dashboard/blob/main/Sales%20_Tableau.png?raw=true)


#### Pronounced Q4 Seasonal Demand Acceleration: 

November and December consistently achieve the highest sales volumes across the multi-year cycle. This surge reflects highly concentrated holiday demand, contrasting starkly with January and February, which exhibit a post-holiday sales contraction.

#### Distinct Outliers in Subcategory Profit Margins:

High-volume sales do not inherently guarantee healthy profit margins. Specific product segments like Phones, Chairs, and Copiers maintain strong profitability markers, whereas other segments such as Tables, Bookcases, and Supplies frequently incur losses despite generating significant baseline revenue.

#### Shifting Purchase Frequency and Engagement: 

Historical transaction patterns from 2020 to 2021 showed that the majority of individual customers placed only a single order per fiscal year. In contrast, analytics from 2022 to 2023 demonstrate an increase in engagement, with most active customers averaging two or more orders per year. This structural change points to rising customer loyalty and improved retention rates.


## Recommendations for Improvements

#### Implement Live Advanced Forecasting Models: 

Integrate exponential smoothing or ARIMA forecasting algorithms directly into the time-series views to generate real-time predictive sales corridors for future quarters based on historical variance.

#### Incorporate Row-Level Security and Regional Filters:

Implement dynamic user-attribute parameters so that regional sales directors automatically filter dashboards down to their specific operational territories upon logging in.

#### atabase Query Performance Tuning:

Materialize data extracts instead of relying on live flat files to speed up the execution of nested Level of Detail (LOD) expressions, reducing dashboard loading lag when working with larger datasets.
