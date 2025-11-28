# PIZZA-SALES-PANALYSIS
An Excel project analyzing a year's worth of sales from a fictitious pizza sales place. The dataset encompasses details such as pizza type, size, quantity, price, and ingredients. The goal is to derive actionable insights to inform strategic decisions and optimize overall operational effectiveness.

### Table of Contents
- [Project Overview](https://github.com/Oluwaseun2024-ctrl/PIZZA-SALES-PANALYSIS#project-overview)
- [Project Scope](https://github.com/Oluwaseun2024-ctrl/PIZZA-SALES-PANALYSIS#project-scope)
- [Project Objectives](https://github.com/Oluwaseun2024-ctrl/PIZZA-SALES-PANALYSIS#project-objectives)
- Expected Outcome
- Document Purpose
- Use Case
- Data Source
- Data Cleaning and Processing
- Data Analysis
- Data Visualization
- Recommendation
- Conclusion

### Project Overview
This project involves an in-depth analysis of a year's worth of sales data from a fictitious pizza place. The analysis is performed using Excel, providing valuable insights to drive strategic decisions and optimize operational effectiveness.

### Project Scope
The project covers a comprehensive analysis of pizza sales, including order details, orders, pizza types, and pizzas. The analysis spans a full year, providing a detailed view of operational performance during this period.

### Project Objectives
The primary objectives of this analysis are:

- **Sales Analysis:** Understand sales patterns over the year, identifying peak times and high-demand periods.
- **Product Performance:** Evaluate which types and sizes of pizzas are most popular and generate the most revenue.
- **Customer Preferences:** Analyze ingredient popularity and preferences to refine the menu offerings.
- **Operational Insights:** Uncover inefficiencies and areas for improvement in operations and supply chain management.

### Expected Outcome
The analysis aims to provide actionable insights, including:
- Daily customer count.
- Identification of peak hours.
- Average number of pizzas per order.
- Identification of bestsellers.
- Revenue analysis.
- Detection of seasonality in sales.
- Recommendations on menu optimization and promotional strategies.

### Data Source
The dataset for this project is sourced from [Maven Analytics website](https://app.mavenanalytics.io/datasets?dataStructure=Single+table&search=BANK) designed specifically for practice purposes. It is presented in an Excel file with four tables (Order Details, Orders, Pizza Types, and Pizzas) comprising 48,620, 21,350, 32, and 96 rows respectively, and 4, 3, 4, and 4 columns respectively. The dataset includes key attributes essential for a comprehensive analysis, such as:

**_1. How many customers do we have each day?_**

The primary objective of this analysis is to determine the daily customer count at Pizza Sales Place using the order_id as a proxy for individual customer transactions. This information helps in understanding the daily customer flow, identifying peak and slow periods, and optimizing business operations.
To achieve this, a pivot table was created. The day column was placed in the row section, and order_id was placed in the value section to count the number of orders. The results were visualized using a bar chart.

![](https://github.com/Oluwaseun2024-ctrl/PIZZA-SALES-PANALYSIS/blob/main/Number%20of%20Customers%20Per%20Day.png)

```𝐴𝑣𝑒𝑟𝑎𝑔𝑒 𝑄𝑢𝑎𝑛𝑡𝑖𝑡𝑦 = 𝑆𝑢𝑚 𝑜𝑓 𝑄𝑢𝑎𝑛𝑡𝑖𝑡𝑖𝑒𝑠 / 𝐶𝑜𝑢𝑛𝑡 𝑜𝑓 𝑄𝑢𝑎𝑛𝑡𝑖𝑡𝑖𝑒𝑠 = 1```


```SQL
SELECT
  Month_Name,
COUNT
  (Complaint_ID) AS [Total No of Complaints]
FROM
  Financial_Consumer_Complaints
GROUP BY
  Month_Name,
  Month_Number
ORDER BY
  Month_Number ASC
```

| Name | Age | Class | City |
|------|-----|-------|------|
|Toyosi|27|JSS 1|Ekiti|
|Seyi|31|Pri 5|ife|

| Year | Total No of Complaints |
| ---- | ---------------------- |
| 2017 | 5394                   |
| 2018 | 7872                   |
| 2019 | 7075                   |
| 2020 | 8942                   |
| 2021 | 11149                  |
| 2022 | 12953                  |
| 2023 | 9131                   |


```PYTHON
sns.scatterplot(x=' Income ', y='NumWebPurchases', data=data)
plt.title('Income vs. NumWebPurchases')
plt.xlabel('Income')
plt.ylabel('Number of Web Purchases')
plt.show()
```
