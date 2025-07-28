# Profitability Insights and Delivery Risk Prediction in E-Commerce

## Project Overview

This project explores the key drivers of order profitability and late delivery risk in an e-commerce business. Using detailed order-level data, we analyze how variables such as product category, shipping mode, and quantity affect profit margins. We also build a predictive model to classify orders at risk of late delivery, leveraging features like scheduled shipment days, shipping method, and regional attributes.

The goal is to uncover high-margin segments, flag unprofitable patterns, and provide a data-driven foundation for improving operational efficiency. The findings support smarter product pricing, better carrier selection, and proactive delivery risk mitigation.


## Summary

- This report analyzes a total of 180,519 orders, generating a combined profit of $3,966,903. The average profit margin across all orders is 10.78%. 
- The most profitable product category Fishing, under consumers; contributing 19% of total profit. 
- The shipping mode most associated with late delivery is First Class, where late delivery risk is 95%.

## Data Overview

The dataset contains detailed records of transactions and supply chain operations from DataCo Global, covering multiple product categories including Clothing, Sports, and Electronic Supplies. The data spans the full order lifecycle—from customer details and purchase behavior to shipping logistics and profit metrics.

It includes 52 structured fields such as product category, customer location, shipping dates, delivery status, order profit, and pricing. Key variables like "Late delivery risk", "Benefit per order", and "Shipping mode" support analysis of operational performance and customer behavior.

This structured dataset was analyzed to understand inefficiencies across provisioning, production, and distribution processes, enabling insights into delivery delays, profit margins, and customer segmentation. It is particularly suited for advanced analytics and machine learning models to optimize supply chain operations and forecast demand patterns.

<p align="center">
  <img src="Data Visualizations/Data 1.png" alt="Data Overview" width="200", height = "600", style="display inline-block;"/>
  <img src="Data Visualizations/Data 2.png" alt="Profits Margins by Shipping Modes" width="200", height = "600", style="display inline-block;"/>
</p>

## Analysis and Insights

  ![alt text](https://github.com/Lopeznil/Projects/blob/main/Profitability%20Insights%20and%20Delivery%20Risk%20Prediction%20in%20E-Commerce/Data%20Visualizations/Sales_Overview.png "Sales Overview")

### Key drivers of profitability

- Sales vs Profits
    - As expected, on average, a higher sales volume generates more profit. Products related to fishing generated $6.9M worth of sales, accounting for nearly 20% of all sales, with a profit of $0.7M.
    - Although products related to fishing has the highest sales, its average profit margin is only 10.91%, indicating potential margin leakage. In contrast, products related to Golf have a significantly smaller sales volume but delivers a margin of 17.46%.

<p align="center">
  <img src="Data%20Visualizations/Sales_Profits.png" alt="Sales vs Profits organized by category" width="700", height = "525">
</p>
<p align="center">
 <img src="Data%20Visualizations/Sales_Profit_margins.png" alt="Sales vs Profit Margins organized by category" width="700", height = "600">
  </p>
  
- Shipping Modes vs Profits
    - Majority of orders were placed through standard class shipping compared to other modes, hence generating a larger profit.
      However, looking at profit margins paint a different story.
    - First class shipping achieves a profit margin larger than 11%, whereas, other modes only average 10.5%.

<p align="center">
  <img src="Data%20Visualizations/Shipping%20Modes.png" alt="Count of orders by Shipping Modes" width="400", height = "300",style="display inline-block;">
  </p>
<p align="center">
  <img src="Data%20Visualizations/Shipping%20Mode%20Profit.png" alt="Profits by Shipping Modes" width="400", height = "300",style="display inline-block;"/>
  <img src="Data%20Visualizations/Shipping%20Mode%20Profit%20Margin.png" alt="Profits Margins by Shipping Modes" width="400", height = "300", style="display inline-block;"/>
</p>

- Order Quantity vs Profits
    - As expected, on average, higher order quantities generate more profit. The visual seemingly shows a linear relationship between the two variables, in most categories.
    - Profit margins are seemingly unaffected by order quantities, in some cases having a negative impact on profit margin.

<p align="center">
  <img src="Data Visualizations/Top 5 Profitable_Profit_Quantity.png" alt="Profits by Order Quantity for Top 5 most Profitable Categories" width="700", height = "525",style="display inline-block;">
  </p>
  <p align="center">
  <img src="Data Visualizations/Top 5 Profitable_Margin_Quantity.png" alt="Profit Margins by Order Quantity for Top 5 most Profitable Categories" width="700", height = "525",style="display inline-block;">
  </p>

### Late delivery risks

- Shipping Modes
    - The late delivery rate across all orders averages to 55%. The shipping mode most associated with late delivery is first class, where late delivery rate is 95%.
    - Orders scheduled for more than 1 days are 3x less likely to be late.

  <p align="center">
  <img src="Data Visualizations/Late Delivery Risk by shipping modes.png" alt="Late Delivery Risk by shipping mode" width="400", height = "300",style="display inline-block;">
  <img src="Data Visualizations/Delivery risk by scheduled shipment days.png" alt="Late Delivery Risk by scheduled shipping time" width="400", height = "300",style="display inline-block;">
  </p>
  
## Suggestions
### Profitability
  - Categories like 'Golfing' yield higher profit margins (~17%) despite lower sales volume. Prioritizing the promotion of such low-volume, high-margin products can significantly enhance overall profitability.
  - Assess the impact of high-quantity discounts on profitability by analyzing the relationship between per-order quantities and average profit margins across total quantities sold, to identify categories where discount strategies should be reconsidered or reduced.
### Late Delivery risks 
  - Examine the reliability of First Class shipping, as the scheduled delivery dates are being consistently underestimated.

## Tools Used

### Power BI
  - Developed the visualizations presented in this report.
### Python
  - Extracted  data of company in CSV format.
  - Removed uninformative columns and verified data types for consistency.

