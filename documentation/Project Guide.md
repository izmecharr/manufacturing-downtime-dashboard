##Soda Manufacturing Line Downtime Dashboard - Power BI Project Guide
- Shows the thought process of the developer/analyst while creating the Manufacturing Downtime and Efficiency Dashboard. 

1. Who is the audience of the Business Intelligence Dashboard
- 

2. What is the business goal/s?
- 

3. What are the metrics and level of detail inline with business goal/s?
Metric
Level of Detail

4. Set Prototype layout
- Don't care about the design, just what metrics are necessary to be shown. 

Dashboard Architecture for Beverage Manufacturing

Page 1: Production Performance Overview
Target Audience: Plant Manager & Production Supervisors
1. Gauge Chart: Overall Line Efficiency (Current: ~56%, Target: 85%)

2. KPI Cards:
- Total Batches Produced (38)
- Average Batch Efficiency (56.2%)
- Total Downtime Hours (Calculate from your data)
- Estimated Weekly Loss (₱XXX,XXX)

3. Donut Chart: Production Mix by Product
- LE-600 (Lemon Lime): Most produced
- Product efficiency comparison

4. Column Chart: Daily Production Efficiency Trend
- Show efficiency by production date
- Highlight best vs worst days

Page 2: Downtime Root Cause Analysis
Target Audience: Maintenance Team & Quality Managers
1. Pareto Chart: Downtime Factors by Impact
- Based on your data: Factor 2 (Batch change), Factor 3 (Labeling error), Factor 7 (Machine failure)
- Show cumulative percentage line

2. Treemap: Downtime Categories Sized by Minutes Lost
- Color code by Operator Error (Yes/No)

3. Heat Map: Downtime by Product Type × Factor
- Identify if certain products have specific issues

4. Waterfall Chart: Perfect Batch Time vs Actual Time Breakdown
- Start with min batch time (60/98 minutes)
- Add each downtime factor
- Show total actual time

Page 3: Operator Performance Analysis
Target Audience: Production Supervisors & HR
1. Bar Chart: Operator Efficiency Comparison
- Mac vs Maiza vs Rita performance
- Include confidence intervals based on batch count

2. Scatter Plot: Operator Experience vs Efficiency
- X-axis: Number of batches handled
- Y-axis: Average efficiency
- Size: Total downtime minutes

3. Matrix Table: Operator × Downtime Factor Analysis
- Show which operators struggle with specific issues

Page 4: Product-Specific Deep Dive
Target Audience: Process Engineers & Quality Team

1. Clustered Column Chart: Efficiency by Product Type
- 600ml vs 2L comparison
- Flavor-specific performance

2. Line Chart: Product Efficiency Trends Over Time
- Track if specific products improve/decline

3. Funnel Chart: Perfect Batch → Actual Performance
- Show efficiency loss stages

5. Clean Up cluttered and unnecessary data
- This is when we start to care about the design, color, text etc. of the Dashboard

6. Make the visuals intuitive and clear
- Rethink and restructure if the specified audience can read the dashboard.

7. Tell a story
- make the title of graphs more like telling a story 
- Add insights and recommendations

8. Increase interactivity and detail