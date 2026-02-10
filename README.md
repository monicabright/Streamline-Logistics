# STREAMLINE LOGISTICS ORDER FULFILMENT
### Real-Time Insight Into Delivery Performance and Customer Satisfaction

## Project Background

This report outlines the findings and operational strategies for Streamline Logistics Solutions, a logistics provider with over two decades of experience in nationwide delivery. The business relies on high-volume, dependable logistics; however, recent operational challenges; mounting order backlogs and rising expenses triggered a need for a data-driven review of the fulfillment process.
This project was executed entirely within Microsoft Excel. The raw dataset was cleaned, normalized, and analyzed using Pivot Tables. The final output is an interactive Excel dashboard consisting of two primary views: Order Fulfillment and Resource Allocation.

### Insights and recommendations focus on these key areas:
- **Category 1:** Delivery Performance & Delay Analysis
- **Category 2:** Resource & Driver Efficiency
- **Category 3:** Demand Patterns & Peak Hour Stress
- **Category 4:** Geographic & Routing Bottlenecks

### Data Structure & Initial Checks
The analysis was performed on a single comprehensive dataset containing 1,500 records. This table includes fields for Order IDs, timestamps, delivery zones, driver assignments, vehicle information, and customer feedback.
To ensure accuracy, the data underwent a cleaning process to handle missing timestamps and standardize duration metrics (measured in minutes). Although stored in a single table, the data was organized logically to allow for the multi-page dashboard reporting.

## Executive Summary
### Overview of Findings
The fulfillment process is currently under significant strain, with 80.3% of orders experiencing delays and 33.3% categorized as backlogged. Analysis shows that the 10:00 AM peak hour is a critical breaking point where order volume outpaces driver availability. Furthermore, the operational underperformance of "Van A" and the inefficient use of "Expedited" rules are primary contributors to the current 32.07% customer satisfaction score.
![](https://github.com/monicabright/AfriTech-Electronics/blob/main/Customer%20Analysis%20Afritech.png)

## Insights Deep Dive
### Category 1: Order Fulfillment
- **Systemic Delays:** The data confirms that 80.33% of orders are delayed by more than 5 minutes. This is not isolated to a single region but is a broad operational failure that directly impacts the bottom line.
- **The Backlog Reality:** One-third of all orders (33.33%) are currently backlogged. These are defined as orders still in progress with a delay exceeding 10 minutes, creating a "clog" in the system that impacts subsequent delivery windows.
- **Customer Sentiment Correlation:** There is a sharp drop in satisfaction once delays exceed the 5-minute mark. The current CSAT of 32.07% suggests that the majority of the customer base is dissatisfied with the current speed of service.
[Visualization: Order Status Breakdown & Delay Duration vs. Satisfaction]
### Category 2: Resource Allocation
- **Van A Bottleneck:** Van A is responsible for 35% of all deliveries, yet it is the single largest source of delays. This vehicle is either over-assigned or being used for routes that are inherently inefficient.
- **Driver Performance Variance:** Pivot Table analysis identified specific high-performing drivers (D10, D85) who maintain significantly lower delay rates. Conversely, a large portion of the driver pool is struggling with standard delivery timelines.
- **Expedited Rule Misuse:** The "Expedited" allocation rule is used for 32% of orders but fails to actually reduce delivery times. This indicates that the rule is being applied to too many orders, effectively neutralizing its priority status.
[Visualization: Driver Delay Rankings & Vehicle Utilization Rates]
### Category 3: Demand Patterns & Timing
- **Peak Hour Pressure:** The 10:00 AM window sees the highest influx of orders. The current resource allocation is static and does not account for this surge, leading to the daily accumulation of backlogs.
- **Average Throughput:** With an average delivery time of 73.56 minutes, the operation cannot clear the 10:00 AM peak before the afternoon orders begin to arrive.
[Visualization: Hourly Order Volume vs. Delay Minutes]
### Category 4: Geographic & Routing Issues
- **Zone 1 & CityB Hotspots:** These areas consistently report the highest number of delayed orders. The data suggests that systemic issues—such as heavy traffic or difficult delivery locations—are not being factored into the current route planning.
- **Visibility Gaps:** Analysis of customer feedback reveals that a lack of real-time updates during these geographic delays is a major driver of "Negative" ratings.
[Visualization: Map of Delay Density by Delivery Zone]

## Recommendations
Based on the Excel analysis, the following actions are suggested for the Operations and Logistics Team:
- **Balance the Fleet:** Shift 15-25% of Van A’s current workload to other underutilized vehicles to reduce the primary bottleneck.
- **Address the 10:00 AM Surge:** Adjust driver shift starts to ensure maximum personnel are active 30 minutes prior to the 10:00 AM peak.
- **Audit Allocation Rules:** Tighten the criteria for "Expedited" deliveries. By reducing the volume of expedited orders, the team can ensure that high-priority shipments actually receive priority handling.
- **Optimize Zone 1 Routes:** Conduct a specific route review for CityB/Zone 1. Testing smaller delivery windows or alternative routes in these areas may bypass consistent traffic hurdles.
- **Improve Communication:** Implement a standard practice of notifying customers as soon as an order enters the "Delayed" category (>5 mins) to manage expectations and improve satisfaction.

## Assumptions and Caveats
- **Delay Classification:** Any order exceeding its scheduled time by more than 5 minutes was flagged as "Delayed."
- **Backlog Classification:** "Backlog" was defined as any order still "In Progress" with a delay of more than 10 minutes.
- **Data Consistency:** The analysis assumes that the 1,500 records provided are a representative sample of daily operations across all regions.
