# E-commerce Product Management System

This is a simple Spring Boot project that demonstrates logging and exception handling. The project manages products in an e-commerce system.

## Features
- Add a product
- Fetch all products
- Fetch a product by ID
- Global exception handling
- Logging using SLF4J with Logback

## Folder Structure
```
src/
└── main/
    ├── java/
    │   └── com/example/ecommerce/
    │       ├── controller/
    │       ├── service/
    │       ├── repository/
    │       ├── entity/
    │       └── exception/
    └── resources/
        ├── application.properties
        └── logback-spring.xml
```

## How to Run
1. Clone this repository.
2. Navigate to the project directory.
3. Run the application using:
   ```
   mvn spring-boot:run
   ```
4. Use tools like Postman to test APIs:
   - `GET /products` - Fetch all products.
   - `GET /products/{id}` - Fetch product by ID.
   - `POST /products` - Add a product.

## Logging
- Logs are configured using Logback.
- Logs can be viewed in the console.

## Example API Request
**Add a Product**
```json
POST /products
{
  "name": "Laptop",
  "description": "Gaming Laptop",
  "price": 1200.0
}
```

**Response**
```json
{
  "id": 1,
  "name": "Laptop",
  "description": "Gaming Laptop",
  "price": 1200.0
}
```
