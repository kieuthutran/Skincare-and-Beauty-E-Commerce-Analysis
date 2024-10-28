# **1. Overview**
The skincare and beauty e-commerce market are thriving and evolving rapidly. We have collected so much data, and now we are interested in gaining more insights about the market, product, customers and sales etc.

# **2. Tools and Technologies**
   - Microsoft Power BI
   - Global skincare and beauty e-store dataset

|Column | Dictionary|
|---|----------------|
|Row ID | Unique ID of the row|
|Order ID | ID of the order (one order can have multiple items)|
|Order Date | Date when order was made|
|Customer ID | ID of the customer (one customer can make multiple orders)|
|Segment | Customer segment |
|City | Order city|
|State | Order state (where applicable)|
|Country | Order country|
|Country latitude | Geographic coordinates of the order country|
|Country longitude | Geographic coordinates of the order country|
|Region | Region to which the order belongs to|
|Market | Market to which the order belongs to|
|Subcategory | Product subcategory|
|Category | Product category|
|Product | Product name|
|Quantity | Number of products purchased per order|
|Sales | Total sales in $|
|Discount | Discount applied to the order|
|Profit | Total profit for each order after discount|

# **3. Requirements**
Using Power BI, analyze an order dataset from a global skincare and beauty e-store
The primary goals are to: 
1) Analyze sales volumes and profitability across various product groups and markets, focusing on key performance indicators (KPIs) critical to the e-store's success
2) Provide actionable insights that can drive strategic decision-making for the e-store's future growth.

# **4. Design thinking**
**Step 1 - Empathize**
|5W1H | |
|---|----------------|
|Who will be viewing this Dashboard? | Sales team, Marketing team|
|If we had to choose only one key Stakeholder, who would it be?  | Sales team|
|What problem does this Dashboard solve?  | A sales dashboard provides a centralized view of key sales metrics and performance indicators to help sales teams monitor performance, identify trends, and make data-driven decisions.|
|Describe the problem in one sentence  | Centralized view of key sales metrics and performance indicators.|
|When and where will Stakeholders view this Dashboard?  | The Dashboard can be viewed daily or weekly, depending on the specific needs and goals of the organization or when presenting to stakeholders.<br>The Dashboard can be accessed from a variety of devices, including computers, laptops, tablets, and smartphones.|
|Why do stakeholders need this Dashboard?  | Monitor sales performance<br>Identify trends and opportunities<br>Improve sales efficiency<br>Support strategic planning<br>Reduce risk|
|How have stakeholders been achieving their goals so far?  | Through report analysis, stakeholders can gain a comprehensive understanding of key business indicators, facilitating the monitoring of current business situations and forecasting trends.|

|Stakeholder Empathy Mapping | |
|---|----------------|
|Pains  | Lack of defined key performance indicators (KPIs) to track business success, coupled with a limited understanding of target markets and core product offerings.|
|Thinking and feeling  | Need to enhance their understanding of sales performance and key sales metrics to optimize sales strategies, as current data and reporting capabilities are insufficient.|
|Seeing  | A clearer understanding of the current business situation, including whether targets are being met and whether growth or decline is occurring, is necessary.|
|Saying and doing  | "We need more data-driven insights." "Our strategies need to be more targeted." Actively seeking better tools and processes for data analysis and sales KPI|
|Gains  | Enhancing sales performance understanding, implementing better-targeted sales campaigns, increasing sales and engagement, and streamlining decision-making processes.|

|Fact table | Dim table|
|---|----------------|
|Fact_Transaction  | Dim_Date|

**Step 2 - Define POV**
| | NORTHSTAR METRIC|
|---|----------------|
|What VALUE you want to measure?  | Revenue, Profit|
|WHEN the value DELIVERY SUCCESS?  | When the revenue meets or exceeds the predefined target, indicating successful sales and profitability.|
|Northstar Metric Name  | Revenue|
|WHY do you choose this metric?  | Revenue is a key indicator of business growth and success, as it measures the total sales generated and reflects the company's financial health.|

Dimension Group
|Group 1 | Group 2 | Group 3 |
|---|----------------|-----|
|Market | Product| Customer|

Define Point of View
|View | Description | Why |
|---|----------------|-----|
|Sales Overview | Overview of revenue (Total, Market, Product, Customer Segment)| To provide a high-level view of overall business performance aiding strategic decision-making.|
|Market Analysis | Revenue analysis by Market| To monitor detailed performance trends and understand the impact of market factors on revenue growth.|
|Product Analysis | Revenue analysis by Product| Provide insights into product performance, best-selling items, and order history over time.|
|Customer Analysis | Revenue analysis by Customer| Offers a comprehensive view of customer data to identify key segments, track customer journeys, and measure loyalty.|

**Step 3 - Ideate**

Brainstorming
|Idea Name | Layer 0 Dimension: Total Metrics | Layer 1 Dimension: Breakdown by 1 Dimension | Layer 2 Dimension: Breakdown by 2 Dimensions|
|---|----------------|-----|-----|
|Sales Overview | | | |
|Market Analysis | | | |
|Product Analysis | | | |
|Customer Analysis | | | |

Next, I proceeded with **Step 4 - Prototype** and Review multiple times and achieved the final result, which will be presented in the following section as a dashboard.
# **5. Dashboard**

<img src="https://i.imgur.com/DAYlQdv.png">

***

<img src="https://i.imgur.com/Wnz9CFl.png">

***

<img src="https://i.imgur.com/pWUgr53.png">

***

<img src="https://i.imgur.com/jhtY7MF.png">

# **6. Key Insights**
**Sales Trends by Market:** *North America* and *Europe* consistently outperformed other markets with growth across all product categories.

**Most Profitable Segments:** *The corporate segment* was consistently the most profitable customer segment from 2020 to 2023.

**Profit Distribution by Market:** North America, Europe, and Australia were the most profitable regions, with *North America* leading the way.

**Best-selling products:** *Herbal Essences Bio*, a *body care* product, has been the top seller for four years, driving the highest profit margins in the industry.

**Discount Strategy Review:** The discount strategy over the last few years appears to have *negatively impacted profits*, suggesting it may not have been effective. However, this is a simplistic analysis and there could be other factors at play. For a more comprehensive analysis, other factors such as sales volume, customer retention, and market conditions should also be considered.

