# Data Visualization and Analytics Interview at Hiflylabs
## Understanding the Dataset
### Context
This is a publicly available dataset of a Brazilian Online Store. The dataset has information of 100k orders from 2016 to 2018 made at multiple marketplaces in Brazil. Its features allows viewing an order from multiple dimensions: from order status, price, payment and freight performance to customer location, product attributes and finally reviews written by customers. We also released a geolocation dataset that relates Brazilian zip codes to lat/lng coordinates.
This is real commercial data, it has been anonymised, and references to the companies and partners in the review text have been replaced.

> [!CAUTION]
> - An order might have multiple items.
> - Each item might be fulfilled by a distinct seller.
> - All text identifying stores and partners where replaced by the names of Game of Thrones great houses.

Open the dropdown menu to get more detail of the contents of each dataset:
<details>
<summary>olist_customers_dataset.csv</summary>

This dataset has information about the customer and its location. Use it to identify unique customers in the orders dataset and to find the orders delivery location.

At our system each order is assigned to a unique customer_id. This means that the same customer will get different ids for different orders. The purpose of having a customer_unique_id on the dataset is to allow you to identify customers that made repurchases at the store. Otherwise you would find that each order had a different customer associated with.

| Column Name | Description |
| --- | ---|
| customer_id | key to the orders dataset. Each order has a unique customer_id |
| customer_unique_id | unique identifier of a customer |
| customer_zip_code_prefix | first five digits of customer zip code |
| customer_city | customer city name |
| customer_state | customer state |

</details>
<details>
<summary>olist_geolocation_dataset.csv</summary>
FIXME
</details>

<details>
<summary>olist_order_items_dataset.csv</summary>
FIXME
</details>
<details>
<summary>olist_order_payments_dataset.csv</summary>
FIXME
</details>
<details>
<summary>olist_order_reviews_dataset.csv</summary>
FIXME
</details>
<details>
<summary>olist_orders_dataset.csv</summary>
FIXME
</details>
<details>
<summary>olist_products_dataset.csv</summary>
FIXME
</details>
<details>
<summary>olist_sellers_dataset.csv</summary>
FIXME
</details>
<details>
<summary>product_category_name_translation.csv</summary>
FIXME
</details>

### Data Schema
The data is divided in multiple datasets for better understanding and organization. Please refer to the following data schema when working with it:
<picture>
![Data Schema](image.png)
</picture>

## Tasks

### Task 1 - Data Modeling & Visualization
*In the following task we'd like to understand your data modeling and visualization skills. Whether you understand the abstraction difference between Executive and Operational dashboards.* 
- Using the above mentioned semantic model diagram assamble the following data model in **Power BI**.
- Build a comprehensive dashboard (i.e. multiple report pages) on which a C-level Executive can visually run a health-check on the company.
- Build an tactical report page where one can track the website's performance in attracting new users and generating revenue.
- Name a few business drivers that executives can use to track the business's success.
- Explore at least three distinct areas in detail in your solution.

> [!TIP]
> Multiple areas can be explored in the data model. Some examples are:
> - Sales
> - Orders
> - Sellers
> - Logistics
> - Customers
> - Web Analytics

### Task 2 - Insight Generation
*In this section we would like to assess your ability to make sense of the data at hand pinpoint the critical aspects of it and your general skills in data storytelling.*
- Name the three most important insights to a C-level executive. Explain your findings in detail! What are the business actions one could take on your insights?
- You can use any method of presentation in your solution.