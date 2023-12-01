# designing-a-online-database-for-online-merch
Products:

ProductID (Primary Key)
Name
Description
Price
StockQuantity
CategoryID (Foreign Key referencing Categories table)
Categories:

CategoryID (Primary Key)
CategoryName
Customers:

CustomerID (Primary Key)
FirstName
LastName
Email
Password
Address
PhoneNumber
Orders:

OrderID (Primary Key)
CustomerID (Foreign Key referencing Customers table)
OrderDate
TotalAmount
OrderDetails:

OrderDetailID (Primary Key)
OrderID (Foreign Key referencing Orders table)
ProductID (Foreign Key referencing Products table)
Quantity
Subtotal
Relationships:
One-to-Many relationship between Categories and Products (One category can have many products).
One-to-Many relationship between Customers and Orders (One customer can place many orders).
One-to-Many relationship between Orders and OrderDetails (One order can have multiple order details).
