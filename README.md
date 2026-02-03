# API Testing Project — Postman (DummyJSON)

Hands-on API testing project to demonstrate REST API testing skills using Postman.

## API under test
DummyJSON Auth: https://dummyjson.com/docs/auth

## Scope
Tested endpoints:
- POST /auth/login — success (get access token)
- GET /auth/me — authorized request (Bearer token)
- POST /auth/login — negative case (invalid payload → 400)

## Artifacts
- Postman collection: [postman/collection.json](./postman/collection.json)
- Environment template: [postman/environment.example.json](./postman/environment.example.json)

## How to run
1. Import the collection and the environment into Postman
2. Select environment `qa_api_project`
3. Run requests:
   - Login - success
   - GET current auth user
   - Login - invalid payload

**Results:** 3 requests • 1 auth flow • 1 negative case