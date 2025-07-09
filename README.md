# 🛒 Online Shopping System

A simple full-stack shopping system built using:

- Java 17
- Spring Boot 3.5.2
- MySQL (for database)
- HTML + JavaScript (for frontend)

---

## 📁 Project Structure
online-shopping-system/
├── frontend/
│ ├── index.html # Customer UI
│ └── admin.html # Employer/Admin UI
├── src/main/java/... # Spring Boot source code
├── src/main/resources/
│ ├── application.properties
├── .gitignore
├── pom.xml
├── README.md


---

## 💡 Features

### 👤 Customer (`index.html`)
- View available products
- Add items to cart
- View cart and total
- Buy (simulated checkout)

### 🧑‍💼 Employer/Admin (`admin.html`)
- Add new products
- Edit existing products
- Delete products

---

## 🧱 Technologies Used

- Java 17
- Spring Boot 3.5.2
- Spring Data JPA
- MySQL
- HTML + JS 
- Maven

---

## 🧰 Setup Instructions

### ✅ 1. Clone the Project

git clone https://github.com/azwad1/online-shopping-system.git
cd online-shopping-system

### 2. MySQL Setup

CREATE DATABASE shopping_db;

### 3. Configure application.properties

In src/main/resources/application.properties:
spring.datasource.url=jdbc:mysql://localhost:3306/shopping_db
spring.datasource.username=root
spring.datasource.password=root

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true


### ✅ 4. Run Spring Boot App

mvn spring-boot:run
The app will run at:
📍 http://localhost:8080

### 🌐 Frontend Usage
Open the files in a browser:

frontend/index.html → for customer

frontend/admin.html → for employer/admin

### ✅ Make sure the backend is running to allow communication.

### 🧪 API Endpoints
Method	Endpoint	Description
GET	/products	List all products
POST	/products	Add a new product
PUT	/products/{id}	Update a product
DELETE	/products/{id}	Delete a product

Test using Postman or the frontend UI.

 ### 🧠 Sample Cart Flow (index.html)
Load the product list

Click Add to Cart

View selected items and total

Click Buy → shows a simple alert


### 🙋 Author
GitHub: azwad1

Built as a learning/student-level project

### 📄 License
This project is open for educational use.


---
