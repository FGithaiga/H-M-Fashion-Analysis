## OVERVIEW 

The H&M Fashion Dataset contains information about products sold by H&M, including details about customers, orders, and product attributes. This dataset is intended for data analysis, machine learning, and business intelligence purposes, allowing users to gain insights into customer behavior, product performance, and sales trends.

## Dataset Structure

The dataset consists of several tables, each representing different entities related to H&M's business operations. The main tables include:

1. **Brand**
   - `BrandID`: Unique identifier for each brand (Primary Key)
   - `BrandName`: Name of the brand

2. **Category**
   - `CategoryID`: Unique identifier for each product category (Primary Key)
   - `CategoryName`: Name of the product category

3. **Product**
   - `ProductID`: Unique identifier for each product (Primary Key)
   - `ProductName`: Name of the product
   - `BrandID`: Foreign key referencing the Brand table
   - `CategoryID`: Foreign key referencing the Category table
   - `Price`: Price of the product
   - `Color`: Color of the product
   - `Size`: Size of the product
   - `StockQuantity`: Quantity of the product in stock

4. **Customer**
   - `CustomerID`: Unique identifier for each customer (Primary Key)
   - `Name`: Name of the customer
   - `Email`: Email address of the customer (Unique)
   - `Gender`: Gender of the customer
   - `Age`: Age of the customer
   - `MembershipStatus`: Membership status of the customer

5. **Orders**
   - `OrderID`: Unique identifier for each order (Primary Key)
   - `CustomerID`: Foreign key referencing the Customer table
   - `OrderDate`: Date when the order was placed
   - `TotalAmount`: Total amount of the order
   - `PaymentMethod`: Method of payment used for the order

6. **OrderDetails**
   - `OrderID`: Foreign key referencing the Orders table
   - `ProductID`: Foreign key referencing the Product table
   - `Quantity`: Quantity of the product ordered
   - `Price`: Price of the product at the time of the order

