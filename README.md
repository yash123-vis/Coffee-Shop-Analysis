# Coffee-Sales-Analysis
Using Excel to analyze sales data for a coffee shop. The Goal is to find insights that help improve business performance by looking at things like what people buy, when they buy it, and how busy the stores are. By cleaning and organizing the data, we'll use Excel to understand trends like peak sales hours, popular products, and how sales vary across days, months, and different store locations. 


## PROBLEM STATEMENT:


Analyze sales records and build a Dashboard for a coffee shop using Excel. Identify trends, patterns, and insights that can inform strategic decision-making and enhance business performance. The objective is to explore various aspects of sales data, including product performance, peak sales periods, and revenue trends, to uncover actionable insights that can improve sales strategies.


## RECOMMENDED ANALYSIS:


1. How do sales vary by day of the week and hour of the day ?
2. Are there any peak times for sales activity ?
3. What is the total sales revenue for each month ?
4. How do sales vary across different store locations ?
5. What is the Average Price Per Order ?
6. Which products are the best selling in terms of Quantity & Revenue ?
7. How do sales vary by Product Category and Size ?


## DATA UNDERSTANDING:


Transaction records for Maven Roasters, a fictitious coffee shop operating out of three NYC locations. Dataset includes the transaction date, timestamp and location, along with product-level details.


### 1.Data Structure


    File type : Excel
    Table : 1
    FIELDS : 11
    Records : 149,116
    Data Span : Jan 2023 – Jun 2023(6 months)
    (Source : Maven Analytics)


### 2.Data Description


![image](https://github.com/lkh-pranav/Coffee-Sales-Analysis/assets/165638568/11f67bce-b53c-4b4b-a3f6-4ad876db7e92)


## DATA PREPARATION:

In the data preparation step, the raw sales data from the coffee shop, including transaction records, product information will be collected and organized into a structured format suitable for analysis in Excel. This involves cleaning the data to remove any inconsistencies, errors, or missing values, standardizing formats, and ensuring data integrity. Additionally, data is aggregated and transformed as needed to facilitate analysis, such as calculating total sales, average order value, and average bill per person. Once cleaned and structured, the prepared data will serve as the foundation for building Dashboard.


### Data Cleaning and Tranformation

   
In Power query editor,

•	Reviewing each column to get a good grasp of the data and understand its context within the domain. This helps in recognizing errors, inconsistencies and important information related to the coffee shop's operations.
•	Abbreviations such as "Lg," "Rg," and "Sm" were used to represent the size of products in the "product_detail" column. But instead created a new column named "size" to provide a clearer representation of product sizes.
Sm >> Small , Rg >> Regular , Lg >> Large

•	Leading and Trailing spaces were eliminated from all columns, enhancing the cleanliness and uniformity of the dataset
•	The “transaction_time” column underwent a refinement process where date values were removed, leaving only the time in HH:MM:SS format.

•	A new custom column named "Total_bill" was created by multiplying the “unit_price” and “transaction_qty” for each entry. This addition provides a comprehensive overview of the total sales generated from each transaction.

•	Extracting the “day of the week” and “month name” from the "transaction_date" column allows for a detailed analysis of how sales fluctuate across different days and months. Similarly, extracting the “hour of the day” from the "transaction_time" column enables the identification of peak sales hours.


## CREATE PIVOT TABLES:


Utilized pivot charts to swiftly summarize and analyze data, enabling the rapid identification of trends and patterns. And also by leveraging pivot charts, the process of constructing dynamic dashboards becomes seamless.


![image](https://github.com/lkh-pranav/Coffee-Sales-Analysis/assets/165638568/bbe6af71-eed2-46cc-b615-ef1649be57f6)


## DASHBOARD OVERVIEW:


Crafted an engaging and dynamic dashboard tailored for coffee sales analysis. This interactive platform offers stakeholders a user-friendly interface to explore key metrics, trends, and insights effortlessly.


•	Utilized line charts to visualize sales trends over hours of the day, highlighting peak sales periods and identifying fluctuations in customer demand.


•	Employed horizontal bar charts to depict daily sales performance, enabling easy comparison of sales figures across different days of the week.


•	Utilized pie charts and donut charts to illustrate the percentage distribution of sales based on product sizes and categories, providing a clear visual representation of the contribution of each size and category to overall sales.


•	Implemented column charts to display footfall and sales data for each store location, facilitating comparison of customer traffic and revenue generation across different stores.


### Check out my [Excel Workbook](https://1drv.ms/x/c/594dd24d75e2ee39/IQNwXvYC9xfkR40x0s6Q3XCjATkxaISe5KJBz9702WkE8FM)


### Snapshot


![Dashboard](https://github.com/lkh-pranav/Coffee-Sales-Analysis/assets/165638568/1a396976-e919-4b61-b6fa-c2f40a11b23b)


### INSIGHTS:


### Busiest Days and Times: 
•	The busiest hours for coffee sales are between 8:00 AM and 10:00 AM, indicating strong demand during morning rush hours.
•	Mondays and Fridays tend to have the highest sales volumes, indicating increased demand at the beginning and end of the workweek.


### Percentage share based on Size:
•	Large-sized drinks dominate the sales representing the preferred choice among customers while Small-sized drinks are the least contributed.


### Comparable Footfall Distribution:
•	All stores exhibit almost similar level of foot traffic throughout the months, indicating a balanced distribution of customers across different locations. Similar footfall levels present equal opportunities for sales and revenue generation across all stores.


### Percentage share based on Category:
•	Coffee and Tea Categories  account for the largest percentage share of sales which is about 67% with Coffee being the most contributed(39%).

### Top Products
•	Barista Espresso emerges as the best-selling product, reflecting a strong demand for coffee among customers followed by Brewed Chai Tea ranks as the second-highest selling product.




