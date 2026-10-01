<p align="center">
  <img src="screenshots/banner.png" alt="Logistics & Delivery Performance Intelligence Dashboard" width="100%">
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" alt="Power BI">
  <img src="https://img.shields.io/badge/DAX-Measures-176B50?style=for-the-badge" alt="DAX">
  <img src="https://img.shields.io/badge/Excel-Data%20Prep-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" alt="Excel">
  <img src="https://img.shields.io/badge/Dataset-Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" alt="Kaggle">
</p>

<p align="center"><b>An interactive Power BI project for logistics analytics, delivery performance monitoring and operational cost analysis.</b></p>

<p align="center">
  <a href="#-project-overview">Overview</a> •
  <a href="#-dashboard-preview">Preview</a> •
  <a href="#-dashboard-structure">Structure</a> •
  <a href="#-dax-measures">DAX</a> •
  <a href="#-key-findings">Findings</a> •
  <a href="#-limitations">Limitations</a>
</p>

---

## 📌 Project Overview

The **Logistics & Delivery Performance Intelligence Dashboard** analyzes 25,000 delivery records across multiple delivery partners, regions, package types, vehicle types and delivery modes. It turns raw logistics data into interactive charts, KPI cards, slicers and DAX measures, so users can see where deliveries are delayed, what drives cost and how customers rate the service.

**Three business questions drive the project**

- 🚚 How can delivery performance be monitored and improved?
- 💰 Which operational categories explain delivery costs?
- ⭐ How can customer ratings be used to evaluate service quality?

### At a glance

| 📦 Deliveries | ⏱️ Delay Rate | ✅ On-Time Rate | 💰 Avg. Cost | ⭐ Avg. Rating |
| :---: | :---: | :---: | :---: | :---: |
| **25,000** | **26.7%** | **73.3%** | **₹864.94** | **3.67 / 5** |

---

## 🖼️ Dashboard Preview

### Page 1 – Executive Overview
<img src="screenshots/page1_executive_overview.png" alt="Executive Overview" width="100%">

### Page 2 – Delivery Performance Analysis
<img src="screenshots/page2_delivery_performance.png" alt="Delivery Performance Analysis" width="100%">

### Page 3 – Cost & Operations Analysis
<img src="screenshots/page3_cost_operations.png" alt="Cost and Operations Analysis" width="100%">

### Page 4 – Customer & Service Analysis
<img src="screenshots/page4_customer_service.png" alt="Customer and Service Analysis" width="100%">

### Page 5 – Regional & Package Cost Insights
<img src="screenshots/page5_regional_package_cost.png" alt="Regional and Package Cost Insights" width="100%">

---

## 🎯 Project Objectives

- Analyze overall delivery performance using key performance indicators.
- Measure the proportion of delayed and on-time deliveries.
- Compare delivery performance across partners and regions.
- Explore delivery costs across vehicles, delivery modes and package types.
- Understand customer satisfaction through delivery ratings.
- Identify patterns that may be associated with delivery delays.
- Present findings through an interactive, easy-to-understand dashboard.

## 🛠️ Tools & Technologies

| Tool | Purpose |
| --- | --- |
| Microsoft Excel | Data cleaning and preparation |
| Power Query | Data transformation |
| Power BI | Dashboard creation and visualization |
| DAX | Creating measures and KPIs |

---

## 🗂️ Dataset

