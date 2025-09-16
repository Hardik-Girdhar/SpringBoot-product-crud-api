
# Spring Boot Product CRUD API

A simple Spring Boot REST API for managing products using an H2 in-memory database. This project demonstrates basic CRUD operations with Spring Data JPA and exposes endpoints for creating, reading, updating, and deleting products.

## 🚀 Technologies Used
- Java 17
- Spring Boot
- Spring Data JPA
- H2 Database
- Maven

## 📦 Project Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/springboot-product-crud-api.git
   ```
2. Navigate to the project directory:
   ```bash
   cd springboot-product-crud-api
   ```
3. Run the application:
   ```bash
   mvn spring-boot:run
   ```
4. Access the H2 console at:
   ```
   http://localhost:8080/h2-console
   ```
   Use JDBC URL: `jdbc:h2:mem:hardik`

## 📘 API Endpoints
| Method | Endpoint            | Description              |
|--------|---------------------|--------------------------|
| GET    | `/products`         | Get all products         |
| GET    | `/products/{id}`    | Get product by ID        |
| POST   | `/products`         | Add a new product        |
| PUT    | `/products`         | Update an existing product |
| DELETE | `/products/{id}`    | Delete product by ID     |

## 📥 Sample JSON Requests
### Add Product
```json
{
  "prodName": "Laptop",
  "prodPrice": 75000
}
```

### Update Product
```json
{
  "prodId": 101,
  "prodName": "Smartphone",
  "prodPrice": 30000
}
```

## 📄 License
This project is licensed under the MIT License.
