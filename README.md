# Citibike-Data-Viz-and-Insights
Tableau project analyzing Citi Bike usage in NYC. Built three dashboards on rider demographics, daily system utilization, and station geography, using September 2024 trip data. Highlights member dominance, commute peaks, and key pick-up/drop-off hotspots to guide operations and rebalancing and suggests rebalancing tactics by time of day for users.


# CSV Files
https://drive.google.com/drive/folders/1NhBgnlArKS2kISV44Cl-JOexjGWTcllE?usp=sharing

# Skills & Techniques Used
## Data preparation & modelling
- Combined five monthly Citi Bike CSVs into a single dataset using a table union in Tableau.
- Set correct data types and geographic roles (dates, datetimes, latitude/longitude).
- Built a clean data model that supports ridership, utilization, and geographic views from the same source.
## Calculated fields & time-based features
- Created custom measures such as Trip Duration (minutes) using DATEDIFF.
- Derived Day of Week and Hour of Day using DATENAME and DATEPART for temporal analysis.
## Dashboard interactivity
- Created a parameter (Station View) and parameter-driven calculated fields (Selected Lat/Lng/Station Name) to toggle a single map and bar chart between Pick-Up and Drop-Off views.
- Used filters as slicers (Day of Week, Rider Type, Bike Type, Time of Day) and applied them across multiple worksheets to make the dashboards interactive.
- Customized tooltips to show relevant context (hour, rider type, bike type, station name, trip count).
## Visualization & analysis
- Built a variety of charts: pie charts, bar charts, line charts, heatmaps, and KPI-style summary views.
- Analyzed ridership composition (members vs casuals, classic vs electric), average trip duration by rider type and day of week, and hourly utilization patterns across weekdays vs weekends.
- Designed geospatial maps of station-level demand using sized/colored circles to highlight key pick-up and drop-off hotspots.
## Storytelling & recommendations
- Synthesized findings from all three dashboards into operational recommendations for Citi Bike (e.g., when and where to rebalance bikes, how to serve members vs casuals, and how to position e-bikes during peak hours).

# Operational Insight
Citi Bike should use low-demand hours (roughly 10–3 PM on weekdays) to relocate bikes from stations that consistently see high drop-off volumes to those with high pick-up demand. This ensures that more bikes are available at popular origin stations heading into the evening peak (≈5–8 PM). By repeating this rebalancing cycle daily (shifting bikes from sink stations (net receivers) to source stations (net exporters) during midday lulls) the system can reduce stockouts at busy locations and encourage more riders to use the service during peak periods. 

They should also refine their pricing strategy for casual riders to encourage more frequent use and nudge them toward membership. For example, by offering discounted multi-ride passes, off-peak pricing, or targeted promotions that make the system more attractive and cost-effective for non-members.