- **Name:** Delivery Logistics Dataset (India – Multi-Partner)
- **Source:** [Kaggle – Delivery Logistics Dataset](https://www.kaggle.com/datasets/muhammadahmaddaar/delivery-logistics-dataset-india-multi-partner)
- **Records:** approximately 25,000 | **Columns:** 15 | **Format:** CSV
- **Domain:** Logistics and delivery operations

<details>
<summary><b>Click to view the key dataset fields</b></summary>

| Column | Description |
| --- | --- |
| `delivery_id` | Identifier associated with a delivery record |
| `delivery_partner` | Logistics partner handling the delivery |
| `package_type` | Category of the package |
| `vehicle_type` | Type of vehicle used |
| `delivery_mode` | Mode of delivery |
| `region` | Geographic region |
| `weather_condition` | Weather condition associated with the delivery |
| `distance_km` | Delivery distance in kilometres |
| `package_weight_kg` | Package weight in kilograms |
| `delivery_time_hours` | Recorded delivery time |
| `expected_time_hours` | Expected delivery time |
| `delayed` | Indicates whether a delivery was delayed |
| `delivery_status` | Delivery status |
| `delivery_rating` | Customer rating for the delivery |
| `delivery_cost` | Cost associated with the delivery |

</details>

---

## 🔄 Project Workflow

1. **Data Collection** – obtained the logistics dataset from Kaggle.
2. **Data Inspection** – reviewed structure, column names, data types and values.
3. **Data Preparation** – used Excel and Power Query to prepare the data.
4. **Data Validation** – examined quality, including repeated delivery identifiers.
5. **Data Modeling** – loaded the data into Power BI and organized the fields.
6. **DAX Measure Creation** – built ten measures for counts, rates, costs and ratings.
7. **Dashboard Development** – designed five report pages with KPI cards, charts and slicers.
8. **Performance Analysis** – compared delivery performance, costs and ratings across categories.
9. **Insight Development** – identified patterns and areas for further investigation.

---

## 📊 Dashboard Structure

| Page | Focus | KPIs | Main visuals |
| --- | --- | --- | --- |
| **1. Executive Overview** | High-level summary | Total Deliveries, Delayed Deliveries, Average Delivery Cost, Average Delivery Rating, Delay Rate | Delayed deliveries by partner, on-time vs delayed by region, delay rate by region |
| **2. Delivery Performance Analysis** | Where delays happen | Delay Rate, On-Time Rate, Delayed Deliveries, Average Delivery Rating | Delay rate by partner, region, weather and package type; donut of delivery status |
| **3. Cost & Operations Analysis** | What drives cost | Total Delivery Cost, Average Delivery Cost, Average Delivery Rating, Total Deliveries | Average cost by partner, delivery mode and vehicle type |
| **4. Customer & Service Analysis** | Ratings and service quality | Average Delivery Rating, Low Rating %, Delayed Deliveries, On-Time Rate | Rating by delay status, rating distribution, rating by partner, low rating % by region |
| **5. Regional & Package Cost Insights** | Cost by region and package | Total Deliveries, Total Delivery Cost, Delay Rate, Average Delivery Cost | Average cost by region and by package type |

---

## 🧮 DAX Measures

| Measure | Purpose |
| --- | --- |
| **Total Deliveries** | Counts delivery records |
| **Delayed Deliveries** | Counts records marked as delayed |
| **On-Time Deliveries** | Counts records marked as not delayed |
| **Delay Rate %** | Delayed deliveries as a percentage of total deliveries |
| **On-Time Rate %** | On-time deliveries as a percentage of total deliveries |
| **Average Delivery Cost** | Average delivery cost |
| **Total Delivery Cost** | Sum of delivery costs |
| **Average Delivery Rating** | Average customer rating |
| **Low Rating Deliveries** | Counts deliveries with a rating of 2 or below |
| **Low Rating %** | Low-rating deliveries as a percentage of total deliveries |

**Functions used:** `COUNTROWS()` · `CALCULATE()` · `DIVIDE()` · `AVERAGE()` · `SUM()`

## 📈 Charts & Visualizations

| Visualization | Analytical Purpose |
| --- | --- |
| Clustered Column Chart | Compares values across categories |
| Clustered Bar Chart | Compares average delivery cost across package types |
| Stacked Column Chart | Shows the composition of delivery counts |
| Donut Chart | Shows the distribution of a selected category |
| KPI Cards | Highlight important performance indicators |

## 🎚️ Interactive Slicers

| Slicer | Purpose |
| --- | --- |
| Delivery Partner | Focuses analysis on a selected logistics partner |
| Region | Filters results by geographic region |
| Weather Condition | Explores delivery performance under selected weather conditions |
| Delivery Mode | Compares results for selected delivery modes |
| Package Type | Filters delivery costs by package category |

> [!NOTE]
> The available slicers vary by report page. KPI cards and charts respond to applicable filter selections.

---

## 🔍 Key Findings

### 🚚 Delivery Performance
- Of 25,000 deliveries, 6,669 (26.7%) were marked delayed and 18,331 (73.3%) were on time. The delayed group includes about 5,340 late deliveries and 1,329 failed deliveries.
- Weather shows the widest gap in delay rates: stormy (41.4%) and rainy (37.4%) conditions are well above clear (17.4%), hot (17.1%) and cold (16.0%).
- Delay rates across partners are close together, from 24.8% (Delhivery) to 28.3% (XpressBees).
- Central has the highest regional delay rate (27.3%) and East the lowest (25.8%).

### 💰 Cost & Operations
- Total delivery cost is ₹21.62M, with an average of ₹864.94 per delivery.
- Delivery mode shows the largest cost difference: same-day (₹929.87) and express (₹880.43) cost more than two-day (₹829.71) and standard (₹819.34).
- Average cost differs only slightly by partner (₹848.11 to ₹872.83), vehicle type (₹857.66 to ₹869.24) and region (₹858.30 to ₹874.21).
- Clothing (₹879) and automobile parts (₹877) have the highest average cost by package type, and fragile items (₹847) the lowest.

### ⭐ Customer & Service
- The average rating is 3.67 out of 5, and 18.1% of deliveries have a low rating (2 or below).
- Deliveries not marked delayed average a rating of 4.2, compared with 2.2 for delayed deliveries.
- Average ratings are similar across partners (3.6 to 3.7).
- Central has the highest low-rating share (18.8%) and East the lowest (17.4%).

> [!IMPORTANT]
> These findings describe associations in the current dataset. Further analysis would be needed to establish the causes of delays, cost differences or rating patterns.

---

## 💼 Business Value

- Monitor delivery performance through key metrics.
- Compare delivery partners and geographic regions.
- Examine operational cost differences.
- Explore customer satisfaction patterns.
- Identify categories that may require further investigation.

## ⚠️ Limitations

- The dataset contains repeated delivery identifiers. Records sharing an identifier have different values in other fields, so they were treated as separate records and retained. The number of records should therefore not automatically be interpreted as the number of unique deliveries.
- The `delayed` field marks both late and failed deliveries as delayed, so Delayed Deliveries (6,669) and Delay Rate (26.7%) include the 1,329 failed deliveries shown separately in the delivery status chart.
- Some delivery-time fields had data-type consistency challenges during preparation and need further validation before detailed time-based analysis.
- Relationships observed in the dashboard do not necessarily indicate causation.
- Dataset sharing depends on permission to redistribute the source data.

## 🚀 Future Enhancements

- Investigate the causes of delivery delays in greater detail.
- Add validated delivery-time and expected-time analysis.
- Develop additional cost-efficiency indicators.
- Add time-based performance trends, if reliable date fields become available.
- Introduce predictive analytics for delivery-delay risk.

## 📁 Project Files

- 📊 [Presentation (PowerPoint)](presentation/Logistics_Delivery_Dashboard_with_Screenshots.pptx)
- 🖼️ [Dashboard screenshots](screenshots/)

---

## ✅ Conclusion

This project shows how Power BI, Power Query and DAX can turn logistics data into an interactive analytical report. By bringing delivery performance, operational costs and customer ratings together, it gives a structured way to explore logistics operations, and it demonstrates practical skills in data preparation, KPI development, data visualization and business analysis.

## 👤 Author

**Asmiya Farin S**
