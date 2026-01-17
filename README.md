# Student Management System

A robust and scalable web application built with **Spring Boot 3.3.5** to manage student records. This project uses **Spring Data JPA** for data persistence, **MySQL** as the database, and **Thymeleaf** for a dynamic front-end.

---

## 🚀 Features
* **Full CRUD Support:** Create, Read, Update, and Delete student profiles.
* **Database Integration:** Persistent storage using MySQL.
* **Responsive UI:** Server-side rendering with Thymeleaf templates.
* **Live Reload:** Uses Spring DevTools for instant feedback during development.

---

## 🛠️ Tech Stack & Dependencies

This project is configured with the following dependencies in the `pom.xml`:

* **Java 21**
* **Spring Boot Starter Web**: For RESTful APIs and web infrastructure.
* **Spring Data JPA**: For database interaction and Hibernate support.
* **Thymeleaf**: The template engine for rendering HTML.
* **MySQL Connector/J**: The JDBC driver to connect to MySQL.
* **Spring Boot DevTools**: For faster development (auto-restart).
* **Spring Boot Starter Test**: For unit and integration testing.

---

## ⚙️ Configuration (`application.properties`)

To get the application running, create a database in MySQL named `student_db` and update your `src/main/resources/application.properties` as follows:

```properties
# Database connection settings
spring.datasource.url=jdbc:mysql://localhost:3306/student_db?useSSL=false&serverTimezone=UTC
spring.datasource.username=root
spring.datasource.password=your_password_here

# Hibernate/JPA settings
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect

# Thymeleaf settings
spring.thymeleaf.cache=false
