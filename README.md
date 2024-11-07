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
|Sales Overview | Total revenue<br>Total profit<br>Total order<br>Total unit sold| % revenue by market<br>% revenue by segment<br>% profit by category<br>Revenue and Profit trend by year| |
|Market Analysis | Slicer: year, country, segment, product| % profit by region| % revenue by region and year<br>Top products in each market|
|Product Analysis | Slicer: year, country, segment, product| % revenue by category<br>Order times<br>Highest ordered product| % profit by segment and category<br>Profit and Discount Relation|
|Customer Analysis | Total customer<br>Total order<br>Avg revenue by transaction<br>Avg profit by transaction| Count customer by region<br>Profit margin by segment| Top customers by country|

Next, I proceeded with **Step 4 - Prototype** and Review multiple times and achieved the final result, which will be presented in the following section as a dashboard.
# **5. Dashboard**

**VIEW 1**
<img src="https://i.imgur.com/DAYlQdv.png">

* Overview: While sales and units sold _increased_, profits _decreased_ year-by-year. This could be due to various factors like increased costs, lower selling prices, or a change in product mix.
* The _corporate segment_ was consistently the most profitable customer segment from 2020 to 2023.
* The _Europe_ market has been the most profitable from 2020 to 2023.
* _Body care_ has generated the highest profits, followed by make-up and face care.

***

**VIEW 2**
<img src="https://i.imgur.com/Wnz9CFl.png">

* _North America_, _Europe_, and _Australia_ were the most profitable regions, with North America leading the way.
* _North America_ consistently outperformed other markets with growth across all product categories.
* The top-selling products vary by region, highlighting the importance of tailoring product offerings to local preferences.

***

**VIEW 3**
<img src="https://i.imgur.com/pWUgr53.png">

* _Herbal Essences Bio_ is the best-selling product, with the highest sales and profit. It has also shown significant year-over-year (YoY) sales growth.
* The _body care_ category is the most profitable category for all customer segments. It generates the highest total sales and profit.
* The _face care_ category has the highest profit margin, indicating strong pricing and cost control.
* Orders are highest on _Fridays_ and _Saturdays_, indicating potential opportunities for targeted marketing campaigns and promotions.
* The discount strategy implemented in the past few years has had a mixed impact on profit. Some discounts have increased sales but _negatively_ impacted profit margins.

***

**VIEW 4**
<img src="https://i.imgur.com/jhtY7MF.png">

* The average sales value per transaction is $181, and the average profit per transaction is $40. This indicates a _reasonable_ profit margin.
* The _corporate segment_ generates the highest total sales and profit, indicating a strong focus on corporate clients.
* The majority of customers (nearly 70%) have made only _one_ purchase. A smaller number of customers have made multiple purchases, with the highest frequency being two. This suggests a decreasing trend in customer retention or repeat purchases.

# **6. Recommendations**

**Improve Profitability**: Conduct a detailed analysis of the factors contributing to the decline in profitability, which may involve reducing costs, increasing prices, or changing the product mix.

**Market Penetration**: Explore new market opportunities, particularly in Asia Pacific.

**Product Line Optimization**: Optimize product line by discontinuing low-performing products and introducing new products that align with market trends.

**Customer Retention**: Efforts should be made to convert one-time buyers into repeat customers. This could involve loyalty programs, personalized marketing, or improved customer service.

