# Narmeen-products-collection

This repository contains a Postman collection that demonstrates various API requests for managing product data. The collection includes multiple API operations such as retrieving, adding, updating, partially updating, and deleting product objects.

Features
GET Requests:

GetAllObjects: Retrieves all product objects.
GetListOfObjects: Retrieves a filtered list of product objects.
GetSingleObject: Retrieves a single product object by ID.

POST Request:

AddObject: Adds a new product object to the collection.

PUT Request:

UpdateObject: Updates an existing product object.

PATCH Request:

PartiallyUpdateObject: Partially updates an existing product object.

DELETE Request:

DeleteObject: Deletes a product object by ID.

### Environment Variables

The collection uses two environment variables to make the requests dynamic:

url: The base URL of the API.

object_id: The ID of a specific product object (used dynamically in certain requests).

Before running the requests, make sure to import both the collection and the environment into Postman.

### How to Import the Collection and Environment
Download the collection and environment files from this repository.
Open Postman.
Click Import (located at the top-left of the Postman window).
Select the File tab and choose the downloaded collection (ProductsCollection.postman_collection.json) and environment (ProductsCollection-QA.postman_environment.json) files.
Click Import to add them to Postman.

### Environment Variables Setup:
URL: (https://api.restful-api.dev).
object_id: The product ID you want to work with for GET, PUT, PATCH, and DELETE requests. This will be used dynamically in the request URLs.

### How to Use
Once the collection and environment are imported, select the environment in the top-right corner of Postman.
Make sure to set the url and object_id in the environment before running the requests.

### Test Scripts
I have added test scripts to each request to verify that the APIs are working as expected and that the responses are correct. These tests include checks for:

Status codes: Ensure the response status code is correct (e.g., 200 OK, 201 Created).
Response validation: Ensure the response contains the expected data (e.g., product name,id etc).
Dynamic variables: Ensure the correct use of environment variables like url and object_id.
Each request has been tested to confirm that it functions as expected.

