🚖 Uber Ride Operations & Revenue Intelligence Dashboard
🔥 Key Business Insights (Executive Summary)

📈 Demand peaks during weekday rush hours (8–10 AM & 5–9 PM), indicating commute-driven ride behavior.

❌ Cancellation rates increase significantly when pickup time exceeds threshold levels, suggesting operational delay impact.

🚘 Go Mini contributes highest booking volume but also the highest cancellation share, highlighting vehicle-category imbalance.

💰 Revenue growth correlates strongly with completion rate, indicating that reducing cancellations directly improves profitability.

📍 Pickup vs Drop analysis reveals demand concentration in specific zones, enabling supply reallocation strategies.

📊 Month-over-Month tracking shows clear performance volatility, addressed using Rolling 3-Month smoothing for stability.

📌 Project Overview

This project analyzes Uber ride booking data to uncover:

Operational inefficiencies

Cancellation drivers

Revenue performance patterns

Time-series demand trends

Pickup vs Drop behavioral insights

The dashboard is designed from an executive decision-making perspective, structured into four analytical layers.

🧹 Data Engineering & Modeling Approach
🔍 Data Cleaning (Power Query)

Null handling with business-rule validation

Booking-status logic enforcement

Ratings restricted to completed rides

Distance and revenue anomaly validation

Feature engineering:

Peak / Non-Peak classification

Weekday vs Weekend tagging

Booking Hour extraction

Business-consistent transformation pipeline

🏗 Dimensional Modeling (Star Schema)

The flat transactional dataset was transformed into a scalable star schema:

🔹 Fact Table

Fact_Rides

Booking metrics

Revenue

Distance

Operational flags

Surrogate keys

🔹 Dimension Tables

Dim_Date

Dim_Vehicle

Dim_Location

Dim_Payment

⚡ Advanced Modeling Implemented

Surrogate key creation

One-to-many single-direction relationships

Dual-location modeling (Pickup = Active, Drop = Inactive)

USERELATIONSHIP() for dynamic drop-location analysis

Proper Date table with time intelligence support

📊 KPIs Designed

Total Bookings

Completed Rides

Completion Rate %

Cancellation Rate %

Total Revenue

Avg Booking Value

Revenue Loss due to Cancellations

Month-over-Month Growth %

Rolling 3-Month Average

Pickup vs Drop Demand Analysis

📈 Dashboard Structure
1️⃣ Executive Overview

Provides high-level health metrics:

KPI Cards

MoM Growth %

Revenue Trend

Rolling performance smoothing

<img width="772" height="432" alt="Executive_overview" src="https://github.com/user-attachments/assets/82d66329-6e53-4f69-9338-b1932189c627" />


2️⃣ Demand Analysis

Explores ride distribution patterns:

Bookings by Hour

Weekday vs Weekend comparison

Vehicle Type demand segmentation

Pickup Location concentration

<img width="769" height="434" alt="demand_analysis" src="https://github.com/user-attachments/assets/99b3685d-d084-487e-9299-c3c8d251e62e" />


3️⃣ Cancellation Deep Dive

Identifies operational bottlenecks:

Customer vs Driver cancellation patterns

Cancellation rate by vehicle category

Pickup delay vs cancellation correlation

Location-level cancellation hotspots

<img width="867" height="491" alt="Cencellation_deep_dive" src="https://github.com/user-attachments/assets/53522d4c-080b-461b-a8bd-df2b64ab143d" />


4️⃣ Revenue & Time-Series Analysis

Focuses on financial performance:

Revenue by vehicle type

MoM revenue growth %

Rolling 3-Month smoothing

Revenue vs Completion correlation

<img width="768" height="434" alt="Revenue_and_ratings" src="https://github.com/user-attachments/assets/323e1d83-d98a-4736-bb5c-d22066a7b3df" />

⚙ Tools & Technologies Used

Power BI Desktop

Power Query (ETL & Data Cleaning)

DAX (Advanced Time Intelligence & Context Control)

Star Schema Modeling

Git / GitHub (Version Control)

🚀 Advanced Features Implemented

Dynamic KPI selector using disconnected tables

Time intelligence with DATEADD() & DATESINPERIOD()

Rolling averages for trend smoothing

Conditional formatting for KPI signals

Dynamic insight text generation

Active/Inactive relationship modeling

Context switching using USERELATIONSHIP()

🧠 Analytical Capabilities Demonstrated

✔ Business logic validation
✔ Data modeling expertise
✔ Advanced DAX proficiency
✔ Time-series analysis
✔ Operational analytics
✔ Executive storytelling
✔ Dashboard UX optimization

🎯 Business Value

This dashboard enables stakeholders to:

Identify cancellation drivers

Improve operational efficiency

Optimize vehicle distribution

Monitor revenue health

Track performance momentum

Support data-driven strategic decisions

📌 Future Enhancements

Predictive cancellation modeling

Demand forecasting (ARIMA / Prophet)

Driver performance scoring

Location-based supply optimization

Dynamic benchmark comparisons

👨‍💻 Author

Adithya G
Data Analyst | Business Intelligence Enthusiast
Power BI | DAX | Data Modeling | Analytics Engineering

