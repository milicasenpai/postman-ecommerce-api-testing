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
- Newman
- Newman HTML Extra Reporter
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

Or run it from the command line using Newman:

```bash
newman run ecommerce-api-tests.postman_collection.json -e dummyjson.postman_environment.json
```

To generate the HTML report:

```bash
newman run ecommerce-api-tests.postman_collection.json -e dummyjson.postman_environment.json -r htmlextra --reporter-htmlextra-export newman-report.html
```

## Test Run Summary

Latest local test run:

```text
Iterations: 1
Requests: 9
Assertions: 27
Failed: 0
Errors: 0
Average response time: 143ms
```

HTML report:

```text
newman-report.html
```

## Notes

The `access_token` value is intentionally left empty in the environment file. It is generated automatically after running the login request.

DummyJSON is a public demo API. This project is intended to demonstrate API testing workflow, test coverage planning, Postman scripting, negative testing, and Newman reporting.

## Author

Milica Mijacic
