# 🛒 E-commerce Project (H2 Database)

This is a simple E-commerce web application built using **Spring Boot**, **H2 Database**, and optionally a **React.js frontend**. The backend manages products, categories, and inventory using RESTful APIs and persists data in an in-memory H2 database.

## 🚀 Features

- RESTful API for managing products
- In-memory H2 database for quick development and testing
- Spring Boot for backend API
- (Optional) React.js frontend for product listing
- JPA/Hibernate for ORM
- Auto-generated database schema from entities

## 🛠 Tech Stack

- Java 17+
- Spring Boot
- Spring Data JPA
- H2 Database
- Maven
- (Optional) React.js

## ⚙️ Installation & Run

### Backend (Spring Boot)

1 Access the H2 Console

URL: http://localhost:8080/h2-console

JDBC URL: jdbc:h2:mem:testdb

Username: sa

Password: (leave blank or as configured)

2 API Endpoints
Method	Endpoint	Description
GET	/api/products	List all products
GET	/api/products/{id}	Get product by ID
POST	/api/products	Add a new product
PUT	/api/products/{id}	Update product
DELETE	/api/products/{id}	Delete product

4 Product Entity 
private int id;
private String name;
private String desc;
private BigDecimal price;
private String category;
private Date releaseDate;
private boolean available;
private int quantity;



Notes
H2 is an in-memory database; data resets on server restart.

Use data.sql or CommandLineRunner to preload sample data.

Add proper validation and exception handling for production.

For the data upload can use file or POSTMAN ,   getting annotations right for the layers and apis.
git clone https://github.com/yourusername/ecom-h2-springboot.git
cd ecom-h2-springboot
