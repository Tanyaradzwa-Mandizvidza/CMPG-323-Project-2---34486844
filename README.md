# CMPG-323-Project-2---34486844
For the EcoPower Logistics Management API project, we're designing a powerful RESTful API for seamless logistics data management. With CRUD capabilities and structured endpoints, we're enhancing operations, optimizing resources, and embracing technology's potential.The purpose of this project is to develop an API for handling solar energy system logistical data. This README gives stakeholders instructions on how to use the API and the related report.The C#.Net Core Web API will be used to develop the API.Swagger will be integrated into the API to build and distribute documentation.

# Branching Strategy
I will use a version control strategy for tis project in order to efficiently manage the projects development process. This approach guarantees the main repository's stability while allowing me to work on new features and fixes at the same time.The brances will work as follows.
Master: The stable version of the project will always be found in the master branch. It displays the current level of production readiness. Develop: The branch that will be used for continuous development will be develop branch, it will act as the integration branch. Before being merged into the master branch, it serves as the integration point for new features, bug fixes, and other improvements. 
Feature: Specific features or tasks will have their own feature branches. The develop branch gives rise to multiple feature branches, each of which focuses on a different feature. The feature will be finished and then merged back into the develop branch.

The following information will allow you to use the EcoPower API AND its related report:
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

