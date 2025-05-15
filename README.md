# 🛠️ E-Commerce Product Catalog - Backend

This is the **backend** of the E-Commerce Product Catalog built using **Spring Boot**, **Hibernate**, and **MySQL**.

---

## 📁 Project Structure

```
backend/
├── src/
│   ├── main/java/com/example/catalog/
│   │   ├── controller/ProductController.java
│   │   ├── model/Product.java
│   │   ├── repository/ProductRepository.java
│   │   ├── service/ProductService.java
│   │   └── CatalogApplication.java
│   └── main/resources/application.properties
├── pom.xml
```

---

## 📦 Dependencies

Add these dependencies in Spring Initializr:

* Spring Web
* Spring Data JPA
* MySQL Driver
* Spring Boot DevTools (optional)

---

## ⚙️ application.properties

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/productdb
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL5Dialect
```

---

## 🧪 Sample Product JSON (for POST request)

```json
{
  "name": "Smart Watch",
  "description": "Fitness tracking smartwatch",
  "price": 2999.0,
  "category": "Electronics"
}
```

Include header: `role: admin`

---

## 🔄 REST Endpoints

| Method | Endpoint       | Description          | Access     |
| ------ | -------------- | -------------------- | ---------- |
| GET    | /products      | Get all products     | Public     |
| GET    | /products/{id} | Get product by ID    | Public     |
| POST   | /products      | Add product          | Admin only |
| DELETE | /products/{id} | Delete product by ID | Admin only |

---

## 🧑‍💻 Technologies Used

* Java 17
* Spring Boot
* Spring Data JPA (Hibernate)
* MySQL
* Maven

---

## ▶️ How to Run

1. Create a MySQL database `productdb`.
2. Update credentials in `application.properties`.
3. Run the Spring Boot application:

   ```bash
   ./mvnw spring-boot:run
   ```

Backend runs at: [http://localhost:9090](http://localhost:9090)

---


