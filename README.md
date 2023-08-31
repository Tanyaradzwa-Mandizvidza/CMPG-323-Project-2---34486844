# CMPG-323-Project-2---34486844
For the EcoPower Logistics Management API project, we're designing a powerful RESTful API for seamless logistics data management. With CRUD capabilities and structured endpoints, we're enhancing operations, optimizing resources, and embracing technology's potential.The purpose of this project is to develop an API for handling solar energy system logistical data. This README gives stakeholders instructions on how to use the API and the related report.The C#.Net Core Web API will be used to develop the API.Swagger will be integrated into the API to build and distribute documentation.

# Branching Strategy
I will use a version control strategy for tis project in order to efficiently manage the projects development process. This approach guarantees the main repository's stability while allowing me to work on new features and fixes at the same time.The brances will work as follows.
Master: The stable version of the project will always be found in the master branch. It displays the current level of production readiness. Develop: The branch that will be used for continuous development will be develop branch, it will act as the integration branch. Before being merged into the master branch, it serves as the integration point for new features, bug fixes, and other improvements. 
Feature: Specific features or tasks will have their own feature branches. The develop branch gives rise to multiple feature branches, each of which focuses on a different feature. The feature will be finished and then merged back into the develop branch.

The following information will allow you to use the EcoPower API AND its related report:

Visit the provided GitHub repository to get started with the API. Open it in Visual Studio when you clone the repository to your local computer. To guarantee appropriate communication with the MySQL database, make sure to configure the required database connection settings in the "appsettings.json" file. Customers administration, order processing, and product tracking are just a few of the logistics-related activities that the API's endpoints can handle.

The "Readme.md" file has thorough details about each route, HTTP method, and payload structure and is a good resource for knowledge about the API's endpoints. The creation, reading, updating, and deletion of entities within the database are all covered in this documentation for users. To get a list of customers, for instance, you might navigate to the proper endpoint and issue a GET request. You would make a POST request containing the required payload including the order details to the chosen order endpoint in order to generate a new order. The RESTful principles are also followed while updating and removing entries.

# API Endpoints
# Customers

GET /api/Customers`: Retrieve all customer entries from the database.
GET /api/Customers/{id}`: Retrieve a single customer based on the provided ID.
POST /api/Customers`: Create a new customer entry.
PUT /api/Customers/{id}`: Update an existing customer entry.
DELETE /api/Customers/{id}`: Delete an existing customer entry.

# Orders

GET /api/Orders`: Retrieve all order entries from the database.
GET /api/Orders/{id}`: Retrieve a single order based on the provided ID.
GET /api/Orders/Customer/{customerId}`: Retrieve all orders for a specific customer.
POST /api/Orders`: Create a new order entry.
PUT /api/Orders/{id}`: Update an existing order entry.
DELETE /api/Orders/{id}`: Delete an existing order entry.

# Products

GET /api/Products`: Retrieve all product entries from the database.
GET /api/Products/{id}`: Retrieve a single product based on the provided ID.
GET /api/Products/Order/{orderId}`: Retrieve all products for a specific order.
POST /api/Products`: Create a new product entry.
PUT /api/Products/{id}`: Update an existing product entry.
DELETE /api/Products/{id}`: Delete an existing product entry.

# Additional Features

Role-based Authentication: The API supports role-based authentication using JSON Web Tokens (JWT).
Data Validation: Input data is validated to ensure integrity and consistency.
Error Handling: Proper error responses are provided for invalid requests.
Foreign Key Constraints: The API enforces foreign key constraints to maintain data integrity.
Data Pagination: Some endpoints support pagination to manage large datasets.

# Database information
As the relational database management system (RDBMS) for the project, MySQL is used to store and manage the data. Data about customers, orders, items, and other entities is saved in the database, which acts as an organized repository. The project's backend API communicates with the MySQL database to carry out a number of actions, including getting customer and order information and adding, modifying, and removing records. Foreign key constraints are used in the database schema to create associations between various entities, preserving the consistency and integrity of the data. Entity Framework is used by the API's controllers to manage transactions, run SQL queries on the MySQL database, and connect to the database.

# Reference List
See reference list document with all the requested references.
