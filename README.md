# 🚖 Uber Ride Operations & Revenue Intelligence Dashboard

---

## 🔥 Executive Business Insights

- 📈 Demand peaks during weekday rush hours (8–10 AM & 5–9 PM), indicating commute-driven ride behavior.
- ❌ Cancellation rates increase significantly when pickup time exceeds threshold levels, highlighting operational delays.
- 🚘 Go Mini contributes the highest booking volume but also the highest cancellation share.
- 💰 Revenue growth strongly correlates with ride completion rate.
- 📍 Pickup vs Drop analysis reveals demand concentration zones for supply optimization.
- 📊 Month-over-Month tracking shows performance volatility, stabilized using Rolling 3-Month smoothing.

---

## 📌 Project Overview

This project analyzes Uber ride booking data to uncover:

- Operational inefficiencies  
- Cancellation drivers  
- Revenue performance patterns  
- Time-series demand trends  
- Pickup vs Drop behavioral insights  

The dashboard is structured into four analytical layers from an executive decision-making perspective.

---

## 🧹 Data Engineering & Cleaning

### Power Query Transformations

- Null handling with business validation
- Booking-status logic enforcement
- Ratings restricted to completed rides
- Distance & revenue anomaly detection
- Feature engineering:
  - Peak vs Non-Peak classification
  - Weekday vs Weekend tagging
  - Booking hour extraction

---

## 🏗 Dimensional Data Modeling (Star Schema)

### ⭐ Fact Table
`Fact_Rides`
- Booking metrics
- Revenue
- Distance
- Operational flags
- Surrogate keys

### ⭐ Dimension Tables
- `Dim_Date`
- `Dim_Vehicle`
- `Dim_Location`
- `Dim_Payment`

### ⚡ Advanced Modeling Techniques

- Surrogate key implementation
- One-to-many single-direction relationships
- Dual-location modeling:
  - Pickup → Active relationship
  - Drop → Inactive relationship
- `USERELATIONSHIP()` for dynamic drop analysis
- Proper Date table for time intelligence

---

## 📊 KPIs Designed

- Total Bookings  
- Completed Rides  
- Completion Rate %  
- Cancellation Rate %  
- Total Revenue  
- Avg Booking Value  
- Revenue Loss due to Cancellations  
- Month-over-Month Growth %  
- Rolling 3-Month Average  
- Pickup vs Drop Demand Analysis  

---

# 📈 Dashboard Pages

---

## 1️⃣ Executive Overview

Provides high-level health metrics:

- KPI Cards
- MoM Growth %
- Revenue Trend
- Rolling performance smoothing

![Executive Overview](https://github.com/user-attachments/assets/0defeece-f8da-4e71-929b-7bff5ac1af8c)

---

## 2️⃣ Demand Analysis

Explores ride distribution patterns:

- Bookings by Hour
- Weekday vs Weekend comparison
- Vehicle Type demand segmentation
- Pickup Location concentration

![Demand Analysis](https://github.com/user-attachments/assets/6732871a-97bf-4ab2-a525-717186d8e594)

---

## 3️⃣ Cancellation Deep Dive

Identifies operational bottlenecks:

- Customer vs Driver cancellation patterns
- Cancellation rate by vehicle category
- Pickup delay vs cancellation correlation
- Location-level cancellation hotspots

<img width="867" height="491" alt="Cencellation_deep_dive" src="https://github.com/user-attachments/assets/b85fb80c-b7a2-44b4-88d9-6f8cbe3108d5" />

---

## 4️⃣ Revenue & Time-Series Analysis

Focuses on financial performance:

- Revenue by vehicle type
- MoM revenue growth %
- Rolling 3-Month smoothing
- Revenue vs Completion correlation

![Revenue & Time Series](https://github.com/user-attachments/assets/4c0b709d-0c1c-4e8c-b0de-b18fda8afee7)

---

## ⚙ Tools & Technologies Used

- Power BI Desktop
- Power Query (ETL)
- DAX (Advanced Time Intelligence & Context Control)
- Star Schema Modeling
- Git & GitHub

---

## 🚀 Advanced Features Implemented

- Dynamic KPI selector using disconnected tables
- Time intelligence with `DATEADD()` & `DATESINPERIOD()`
- Rolling averages for trend smoothing
- Conditional KPI formatting
- Dynamic insight text generation
- Active/Inactive relationship modeling
- Context switching using `USERELATIONSHIP()`

---

## 🧠 Analytical Capabilities Demonstrated

✔ Business logic validation  
✔ Data modeling expertise  
✔ Advanced DAX proficiency  
✔ Time-series analysis  
✔ Operational analytics  
✔ Executive storytelling  
✔ Dashboard UX optimization  

---

## 🎯 Business Value Delivered

This dashboard enables stakeholders to:

- Identify cancellation drivers
- Improve operational efficiency
- Optimize vehicle distribution
- Monitor revenue health
- Track performance momentum
- Support data-driven decisions

---

## 📌 Future Enhancements

- Predictive cancellation modeling
- Demand forecasting
- Driver performance scoring
- Location-based supply optimization
- Benchmark comparisons

---

## 👨‍💻 Author

**Adithya G**  
Data Analyst | Business Intelligence Enthusiast  
Power BI | DAX | Data Modeling | Analytics Engineering  

---
