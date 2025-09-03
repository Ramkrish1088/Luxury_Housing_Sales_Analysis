**🏙️ Luxury Housing Sales Analysis — Bengaluru**
-------------------------------------------------

**📊 Project Overview**
------------------------

  This end-to-end analytics project explores luxury housing sales trends in Bengaluru using Python, MySQL, and Power BI. It focuses on understanding market dynamics, builder performance, buyer preferences, and sales channel effectiveness through advanced data transformation and visualization.

**🎯 Objective**
-----------------

Analyze luxury property transactions in Bengaluru to uncover actionable insights across:

    📈Market Trends
    
    🏗️Builder Performance
    
    📉Booking Conversion Rates
    
    🧍‍♂️🧍‍♀️Buyer Behavior
    
    📢Sales Channel Efficience

**🔧 Step 1: Python — Data Cleaning & Feature Engineering**
-------------------------------------------------------------
✅ Tasks:

  Load raw CSV data of luxury property transactions.
  
  Clean and normalize:

    1.Standardize Ticket_Price_Cr (e.g., ₹3.5 Cr → 3.5)
    
    2.Handle nulls in Amenity_Score, Booking_Status, etc.
    
    3.Normalize categorical fields (Builder, Micro_Market, Sales_Channel)

  Derive new features:

    1.Price_per_Sqft
    
    2.Quarter_Number (from transaction date)
    
    3.Booking_Flag (1 for Booked, 0 for Available)
    
**🧠 Step 2: SQL — Load Clean Data into RDBMS**
-------------------------------------------------

🗃️ Tasks:

    1.Design SQL table schema for property_transactions.
    
    2.Load cleaned CSV into MySQL database using SQLAlchemy.

**📊 Step 3: Power BI — Interactive Dashboard**
-------------------------------------------------

🔌 Connection:

    1.Power BI connected directly to MySQL for live querying.

**📈 Visualizations:**
-----------------------
| **Insight Area**                | **Visualization Type**     | **Description**                                                                 |
|--------------------------------|-----------------------------|---------------------------------------------------------------------------------|
| Market Trends                  | Line Chart                  | Bookings over time segmented by `Micro_Market`                                 |
| Builder Performance            | Bar Chart / Table           | Sum and Avg of `Ticket_Price_Cr` by `Builder`                                  |
| Amenity Impact                 | Scatter Plot                | `Amenity_Score` vs `Booking_Conversion_Rate`, bubble size = project count      |
| Booking Conversion             | Stacked Column Chart        | % `Booking_Status` by `Micro_Market`                                           |
| Configuration Demand           | Donut Chart                 | Most in-demand configurations (e.g., 3BHK, 4BHK)                                |
| Sales Channel Efficiency       | 100% Stacked Chart          | Distribution of `Booking_Status` across `Sales_Channels`                       |
| Quarterly Builder Contribution | Matrix Table                | `Builder`-wise sales contribution per `Quarter`                                |
| Possession Status Analysis     | Clustered Column Chart      | Relationship between `Possession_Status`, `Buyer_Type`, and booking decisions  |
| Geographical Insights          | Map Visualization           | Concentration of luxury housing by `Micro_Market` or geographic coordinates     |
| Top Performers                 | KPI Cards / Drill-through   | Top 5 builders by revenue and booking success with drill-through to projects   |

**👨‍💻 Author**
--------------
**Muthuramakrishnan R**
