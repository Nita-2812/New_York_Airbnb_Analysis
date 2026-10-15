# 🏙️ New York City Airbnb Market Analysis & Host Performance Dashboard

## 📌 Project Overview

This project analyzes New York City Airbnb listings using **Microsoft Power BI** to understand the rental market, pricing patterns, neighbourhood performance, host activity, customer reviews, and listing availability.

The interactive dashboard helps users explore how listings are distributed across boroughs, compare prices across room types, identify high-performing hosts, and understand review and availability patterns.

The goal is to turn raw Airbnb data into meaningful insights that can support better business decisions.

## 🎯 Project Objectives

* Analyze Airbnb listing distribution across New York City boroughs.
* Compare average prices across boroughs, neighbourhoods, and room types.
* Understand the distribution of budget, standard, premium, and luxury listings.
* Identify hosts with the highest number of listings and reviews.
* Examine the relationship between host portfolio size and reviews.
* Analyze customer review patterns and listing availability.
* Provide data-driven recommendations to improve market performance.

## 🛠️ Tools & Technologies

* **Microsoft Power BI** — Interactive dashboards and data visualization
* **Power Query** — Data cleaning and transformation
* **DAX (Data Analysis Expressions)** — Measures and calculated columns
* **CSV Dataset** — Data source
* **Data Visualization** — Bar charts, donut charts, scatter plots, maps, and KPI cards

## 📂 Dataset Description

The project uses a New York City Airbnb listings dataset containing information about properties, hosts, locations, prices, reviews, minimum-night requirements, and availability.

The dataset includes fields such as:

| Column | Description |
|---|---|
| `id` | Unique listing identifier |
| `name` | Listing name |
| `host_id` | Host identifier |
| `host_name` | Host name |
| `neighbourhood_group` | Borough or larger location group |
| `neighbourhood` | Neighbourhood name |
| `latitude` and `longitude` | Geographic coordinates |
| `room_type` | Type of accommodation |
| `price` | Listing price |
| `minimum_nights` | Minimum nights required per booking |
| `number_of_reviews` | Number of reviews received by a listing |
| `last_review` | Date of the latest recorded review |
| `reviews_per_month` | Average reviews per month |
| `calculated_host_listings_count` | Number of listings associated with a host |
| `availability_365` | Number of days a listing is available in a year |

## 🧹 Data Cleaning & Transformation

Data preparation was performed in Power Query to improve data quality and make the dataset suitable for analysis.

The main steps included:

* Promoted the first row to column headers.
* Assigned appropriate data types to columns.
* Removed 13 duplicate records based on the listing ID.
* Trimmed unnecessary spaces from text columns.
* Handled missing listing names and host names using `Unknown`.
* Replaced missing `reviews_per_month` values with `0`.
* Removed records with zero prices and handled data errors.
* Checked numeric and date fields for invalid values.
* Created additional categories for pricing and availability.
* Extracted year, month, and quarter from the last review date.

Missing `last_review` dates were retained where no review date was available.

## 📊 Dashboard Pages

### 1. Market Overview

Provides a high-level view of the NYC Airbnb market.

**Visuals included:**
* Listings by Borough
* Listings by Price Category
* Average Price by Borough
* Room Type Distribution
* KPI cards for total listings, total hosts, average price, average availability, and total reviews

**Purpose:** Understand the overall market size, geographical distribution, and pricing differences across boroughs.

### 2. Location Analysis

Explores where Airbnb listings are located and how prices vary by neighbourhood.

**Visuals included:**
* Airbnb Listing Locations map
* Average Price by Neighbourhood
* Room Type Mix by Borough
* Listings by Neighbourhood

**Purpose:** Identify areas with a high concentration of listings, compare neighbourhood prices, and understand the room-type mix across boroughs.

### 3. Room & Pricing

Focuses on room types, rental prices, and minimum-night requirements.

**Visuals included:**
* Price vs Minimum Nights scatter plot
* Average Minimum Nights by Room Type
* Room Type by Price Category
* Average Price by Room Type
* KPI cards for average minimum nights, average price, and maximum price

**Purpose:** Compare room types, understand price differences, and identify unusual price or minimum-night values.

### 4. Host Performance

Analyzes host portfolios and listing performance.

**Visuals included:**
* Top 10 Hosts by Listings
* Top 10 Hosts by Reviews
* Host Listings vs Reviews scatter plot
* Host Portfolio Size Distribution
* KPI cards for total hosts, average listings per host, and average reviews per listing

**Purpose:** Identify hosts with large portfolios, compare review performance, and understand how listings are distributed among hosts.

### 5. Reviews & Availability

Examines review activity and the availability of Airbnb listings.

**Visuals included:**
* Review Activity Over Time
* Reviews vs Availability scatter plot
* Reviews by Borough
* Average Availability by Room Type
* Listings by Availability Category
* KPI cards for total reviews, average reviews per listing, average minimum nights, and average availability

**Purpose:** Understand review patterns, compare availability across room types, and explore the relationship between reviews and availability.

## 🧮 DAX & Feature Engineering

DAX measures were used to calculate important business metrics, including:

* **Total Listings** — Counts Airbnb listings.
* **Total Hosts** — Counts unique hosts.
* **Average Price** — Calculates the average listing price.
* **Total Reviews** — Calculates the total recorded reviews.
* **Average Reviews per Listing** — Measures average reviews for a listing.
* **Average Availability** — Calculates average available days.
* **Average Minimum Nights** — Calculates the average minimum-night requirement.
* **Average Listings per Host** — Measures the average number of listings per host.

Additional calculated columns were created for:

* Price Category
* Availability Category
* Review Year
* Review Month
* Review Quarter
* Host Portfolio Size

These calculations support filtering, comparisons, and interactive analysis.

## 💡 Key Insights

The dashboard highlights several important patterns in the dataset:

* **Market distribution:** Manhattan and Brooklyn contain substantially more listings than the other boroughs.
* **Neighbourhood pricing:** Average prices vary considerably across neighbourhoods, making location an important factor in pricing analysis.
* **Room type:** Entire homes/apartments have the highest average price among the three room types shown.
* **Price categories:** Budget listings form the largest category in the current dashboard.
* **Host performance:** A small number of hosts manage many listings, while most hosts have smaller portfolios.
* **Availability:** The Low Availability category contains the largest number of listings in the current dashboard.
* **Reviews:** Brooklyn and Manhattan contribute the largest review totals among the boroughs shown.
* **Outliers:** A small number of listings have unusually high prices or minimum-night requirements and may require further investigation.

These are descriptive findings from the dashboard; the visuals alone do not prove why the patterns occur.

## 📌 Business Recommendations

1. **Improve market coverage:** Investigate opportunities to attract more hosts in boroughs with fewer listings.
2. **Review pricing strategies:** Compare prices by neighbourhood and room type before setting competitive prices.
3. **Support smaller hosts:** Provide guidance on listing quality, pricing, photographs, and guest communication.
4. **Monitor unusual listings:** Review extreme prices and minimum-night requirements to check for data-quality issues or unusual business rules.
5. **Improve guest experience:** Monitor reviews and encourage hosts to respond to guest feedback.
6. **Use interactive filters:** Compare boroughs, room types, and price categories before making business decisions.

## 📈 Skills Demonstrated

* Data cleaning and transformation using Power Query
* Data analysis using DAX
* Interactive dashboard development
* KPI design and business metric calculation
* Geographic and comparative analysis
* Exploratory data analysis
* Data storytelling and business recommendations

## 🚀 Project Outcome

This project demonstrates how raw Airbnb listing data can be transformed into an interactive Power BI dashboard for exploring the New York City rental market.


