# Jumia (NG) Sales Analysis

### Project Overview

This project seeks to deliver insights into the sales performance of an e-commerce company over the past year. Through an in-depth analysis of sales data, I aim to uncover trends and gain a comprehensive understanding of the company's performance within the Nigerian market. Using Microsoft Excel, I analyzed key insights from a raw dataset, including KPIs, discounts, feedback, locations, payment methods, and quarterly data. To complete the project, I presented the findings and recommendations in an interactive report using Microsoft Power BI.

### Data Source

The main data source for this analysis is the "Jumia (NG) Sales Data" file, which contains sample information on each sale conducted by the company in the Nigerian market.

### Tools

 - Microsoft Excel - Data Cleaning and Analysis
 - Microsoft Power BI - Creating a report

### Data Cleaning/Preparation

 1. Data loading and Inspection.
 2. Handling Missing Values.
 3. Formatting

### Exploratory Data Analysis

EDA (Exploratory Data Analysis) involved examining the sales data to address key questions such as:
 1. What are the top-performing products in terms of sales?
 2. Which state generate the highest revenue?
 3. What are the monthly sales trends?

### Data Analysis

- Determined the sale price by multiplying the unit price by the quantity sold: =[@[Unit Price]]*[@Quantity].
- Applied discounts using XLOOKUP: 15% for order quantities of 2-4, 25% for quantities of 5 or more, and no discount for single-quantity orders: =XLOOKUP(E3,$P$2:$P$6,$Q$2:$Q$6,,0).
- I was able to calculate the discount amount for each item and used IFERROR to manage cases where there are no discounts: =IFERROR([@[Sale Price]]*[@Discount],"No Discount") and =IFERROR([@[Sale Price]]-[@[Discount Amount]],[@[Sale Price]]).
- I extracted the month from the date to facilitate trend analysis on a monthly basis: =MONTH([@Date]) 
- Used pivot tables to obtain the most ordered item, top location, total sales price, gross sales, units sold, and top feedback.


 ### Results/Findings

 The analysis results are summarized as follows 
  1. Smartwatches recorded the highest sales in terms of orders, while laptops had the lowest.
  2. Abia State ranked as the leading location for ordered goods.
  3. No orders were placed in 12 states, including Cross River, Akwa Ibom, Edo, Imo, Nasarawa, FCT, Plateau, Kebbi, Gombe, Borno, Jigawa, and Katsina.
 4. Sales saw a significant decline in February, followed by a substantial increase in May.
 5. The majority of customers prefer using the bank transfer method for payments.
 6. The total sales amounted to ₦525,245,545, while the gross sales reached ₦646,606,647.
 7.Bayelsa recorded the highest number of "bad" feedback reports from customers.
 8. Quarter 3 performed best in terms of sales
 9. The total units sold amounted to 6,176.

 ### Recommedations
 - Since smartwatches had the highest sales while laptops had the lowest, consider expanding the range of smartwatches or related accessories.
 - Given that 12 states reported no orders, targeted marketing campaigns and localized promotions should be developed to reach potential customers in these regions.
 - Bayelsa's high number of negative feedbacks suggests there may be underlying issues with customer satisfaction. Investigate the cause of these complaints, whether related to product quality, customer service, or delivery issues.
 - Given the significant sales increase in May and the decline in February, consider planning targeted promotions during periods of low sales.
 - Stock up on high-demand products such as smartwatches and smartphones.
 - Abia State was the top location for orders, suggesting that regional marketing efforts were effective there. Extend successful marketing tactics in Abia to other regions with potential, like Ebonyi and Anambra.






 
 
