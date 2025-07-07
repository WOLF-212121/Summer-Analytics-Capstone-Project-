🚗 Urban Parking Lots – Real-Time Dynamic Pricing System

Welcome to the repository for our Capstone Project under Summer Analytics. This project focuses on developing a real-time dynamic pricing system for urban parking lots.

📌 Project Overview
In densely populated urban areas, managing parking demand efficiently is crucial. Our system aims to monitor and predict real-time parking lot prices using factors such as occupancy, capacity, and other demand-related variables.
By implementing dynamic pricing, urban parking can be optimized to:
1. Reduce congestion
2. Improve space utilization
3. Offer fair and data-driven pricing for users

🛠️ Libraries & Tools
* Pandas
* Numpy
* Matplotlib
* Bokeh (for real-time visualization)
* Pathway (for real-time data streaming and windowing)

⚙️ Model Architectures
📈 Model 1: Baseline Linear Pricing
1. Base Price: Fixed at $10
2. Approach: Baseline linear model
3. Price Calculation:
 Price = Base Price + (Max Occupancy - Min Occupancy) / Max Capacity
 Calculated for each day individually.
4. Visualization: Real-time data streaming and plotting using Bokeh.

📊 Model 2: Demand-Based Dynamic Pricing
1. Enhanced Factors: Incorporates additional variables to calculate parking demand:
* Occupancy
* Capacity
* Queue Length
* Nearby Traffic Conditions
* Special Days
* Vehicle Type
2. Demand Calculations -
  Demand = ((Max Occupancy - Min Occupancy) / Max Capacity)
         + Queue Length
         - Traffic Condition Nearby
         + Is Special Day
         + Vehicle Type
3. Price Calculation -
  Price = Base Price × (1 + Demand)
4. Visualization: Real-time demand and pricing streamed and visualized with Bokeh.

🔄 Workflow
1. Data Extraction: Ingest raw parking lot data.
2. Schema Definition: Create structured schema tables for clean ingestion.
3. Real-Time Variables: Stream real-time data streams using the defined schema.
4. Time Windowing: Use timestamps to track and analyze data in daily windows.
5. Price Prediction: Compute real-time prices using the above models.
6. Visualization: Plot dynamic pricing outputs with interactive Bokeh dashboards.
  

✅ Key Outcomes
1. A working prototype for real-time parking price prediction.
2. Flexible architecture to extend pricing logic with more features.
3. Live visual dashboards to monitor price fluctuations and parking demand.

