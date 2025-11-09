# Hotel Business Analytics

## Overview

This project is an enterprise-grade Power BI analytics solution designed to analyze daily performance records across multiple hotel properties. The solution is built upon a robust star schema data model and incorporates time intelligence to provide deep insights into hotel operations.

## Key Features

-   Analyzes over 4,000 daily records across 8 hotel properties.
-   Implements a star schema data model with calendar intelligence.
-   Includes over 50 DAX measures for complex time-based calculations (QoQ/YoY growth, booking analysis, holiday performance).
-   Utilizes advanced Power BI features like:
    -   **Field Parameters:** For dynamic metric switching.
    -   **Bookmarks:** For contextual navigation and saved views.
    -   **Drill-through Pages:** For granular, detailed analysis.
-   Employs conditional formatting and strategic visual design for at-a-glance insights.
-   Designed for self-service analytics, accessible to both executives and analysts.

## Data Model

The data is structured in a star schema with one fact table and four dimension tables. The dataset contains 4,000 rows of sample data.

### Fact Table: Daily Hotel Performance

-   `Date`
-   `Hotel ID`
-   `Rooms Sold`
-   `Rooms Available`
-   `Occupancy Rate`
-   `ADR` (Average Daily Rate)
-   `RevPAR` (Revenue Per Available Room)
-   `Leisure Revenue`
-   `Business Revenue`
-   `Group Revenue`
-   `Total Revenue`
-   `Cancellations`
-   `Booking Window`
-   `Avg Length Of Stay`
-   `Customer Satisfaction`

### Dimension Tables

#### DimDate
-   `Date`
-   `Year`
-   `Quarter`
-   `Month`
-   `Month Name`
-   `Week`
-   `Day Of Week`
-   `Is Weekend`
-   `Is Holiday`
-   `Holiday Name`
-   `Season`

#### DimHotel
-   `Hotel ID`
-   `Hotel Name`
-   `City`
-   `State`
-   `Country`
-   `Star Rating`
-   `Total Rooms`
-   `Property Type`

#### DimPromotion
-   `Promotion ID`
-   `Promotion Name`
-   `Discount Pct`
-   `StartDate`
-   `EndDate`

#### DimCustomerSegment
-   `Segment ID`
-   `Segment Name` (Leisure, Business, Group)

## Reports & Visualizations

The Power BI report is broken down into three main pages:

### 1. Executive Summary

![Executive Summary](ScreenShots/Exec_Summary.PNG)

-   **KPIs:** Displays key performance indicators with growth rates and conditional formatting.
-   **Revenue Table:** Shows a revenue split with a parameter to dynamically switch the displayed column.
-   **Waterfall Chart:** Visualizes revenue by month.
-   **Commentary:** Provides actionable insights into performance based on various criteria.
-   **Interactivity:** Features a filter button in the top-left corner for easy data slicing.

### 2. Booking Analytics

-   **Booking Patterns:** Analyzes booking patterns using various charts.
-   **Dynamic Analysis:** A parameter allows users to select different dimensions to analyze booking patterns.
-   **Commentary:** Offers actionable insights into booking trends.
-   **Interactivity:** Includes filter buttons and navigation buttons for detailed exploration.

### 3. Holiday Analytics

-   **Holiday Impact:** Analyzes the effect of holidays on booking and revenue patterns using charts and tables.
-   **Commentary:** Delivers actionable insights related to holiday performance.
-   **Interactivity:** Provides filter and navigation buttons for user-driven insights.Build a Dynamic TopN report in Power BI
