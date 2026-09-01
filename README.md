# Postman E-commerce API Testing Project

API testing portfolio project using Postman, JavaScript assertions, DummyJSON API, and Newman reports.

## Project Overview

This project demonstrates REST API testing for an e-commerce demo API using Postman.

The collection covers authentication, product endpoints, cart endpoints, and negative test scenarios. DummyJSON is used as a public demo API for testing and portfolio purposes.

## Tools Used

- Postman
- JavaScript assertions
- Postman Environment Variables
- DummyJSON API
- Collection Runner
- GitHub

## API Under Test

Base URL:

```text
https://dummyjson.com
```

Official API documentation:

```text
https://dummyjson.com/docs
```

## Test Coverage

### Authentication

- Login with valid credentials
- Get current authenticated user using bearer token

### Products

- Get all products
- Get single product by ID
- Search products

### Carts

- Get single cart
- Get carts by user

### Negative Tests

- Login with invalid password
- Get non-existing product

## Test Assertions

The collection includes assertions for:

- HTTP status codes
- Response body structure
- Required fields
- Data types
- Authentication token extraction
- Error messages
- Response time

## How to Run

1. Import the Postman collection:

```text
ecommerce-api-tests.postman_collection.json
```

2. Import the Postman environment:

```text
dummyjson.postman_environment.json
```

3. Select the environment:

```text
DummyJSON Environment
```

4. Run the collection using Postman Collection Runner.

## Test Run Summary

Latest local test run:

```text
Total tests: 27
Passed: 27
Failed: 0
Errors: 0
```

## Notes

The `access_token` value is intentionally left empty in the environment file. It is generated automatically after running the login request.

## Author

Milica Mijacic
