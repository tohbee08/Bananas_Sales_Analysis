# Bananas_Sales_Analysis
## Table of Content
### Project Overview
### Data Sources
### Tools
### Data Cleaning and Preparation
### Exploratory Data Analysis (EDA)
### Recommendation
### Reference

### Project Overview

Bananas offers subscriptions to their online platform for project management. Bananas' sales data was explored from July 2019 through June 2021, which is organized by Customer ID and Sales Month. Bananas data analysis aim to provide insights into the sales performance of a subscription based SaaS(software as a service) start-up company. By analyzing the sales data, we aim to find trends, gain insight into customers behaviour, predict sales and gain a deeper understanding of the company's present and future financial performance in sales.

### Data Sources

The primary dataset used for this analysis is the "Bananas Sales.xlsx" file, containing detailed account history of the company, which include the customer ID, sales month and subscription type of its customers.

### Tools

- Microsoft Excel
- Data Cleaning and Preparation | Data Analysis

### Data Cleaning and Preparation
In the preparation stage, the following tasks was peformed
- Data loading, cleaning, exploration and questioning.
 - Irrelevant Columns was removed and relevant ones was added which include:
 - upsell $ per non-paying user
 - non-paying users
 - current upsell $
 - upsell priority
 - upsell account detail

### Exploratory Data Analysis (EDA)
EDA of Bananas sales help us gain insight into understanding customer profile and behaviour, find correlation and sales trend and also generate hypothesis for further analysis. The following was observed:
1. Bananas have 55,658 number of users, 35,101 subscribers and $693,025 sales amount, averaging $312 per month.
2. Bananas sell their platform subscriptions at various levels for different prices. Basic users enjoy a "freemium" experience, a free product with limited use. Premium users pay $10 per license, Business users pay $25 per license, and Enterprise users negotiate their price.

### Data Analysis
1. Subscription Type and Licenses Bought grouped to know the total amount of sales for each paid subscription. $4,110 was the sales amount for Enterprise
2. Sales month and subscription type was sliced to gain better understanding of sales trend in each grouped sunscription type.
3. Senior management is looking to identify upsell opportunities. Upsell means getting non-paying accounts to convert to paying accounts of Basic to $10, premium to $10, business to $25 and Enterprise to $27. The total upsell would have been $272,473 if Bananas had all their users paying.
4. Even though we found out how much money Bananas could have made had if they had all their customers paying, it does not address which accounts the customer success team should target for upsell opportunities.
5. Total Upsell $ calculates all the upsell opportunities from each sales month. This isn't helpful in a current analysis because we can't go back in the past. So, Total Upsell $ becomes Current Upsell $ and maximum sales month is used to get the sum of the current Upsell $, which amount to $38,093.
6. To help the customer success team, we will create categories for them to work from.  if Current Upsell $ is greater than or equal to 400, then High, else if Current Upsell $ is greater than or equal to 100, then Medium, else if Current Upsell $ is less than 100, then Low. This will help them prioritize the account that can be targeted for upsell opportunity.
7. Sales month data was aggregated to gain some good insight on month-to-month trends. The analysis shows total sales is increasing while average sales per customer is decreasing.
8. Because Avg Sales Per Customer is decreasing while Total Sales is increasing, one hypothesis for this relationship could be that the share of non-paying customers ("Basic" subscriptions) are growing faster than our paying customers. So, we found out the number paying customers so we can compare the two cohorts.
9. Even though we got the Current Upsell $, which gave us a total amount that could be earned if Bananas got every active non-paying user to upgrade their account.
While that number was insightful, it's still quite unrealistic as Bananas cannot get all their customers to upgrade. The following scenario analysis to see how much we think this is a more realistic sales opportunity was done:
- Projected Upsell Amount that calculates the Current Upsell $ for each Subscription Type and Conversion Rate of 50% for Basic, 45% for Premium, 30% for Business and 15% for Enterprise.
- We know the last month's Sales Amount was about $80,000 but the management aims to earn $100,000 in monthly sales revenue. Using goal seek to find what the Growth Rate needs to be if Sales Target = $100,000, it was dicovered that growth rate has to be at 24%.
- Bananas also wants to explore increasing sales revenue by increasing prices, and they want to see how the projected sales would change in a specific scenario for each Subscription Type. If prices of license is increased, there will be an increase in projected sales.
 - Demand could dcrease if there is an increase in price. 

10. The leadership team at Bananas is goal planning for next month, and they're curious about what sales might be. They want us to forecast this for them using historical data.
- simple moving average (SMA) and weighted moving average (WMA) was used to forecast sales
- Both SMA and WMA forecast an increase in sales of $70,538 and $73,491 respectively for next month.
- Also, the trendlibne shows this is rapid increase in sales.

11. Trendlines didn't give us an output with numbers, only a graphic representation. While this is nice, having a worksheet with actual numbers can be better. Bananas would like actual numbers for a forecast that uses a sophisticated methodology and can consider seasonality and confidence levels.
- The use of forecast sheet was used to create a sophisticasted prediction model.
- Forecast 1 shows the sales month over the past years, showing increase in sales monthly.
- Forecast 2 shows the recent sales month history, and there will be a slight decrease in sales in the first month before a rapid increase in sales with confidence level @90%

### Recommendation
1. To increase revenue, Bananas should prioritize the current Upsell $ that is >= 400, "High"
2. Bananas should also upgrade its customers to a paying account to generate more sales.
3. In order to achieve a sales target of $100,000, the growth rate has to be 24%, which can be achieved by increasing subscription prices.

### Reference
[www.datacamp.com]


