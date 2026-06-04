# API Testing Project — Postman (DummyJSON)

Hands-on API testing project to demonstrate REST API testing skills using Postman.

## API under test
DummyJSON Auth: https://dummyjson.com/docs/auth

## Scope
Tested endpoints:
- POST /auth/login — success (get access token)
- GET /auth/me — authorized request (Bearer token)
- POST /auth/login — negative case (invalid payload → 400)
- GET /products — list all products
- GET /products/1 — single product by ID  
- GET /products/search?q=phone — product search
- GET /auth/me without token — 401 negative case

## Artifacts
- Postman collection: [postman/collection.json](./postman/collection.json)
- Environment template: [postman/environment.example.json](./postman/environment.example.json)

## How to run
1. Import the collection and the environment into Postman
2. Select environment `qa_api_project`
3. Run requests:
   - Login - success
   - GET current auth user
   - GET all products
   - GET product by ID
   - GET products search
   - Login - invalid payload
   - Authorisation without token

**Results:** 7 requests • auth flow • products endpoints • negative cases (401, 400)