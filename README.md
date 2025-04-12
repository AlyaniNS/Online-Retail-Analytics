# Online Sales Analytics
**Analyzing sales data to drive strategic decisions for an online retail store.**

This project analyzes sales data from an online retail store to support strategic decision-making for the CEO and CMO. It involves data cleaning in Python and dashboard development in Tableau to uncover actionable insights.

## Tools Used
- Jupyter Notebook: Data processing & exploration using Python
- Tableau: Data visualization and dashboard creation

## Business Scenario
The dataset, titled Online Retail Dataset, was provided to address critical business questions from the CEO and CMO.
**Key Question by Role**
|Question|Focus Area|
|--------|----------|
|What are the top-performing products based on revenue, and how can we optimize inventory to maximize sales?| CEO|
|Which countries generate the highest revenue, and should we consider expanding to new markets?|CEO|
|What are the key sales trends over time, and how should we adjust our business strategy accordingly?|CEO|
|How many repeat customers do we have, and what strategies can increase customer retention?|CEO|
|Which product categories or specific products have the highest return on investment (ROI) from marketing campaigns?|CMO|
|Which customer segments have the highest lifetime value, and how can we target them more effectively?|CMO|
|Are there patterns in customer purchasing behavior that indicate potential for cross-selling or bundling strategies?|CMO|
|What are the key factors influencing cart abandonment, and how can we optimize our marketing funnel to reduce drop-offs?|CMO|

## Project Background
The CEO and CMO are seeking insights to support expansion plans and improve business performance. They expect an analysis of revenue trends, customer behavior, and product performance to guide decision-making.
### **Key deliverables:**
- Cleaned dataset for reliability
- Interactive Tableau dashboard for exploration
- Actionable insights to drive strategic actions

## Data Overview
### Raw Data
- Size: 541,909 rows × 8 columns
- Columns:
`InvoiceNo`, `StockCode`, `Description`, `Quantity`, `InvoiceDate`, `UnitPrice`, `CustomerID`, `Country`
### Data Cleaning Process
- Removed rows with Quantity <= 1 and UnitPrice < 0.
- Dropped rows with missing `CustomerID`.
- Standardized country names (renamed "EIRE" to Ireland, "RSA" to South Africa).
- Converted `InvoiceDate` to datetime format.
- Extracted `Year`, `Month`, and `YearMonth` for time-based analysis.
### Final Dataset
- Size: 397,884 rows × 12 columns
- New Columns:
    - `Revenue` = Quantity × UnitPrice 
    - `Year`, `Month`, `YearMonth` (derived from `InvoiceDate`)

## Data Visualization
Interactive Tableau dashboards were created to explore:
1. Monthly Revenue Trend (2011)
   ![Monthly Revenue Trend (2011)](https://github.com/AlyaniNS/Online-Retail-Analytics/blob/main/assets/monthly-revenue-trend.png)
   **Goal: Identify seasonality patterns.**
   
2. Top 10 Countries by Revenue (Excluding UK)
   ![Top 10 Countries by Revenue](https://github.com/AlyaniNS/Online-Retail-Analytics/blob/main/assets/top-countries-revenue.png)
   **Goal: Prioritize international market expansion.**
   
3. Top 10 Customers by Revenue
   ![Top 10 Customers by Revenue](https://github.com/AlyaniNS/Online-Retail-Analytics/blob/main/assets/top-countries-revenue.png)
   **Goal: Target high-value customers**
   
4. Top Countries by Demand
   ![Top Countries by Demand](https://github.com/AlyaniNS/Online-Retail-Analytics/blob/main/assets/top-countries-demand.png)
    **Goal: Understand regional purchasing behavior.**

5. New vs Repeat Customers
   ![New vs Repeat Customers](https://github.com/AlyaniNS/Online-Retail-Analytics/blob/main/assets/repeat-vs-new-customers.png)
   **Goal: Measure customer loyalty.**

6. Top-Selling Products
   ![Top-Selling Products](https://github.com/AlyaniNS/Online-Retail-Analytics/blob/main/assets/top-products-by-revenue.png)
   **Goal: Optimize inventory and marketing focus.**

## Key Insights
1. Seasonal Sales Trends (2011)
    - Revenue peaks in November and December (holiday season).
    - Weakest months: January and February (opportunity for promotions).
2. Top Revenue-Generating Countries (Exclude UK)
    - Netherlands, Ireland, and Germany lead in revenue.
    - High sales volume but low revenue in some markets suggests demand for lower-priced goods.
3. Top 10 Customers by Revenue
    - A small group of customers drives ~25% of total revenue (exact percentage from your analysis).
    - Recommendation: Launch loyalty programs and personalized offers.
4. Regional Demand
    - Western Europe (Netherlands, Ireland, Germany) shows strong demand.
    - Mid-tier markets may benefit from localized campaigns.
5. Customer Retention
    - Repeat customers generate 3× more revenue during peak months.
    - Recommendation: Invest in email campaigns and VIP benefits.
6. Top-Selling Products
    - Home decor, kitchenware, and storage dominate sales.
    - Opportunity: Bundle products or feature them in promotions.

## Future Recommendations
- Customer Lifetime Value (CLV) Analysis: Identify high-value segments.
- Cart Abandonment Study: Requires additional behavioral data.
- Regional Pricing Strategy: Test pricing adjustments in mid-tier markets.

## Conclusion
This analysis highlights actionable strategies to improve the online retail store’s performance:
- Inventory planning for seasonal peaks.
- Expand into high-demand markets (Netherlands, Ireland, Germany).
- Retain high-value customers with loyalty programs.
- Promote top-selling products through bundling.
- Further analysis of CLV and cart abandonment will enhance marketing ROI.

## Acknowledgments
This project is part of a self-paced job simulation from [The Forage](https://www.theforage.com/simulations/tata/data-visualisation-p5xo) titled Data Visualisation: Empowering Business with Effective Insights by Tata Group.
