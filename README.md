# Electric Vehicle Market Performance & Insights

A Tableau-based analysis of electric vehicle sales, manufacturers, battery technologies, and global market trends.

## Project Overview

**Electric Vehicle Market Performance & Insights** explores EV market data through sales, manufacturer performance, battery technology, regional distribution, and customer ratings.

The project uses **Tableau Public** to create visualizations and an interactive dashboard.

## Objectives

- Analyze EV sales by manufacturer, region, and manufacturing country.
- Identify top-performing manufacturers based on annual sales.
- Explore battery technology distribution and capacity.
- Analyze EV sales trends by model year.
- Examine customer ratings and vehicle-count distribution.
- Present findings through interactive visualizations and a dashboard.

## Tableau Dashboard

[View Interactive Tableau Dashboard](https://public.tableau.com/views/Book1_17931658458430/Dashboard1)

## Visualizations

The project contains **9 Tableau visualizations**:

| No. | Visualization | Chart Type |
|:---:|---|---|
| 1 | Top 10 Manufacturers by Sales | Horizontal Bar Chart |
| 2 | EV Sales by Market Region | Bar Chart |
| 3 | Battery Technology Distribution | Distribution Chart |
| 4 | EV Sales Trend by Model Year | Trend / Line Chart |
| 5 | Battery Type Share | Pie Chart |
| 6 | EVs by Manufacturing Country | Country Distribution |
| 7 | Average Battery Capacity by Battery Type | Comparison Chart |
| 8 | Customer Rating vs. Vehicle Count | Bar Chart |
| 9 | EV Sales by Country | Country-wise Sales Chart |

## Dataset

The dataset contains two CSV files with **37 attributes** describing EV characteristics, sales, and market information.

| File | Records |
|---|---:|
| `ev_market_train.csv` | 200,000 |
| `ev_market_test.csv` | 100,000 |
| **Total** | **300,000** |

### Key Attributes

- **Vehicle:** `vehicle_id`, `model_name`, `manufacturer`, `model_year`, `category`
- **Geography:** `manufacturing_country`, `market_region`
- **Battery:** `battery_capacity_kwh`, `battery_type`, `battery_cycle_life`, `battery_degradation_pct_5yr`
- **Performance:** `range_km`, `efficiency_wh_per_km`, `motor_power_kw`, `torque_nm`, `top_speed_kmph`
- **Market:** `annual_sales_units`, `price_usd`, `resale_value_pct_3yr`
- **Customer & Ownership:** `customer_rating`, `safety_rating_stars`, `warranty_years`, `insurance_cost_usd_yearly`

## Data Preparation

- Reviewed dataset structure, dimensions, and data types.
- Checked missing values in relevant fields.
- Identified duplicate vehicle identifiers.
- Reviewed field values and categories.
- Prepared dimensions and measures for Tableau visualizations.

> **Note:** Some fields in the training dataset contain missing values. Aggregations should account for nulls, and duplicate `vehicle_id` values should be checked before using distinct vehicle counts.

## Key Areas of Analysis

### Manufacturer & Sales Performance
- Compare annual EV sales across manufacturers.
- Identify the top 10 manufacturers by sales.
- Analyze regional and country-level sales distribution.

### Battery Technology
- Explore battery-type representation in the dataset.
- Compare battery capacity across battery technologies.
- Review battery-related specifications.

### Customer Perspective
- Analyze customer rating distribution.
- Compare vehicle counts across rating levels.
- Explore customer-related attributes alongside vehicle specifications.

## Website

The project website is developed using **HTML, CSS, and JavaScript**.

### Features
- Responsive light-theme interface.
- Project overview and summary cards.
- Embedded Tableau Public dashboard.
- Visualization gallery.
- Project story section.
- Calculated-field reference.
- Searchable and filterable dataset field explorer.
- GitHub repository link placeholder.

### Run Locally

1. Download or clone the repository.
2. Open `index.html` in a modern web browser.
3. Navigate to the dashboard section to explore the embedded Tableau dashboard.

No additional installation or build process is required for the static website.

## Tools & Technologies

| Tool | Purpose |
|---|---|
| Tableau Public | Data visualization and dashboard creation |
| HTML5 | Website structure |
| CSS3 | Styling and responsive layout |
| JavaScript | Interactive website features |
| CSV | Dataset format |
| Git & GitHub | Version control and repository hosting |

## Repository Structure

```text
Electric-Vehicle-Market-Performance-Insights/
├── Dataset/
│   ├── ev_market_train.csv
│   └── ev_market_test.csv
├── index.html
└── README.md
```

*Update this structure to match the actual files and folders in your repository.*

## Author

**Kriti Punjabi**  
Data Analytics Project
