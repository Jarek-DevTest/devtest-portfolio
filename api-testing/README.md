# API Testing Project (Postman)

This repository contains two API testing modules created to demonstrate practical QA Automation skills using Postman, JavaScript test scripts, JSON Schema validation, and REST API testing techniques. Both modules include positive and negative scenarios, validation logic, and automated execution using the Postman Collection Runner.

---

## 1. CRUD Testing Module

### Scope
- Full CRUD testing (GET, POST, PUT, DELETE)
- Chaining requests using environment variables
- Dynamic data generation
- JSON Schema validation
- Negative testing (invalid payloads, missing fields, wrong methods)
- Automated execution using Collection Runner
- Test evidence (screenshots, logs)

### Structure
- postman-collection.json – main Postman collection
- schema/ – JSON Schema files
- screenshots/ – Runner results and test evidence

### Tools Used
- Postman
- REST API
- JSON Schema
- GitHub

### Status
Completed

---

## 2. Data Consistency Tests (API – SQL)

### Project Overview
This module demonstrates API testing focused on validating data consistency between an API layer and a simulated SQL data source. It includes consistency checks, positive and negative scenarios, record-level validation, response structure validation, data type validation, and JSON schema validation.

### Tech Stack
- Node.js and Express
- Postman
- JavaScript
- JSON Schema

### API Endpoints
GET /invoices?customerId=123  
Returns a list of invoices for a specific customer.

GET /invoices/:id  
Returns a single invoice by its ID.

### Test Structure
- GET Invoice – API – SQL Consistency
- GET Invoice – Negative Test
- GET Invoice by ID – Detail Test
- GET Invoice by ID – Negative Test
- GET Invoice – Data Types Validation
- GET Invoice – JSON Schema Validation
- GET Invoice – Response Structure Validation

### Test Coverage
API – SQL Consistency Test  
Validates that API data matches expected SQL data.

Negative Test  
Ensures the API returns an empty array for an invalid customerId.

Detail Test  
Validates a single record against expected SQL values.

Negative Detail Test  
Ensures the API returns 404 for a non-existing invoice ID.

Data Types Validation  
Checks that all fields have correct data types.

JSON Schema Validation  
Validates the response structure using a JSON schema.

Response Structure Validation  
Ensures all required fields exist in every returned object.

### How to Run
Install dependencies:  
npm install

Start the server:  
node server.js

Server runs at:  
http://localhost:3000

Run tests in Postman by opening the collection “Data Consistency Tests – API – SQL”.

### Skills Demonstrated
- API testing
- Positive and negative scenarios
- Data consistency validation
- JSON schema validation
- Response structure analysis
- JavaScript scripting in Postman
- REST API understanding
- Backend mock creation
- Professional test organization and naming conventions

### Summary
This module demonstrates a complete API testing workflow suitable for a QA Automation portfolio. It shows practical testing skills and the ability to validate backend data effectively.

---

## Final Notes
This repository showcases two independent API testing modules:
- CRUD testing
- Data consistency validation

Both demonstrate practical QA Automation skills and can be expanded with additional endpoints or test suites.
