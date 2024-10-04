# EXPLORING AND CLEANING DATA WITH PANDAS

# Instacart

## Overview
* Instacart is a grocery delivery platform where customers can place a grocery order and have it delivered to them, similar to how Uber Eats and Door Dash work. This particular dataset was publicly released by Instacart in 2017 for a Kaggle competition.

### Task:
* To clean up the data and prepare a report that gives insight into the shopping habits of Instacart customers. After answering each question, there is a brief explanation of my results in a markdown cell of my Jupyter notebook.

### Visualizations:
* This project requires to make plots that communicate my results.

### Functionality

* There are five tables in the dataset, and I used all of them to do my data preprocessing and EDA. Below is a data dictionary that lists the columns in each table and describes that data that hold.

### Data dictionary
1.  instacart_orders.csv: each row corresponds to one order on the Instacart app<br>

- 'order_id': ID number that uniquely identifies each order
- 'user_id': ID number that uniquely identifies each customer account
- 'order_number': the number of times this customer has placed an order
- 'order_dow': day of the week that the order placed (which day is 0 is uncertain)
- 'order_hour_of_day': hour of the day that the order was placed
- 'days_since_prior_order': number of days since this customer placed their previous order

2. products.csv: each row corresponds to a unique product that customers can buy<br>

- 'product_id': ID number that uniquely identifies each product
- 'product_name': name of the product
- 'aisle_id': ID number that uniquely identifies each grocery aisle category
- 'department_id': ID number that uniquely identifies each grocery department category

3. order_products.csv: each row corresponds to one item placed in an order<br>

- 'order_id': ID number that uniquely identifies each order
- 'product_id': ID number that uniquely identifies each product
- 'add_to_cart_order': the sequential order in which each item was placed in the cart
- 'reordered': 0 if the customer has never ordered this product before, 1 if they have

4. aisles.csv<br>

- 'aisle_id': ID number that uniquely identifies each grocery aisle category
- 'aisle': name of the aisle

5. departments.csv<br>

- 'department_id': ID number that uniquely identifies each grocery department category
- 'department': name of the department

### Steps:
1. Open files.
2. Preprocess the data.
3. Analysis:
   - How many items do people typically buy in one order? What does the distribution look like?
   - What are the top 20 items that are reordered most frequently (display their names and product IDs)?
   - For each product, what proportion of its orders are reorders (I created a table with columns for the product ID, product name, and reorder proportion)?
   - For each customer, what proportion of their products ordered are reorders?
   - What are the top 20 items that people put in their carts first (displayed the product IDs, product names, and number of times they were the first item added to the cart)?
