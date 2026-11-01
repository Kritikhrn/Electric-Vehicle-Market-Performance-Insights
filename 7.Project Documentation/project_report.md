# Electric Vehicle Market Performance & Insights

## Project Overview

The **Electric Vehicle Market Performance & Insights** project analyzes electric vehicle (EV) market data to understand sales performance, regional demand, battery technologies, vehicle specifications, and customer ratings. The project uses data analysis and Tableau visualizations to turn a large dataset into meaningful insights that can support market understanding and business decision-making.

## Objectives

- Analyze EV sales across manufacturers, countries, and market regions.
- Identify leading manufacturers based on annual sales.
- Explore sales trends across model years.
- Understand the distribution of battery technologies.
- Compare battery capacity across battery types.
- Examine customer ratings and vehicle popularity.
- Present findings through an interactive Tableau dashboard and a supporting website.

## Dataset Description

The project uses two CSV files:

| File | Description | Records |
|---|---|---:|
| `ev_market_train.csv` | Training dataset | 200,000 |
| `ev_market_test.csv` | Testing dataset | 100,000 |

The dataset contains **37 columns** describing EV models, manufacturers, specifications, market information, sales, and customer feedback. The data covers model years **2018–2026** and includes multiple manufacturers, vehicle categories, market regions, and battery types.

### Important Attributes

- **Vehicle and manufacturer:** `vehicle_id`, `model_name`, `manufacturer`, `model_year`
- **Geography:** `manufacturing_country`, `market_region`
- **Classification:** `category`, `battery_type`, `drivetrain`, `recommended_use_case`
- **Battery and performance:** `battery_capacity_kwh`, `battery_cycle_life`, `battery_degradation_pct_5yr`, `range_km`, `efficiency_wh_per_km`, `motor_power_kw`, `torque_nm`, `top_speed_kmph`, `acceleration_0_100_sec`
- **Charging:** `max_dc_charging_kw`, `charging_dc_fast_time_min`, `charging_ac_time_hr`, `num_charging_ports`
- **Commercial metrics:** `price_usd`, `insurance_cost_usd_yearly`, `resale_value_pct_3yr`, `annual_sales_units`
- **Customer and sustainability:** `customer_rating`, `safety_rating_stars`, `co2_saved_tons_per_year`

## Data Preparation

The training dataset contains missing values in selected columns, including:

- `battery_cycle_life`
- `resale_value_pct_3yr`
- `infotainment_screen_inch`
- `annual_sales_units`
- `customer_rating`

The data preparation process should include:

1. Inspecting data types and column consistency.
2. Checking and handling missing values according to the analytical requirement.
3. Identifying duplicate vehicle records.
4. Validating sales, rating, and specification values.
5. Creating calculated fields or aggregations for Tableau.
6. Ensuring consistent dimensions and measures across worksheets.

A duplicate `vehicle_id` was identified in the training dataset during initial inspection. This should be reviewed before vehicle-level analysis to avoid double-counting.

## Methodology

The analysis follows these stages:

1. **Data understanding:** Review the schema, dimensions, measures, and data quality.
2. **Data preparation:** Handle missing values and review duplicates.
3. **Exploratory analysis:** Compare sales, manufacturers, regions, countries, battery types, and ratings.
4. **Visualization:** Build individual Tableau worksheets using appropriate chart types.
5. **Dashboard development:** Combine worksheets into an interactive dashboard.
6. **Storytelling:** Organize the visualizations into a sequence that communicates the main findings.
7. **Web integration:** Publish project information and provide access to the Tableau dashboard through a project website.

## Tableau Visualizations

The project includes the following nine visualizations:

| No. | Visualization | Chart Type | Analytical Purpose |
|---:|---|---|---|
| 1 | Top 10 Manufacturers by Sales | Horizontal bar chart | Identify manufacturers with the highest annual sales |
| 2 | EV Sales by Market Region | Bar chart | Compare sales performance across market regions |
| 3 | Battery Technology Distribution | Bar chart | Explore the number of vehicles across battery types |
| 4 | EV Sales Trend by Model Year | Line chart | Examine changes in sales over model years |
| 5 | Battery Type Share | Pie chart | Show the proportional contribution of battery types |
| 6 | EVs by Manufacturing Country | Treemap or geographic distribution | Explore vehicle representation by manufacturing country |
| 7 | Average Battery Capacity by Battery Type | Bar chart | Compare average battery capacity across technologies |
| 8 | Customer Rating vs. Vehicle Count | Bar chart | Examine customer ratings alongside vehicle counts |
| 9 | EV Sales by Country | Bar chart or map | Compare country-level sales performance |

> **Note:** Chart titles and aggregations should match the final Tableau workbook. For sales-based visualizations, use `SUM(annual_sales_units)`; for vehicle counts, use a distinct count of `vehicle_id` where appropriate. Exclude or handle null values explicitly.

## Dashboard

The Tableau dashboard brings the worksheets together to provide a consolidated view of EV market performance. It is designed to help users compare manufacturers, regions, model years, battery technologies, countries, and customer ratings.

**Published Tableau Dashboard:**  
[View the Electric Vehicle Market Dashboard](https://public.tableau.com/views/Book1_17931658458430/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Project Website

A responsive project website presents the project overview, key analytical areas, visualization descriptions, dataset information, and dashboard access.

### Website Features

- Project overview and key metrics
- Tableau dashboard embed with a direct-link fallback
- Descriptions of the nine visualizations
- Project methodology and calculated-field examples
- Dataset exploration section
- Technology stack and project information
- GitHub repository link in the top navigation (to be configured with the repository URL)

### Run Locally

1. Download or clone the project repository.
2. Open `ev_market_analytics_website_v2.html` in a browser.
3. If the Tableau embed does not load, use the direct dashboard link provided on the page.

## Tools & Technologies

- **Tableau:** Interactive visualizations, dashboard, and story
- **Python / Pandas:** Data inspection and preparation (where applicable)
- **CSV:** Dataset storage and exchange
- **HTML / CSS / JavaScript:** Project website
- **GitHub:** Version control and project hosting

## Repository Structure

```text
Electric-Vehicle-Market-Performance/
├── data/
│   ├── ev_market_train.csv
│   └── ev_market_test.csv
├── ev_market_analytics_website_v2.html
├── README.md
└── project_report.md
```

*Update the repository structure to reflect the actual files and folders committed to GitHub.*

## Limitations

- Missing values in some fields may affect particular analyses.
- Sales and rating insights depend on the selected aggregation and null-handling approach.
- The dataset represents the provided records and may not capture the entire global EV market.
- Tableau Public embedding may be restricted by browser settings or platform behavior; the dashboard's direct link remains available.

## Conclusion

The **Electric Vehicle Market Performance & Insights** project demonstrates how data analysis and visualization can be used to explore the EV market from multiple perspectives. By examining manufacturer sales, regional and country-level performance, model-year trends, battery technologies, technical specifications, and customer ratings, the project provides a structured overview of EV market patterns.

The interactive Tableau dashboard and project website make these analyses accessible and support further exploration of the dataset.

## Author

**Kriti Punjabi**
