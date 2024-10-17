Web Service and Data Layer
-------------------------

The first part of the assignment involves the creation of domain model and a data service.
The data service layer is responsible for establishing communication with the database. In this case, the database 
is "Northwind" which is widely used for testing purposes.

The excepted learning outcome is to understand the mapping between the database model and the object-oriented model.
The domain of the problem will be handled using EF core(Entity Framework Core).

The requirements as quoted in the Assignment are:
--Order
1. Get a single order by ID: Retrieve the complete order, including all its attributes
and the entire list of order details. Each order detail should include the product,
which must also include the category.
2. Get orders by shipping name: Return a list of orders with their ID, date, shipping
name, and city.
3. List all orders: Provide a list of orders with the same information as in
requirement 2.

--Order Details
4. Get details for a specific order ID: Retrieve the order details, including the
product.
5. Get details for a specific product ID: Obtain the complete list of details,
including the product and the order. Order the details by Order Id.

--Product
6. Get a single product by ID: Return Id, Name, UnitPrice, QuantityPerUnit and
UnitsInStock from product plus the name of the category.
7. Get a list of products containing a substring: Search for products with names
matching the given substring and return a list containing only the product names
and category names. [Hint: This requires a new object with only these two
attributes]
8. Get products by category ID: Retrieve a list of products belonging to the given
category, including information as described in requirement 6.

--Category
9. Get category by ID: Return the category if found; otherwise, return null.
10. Get all categories: Provide a list of categories, including their ID, name, and
description.
11. Add a new category: Add a new category to the system, accepting name and
description as arguments. The system should generate a new ID and return the
newly created category.
12. Update category: Accept ID, name, and description as arguments and update the
category with the provided information. If the category is found, update it, and
return true; otherwise, return false.
13. Delete category: Accept the category's ID as an argument. Return true if the
category is successfully deleted; otherwise, return false


To ensure that the web service is functional and implies to what actually is required in the Assignment, a test driven programming approach is followed. The test cases are provided in the Assignment.