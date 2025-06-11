##Soda Manufacturing Line Downtime Dashboard - Power BI Project Guide
- Shows the thought process of the developer/analyst while creating the Manufacturing Downtime and Efficiency Dashboard.
  
1. What are the data available in the dataset?
   
Line productivity (Fact Table) - 38 records
├── Date: Production dates
├── Product: Product IDs (OR-600, LE-600, CO-600, DC-600, RB-600, CO-2L)
├── Batch: Unique batch IDs (422111-422148)
├── Operator: 4 operators (Mac, Charlie, Dee, Dennis)
├── Start Time: Batch start timestamps
└── End Time: Batch completion timestamps

Products (Dimension Table) - 6 products
├── Product: Product IDs
├── Flavor: Orange, Lemon lime, Cola, Diet Cola, Root Beer
├── Size: 600 ml, 2 L
└── Min batch time: Target times (60 min for 600ml, 98 min for 2L)

Line downtime (Fact Table) - 38 batch records
├── Batch: Links to Line productivity
└── Downtime factors 1-12: Minutes lost per factor per batch

Downtime factors (Dimension Table) - 12 factors
├── Factor: IDs 1-12
├── Description: Specific downtime causes
└── Operator Error: Yes/No classification (6 Yes, 6 No)

2. Who is the audience of the Business Intelligence Dashboard
Executive Level:
├── Plant Manager: Overall efficiency, cost impact, strategic decisions
└── Operations Director: Resource allocation, capacity planning

Management Level:
├── Production Supervisors: Daily operations, operator management
├── Quality Manager: Process improvement, error reduction
└── Maintenance Manager: Equipment reliability, downtime reduction

Operational Level:
├── Shift Supervisors: Real-time production monitoring
├── Process Engineers: Technical optimization, process design
└── HR Managers: Training needs, performance management

3. What is the business goal/s?
Operational Excellence:
- Improve Overall Equipment Effectiveness (OEE) from current 70.4% to target 85%
- Reduce average batch time from 85 minutes to 60-minute target
- Minimize production downtime and eliminate inefficiencies

Cost Optimization:
- Reduce production costs by eliminating 25-minute excess time per batch
- Minimize waste from operator errors and equipment failures
- Optimize resource utilization across operators and products

Quality & Consistency:
- Standardize performance across all operators to best-performer level
- Reduce variability in batch times and product quality
- Eliminate operator-related errors through targeted training

Strategic Growth:
- Maximize production capacity with existing resources
- Enable data-driven decision making for future investments
- Build foundation for scalable operations

4. What are the metrics and level of detail inline with business goal/s?
Metric
Level of Detail

5. Set Prototype layout
- Don't care about the design, just what metrics are necessary to be shown. 

6. Clean Up cluttered and unnecessary data
- This is when we start to care about the design, color, text etc. of the Dashboard

7. Make the visuals intuitive and clear
- Rethink and restructure if the specified audience can read the dashboard.

8. Tell a story
- make the title of graphs more like telling a story 
- Add insights and recommendations

9. Increase interactivity and detail
