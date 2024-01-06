# e-commerce-purchases

---

## This project implements an e-commerce project
---

### In the course of the project, the following tasks need to be solved:
1. How many users made only one purchase?
2. How many orders per month are not delivered on average for various reasons (provide a breakdown by reasons)?
3. Determine which day of the week each product is most frequently purchased.
4. How many purchases per week does each user make on average (by month)?
5. Using pandas, conduct a cohort analysis of users. Identify the cohort with the highest retention in the third month from January to December.
6. Using Python, build RFM segmentation of users to qualitatively assess your audience.

---

### Data description:
- olist_customers_datase.csv - table with unique user IDs
  - customer_id - post-order user ID
  - customer_unique_id - unique user ID
  - customer_zip_code_prefix - user’s postal code
  - customer_city - user’s delivery city
  - customer_state - user’s delivery state
- olist_orders_dataset.csv - order table
  - order_id - unique order identifier (check number)
  - customer_id - post-order user ID
  - order_status - order status
    - created - created
    - approved - confirmed
    - invoiced - invoice issued
    - processing - in the process of assembling
    - the order shipped - shipped from warehouse
    - delivered - delivered to the user
    - unavailable - unavailable
    - canceled - canceled
    - order_purchase_timestamp - order creation time
  - order_approved_at - order payment confirmation time
  - order_delivered_carrier_date - time of transfer of the order to the logistics service
  - order_delivered_customer_date - order delivery time
  - order_estimated_delivery_date - promised delivery date
- olist_order_items_dataset.csv - commodity items included in orders
  - order_id - unique order identifier (check number)
  - order_item_id - product identifier within one order (does not contain information about the number of products)
  - product_id - unique product identifier (analog of a barcode)
  - seller_id - unique product manufacturer identifier
  - shipping_limit_date - maximum delivery date for the seller to transfer the order to the logistics partner
  - price - price per unit of goods
  - freight_value - weight of goods
