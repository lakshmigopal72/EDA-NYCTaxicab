# EDA-NYCTaxicab
EDA of NYC taxi cab. This is the Exploratory Data Analysis of the New York Taxi cabs dataset that I worked on as part of the Executive Diploma in Data Science and AI course

# NYC Taxi Trips – Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project presents a comprehensive **Exploratory Data Analysis (EDA)** of NYC taxi trip data to uncover **temporal, spatial, financial, and behavioral patterns** in urban mobility.  
The analysis focuses on understanding **demand trends, fare dynamics, tipping behavior, congestion patterns, and zone-level activity** to derive actionable insights for **routing, dispatching, and pricing optimization**.
---

## 📂 Dataset Description
The dataset contains detailed taxi trip records including:
- Pickup and drop-off timestamps
- Trip distance and duration
- Fare components and surcharges
- Tip amounts and payment types
- Passenger count
- Pickup and drop-off location IDs

A NYC Taxi **zones shapefile** is used to enable spatial analysis and mapping.

---

## 🧹 Data Preparation & Cleaning
Key preprocessing steps included:
- Handling missing values and inconsistent columns (e.g., duplicate airport fee fields)
- Flagging and removing invalid trips (negative fares, zero-duration trips, unrealistic distances)
- Separating **invalid**, **extreme**, and **valid but rare** observations using flags
- Creating derived features such as:
  - Trip duration (minutes)
  - Hour of day, day of week, and time-of-day buckets
  - Fare per mile and tip percentage
- Sampling data uniformly across hours and scaling results appropriately

---

## 📊 Exploratory Analysis Highlights

### ⏰ Temporal Patterns
- Peak demand occurs during **weekday afternoons and evenings**
- Weekends show **flatter demand curves** with higher late-night activity
- Seasonal patterns indicate higher demand and revenue during **spring and autumn**

### 💰 Fare & Revenue Insights
- Fare is **strongly correlated with trip distance** and moderately with trip duration
- Passenger count has minimal influence on fare
- Revenue is evenly distributed across quarters, with **Q2 and Q4 slightly higher**
- Daytime trips contribute most revenue, while nighttime trips yield **higher revenue per trip**

### 💸 Tipping Behavior
- Tip percentage varies widely and depends strongly on **payment method**
- Credit card trips consistently show higher recorded tip percentages
- Low tips are common for:
  - Short trips
  - Cash payments
  - Late-night or group travel
- High tips are associated with longer trips, card payments, and daytime travel

### 🚕 Distance-Tier & Vendor Comparison
- Fare per mile is highest for trips under 2 miles due to base fare effects
- Vendor differences are most visible for short trips and converge for longer distances
- Cost per passenger per mile decreases as passenger count increases

---

## 🗺️ Spatial & Zone-Level Analysis
- Central business districts, airports, and tourist areas are the **busiest pickup zones**
- Nighttime pickup and drop-off zones differ significantly from daytime hotspots
- Pickup/drop-off ratios highlight **origin-heavy and destination-heavy zones**
- Average passenger count varies spatially, with higher occupancy near airports and leisure zones
- Choropleth maps visualize:
  - Trip volumes
  - Average passenger count
  - Zone-level demand intensity

---

## 🚦 Congestion & Route Efficiency
- Slow routes are identified using **average speed by zone pair and hour**
- Peak congestion occurs during commute hours and in dense urban zones
- Nighttime routes generally have higher speeds despite lower volumes

---

## 💡 Key Recommendations
- Time-aware and zone-based cab positioning
- Congestion-aware routing during peak hours
- Dynamic dispatch using pickup/drop-off imbalance
- Distance-tiered and time-sensitive pricing adjustments
- Incentivizing card payments to improve effective revenue
- Matching vehicle size to zones with higher passenger occupancy

---

## 🛠️ Tools & Libraries Used
- **Python** (Pandas, NumPy)
- **Matplotlib / Seaborn** for visualization
- **GeoPandas** for spatial analysis
- **Jupyter Notebook** for analysis workflow

---

## 📈 Outcomes
This EDA provides a **data-driven understanding of urban taxi operations**, offering insights that can support:
- Smarter dispatch and routing decisions
- Revenue-optimized yet competitive pricing strategies
- Improved service availability and utilization

---

## 📌 Future Work
- Predictive demand modeling
- Event-based surge analysis
- Integration with real-time traffic data
- Driver-level performance analysis

---

## ✍️ Author
This project was developed as part of an **Exploratory Data Analysis assignment** focusing on real-world urban mobility data and operational insights.

---

⭐ *If you find this project useful, feel free to star the repository!*

