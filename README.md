# 🛒 Ecommerce API — Laboratory 7

**HTTP Fundamentals and Spring Boot**

---

## 📌 Overview

This project implements a **RESTful API backend** for an e-commerce system using **Spring Boot**.
It demonstrates the use of **HTTP methods, status codes, headers, and REST principles** with an **in-memory data store**.

---

## 🎯 Objectives

* Build a RESTful API using Spring Boot
* Implement CRUD operations for products
* Apply proper HTTP methods and status codes
* Use Java Collections Framework (`List<Product>`)
* Follow layered architecture (Controller → Service → Model)

---

## ⚙️ Tech Stack

* Java 21+
* Spring Boot 4.x
* Spring Web
* Lombok
* Maven / Gradle Wrapper

---

## 📁 Project Structure

```
com.ws101.dizoncolele.EcommerceApi
│
├── controller     # Handles HTTP requests
├── service        # Business logic
├── model          # Data entities
└── EcommerceApiApplication.java
```

---

## 🧩 Product Model

The `Product` class includes:

* `id` (Long)
* `name` (String)
* `description` (String)
* `price` (double)
* `quantity` (int)

---

## 🔄 API Endpoints

### 🔹 Base URL

```
http://localhost:8080/api/products
```

---

### ✅ GET All Products

```
GET /api/products
```

**Response:** `200 OK`

---

### ✅ GET Product by ID

```
GET /api/products/{id}
```

* `200 OK` (found)
* `404 NOT FOUND` (not found)

---

### ✅ CREATE Product

```
POST /api/products
```

**Headers:**

```
Content-Type: application/json
```

**Body Example:**

```json
{
  "name": "Laptop",
  "description": "Gaming Laptop",
  "price": 50000,
  "quantity": 5
}
```

**Response:** `201 CREATED`

---

### ✅ UPDATE Product

```
PUT /api/products/{id}
```

**Response:**

* `200 OK` (updated)
* `404 NOT FOUND`

---

### ✅ DELETE Product

```
DELETE /api/products/{id}
```

**Response:**

* `204 NO CONTENT`
* `404 NOT FOUND`

---

## 📡 HTTP Methods Used

| Operation | Method |
| --------- | ------ |
| Create    | POST   |
| Read      | GET    |
| Update    | PUT    |
| Delete    | DELETE |

---

## 📊 HTTP Status Codes

| Code | Meaning     |
| ---- | ----------- |
| 200  | OK          |
| 201  | Created     |
| 204  | No Content  |
| 404  | Not Found   |
| 400  | Bad Request |

---

## 🧠 Key Concepts Applied

* RESTful API design
* Layered architecture
* In-memory data storage
* HTTP request/response handling
* JSON serialization/deserialization

---

## ▶️ How to Run

1. Open project in IDE
2. Run:

```
EcommerceApiApplication.java
```

3. Access API:

```
http://localhost:8080/api/products
```

---

## 🧪 Testing

Use:

* Postman
* Browser (GET only)
* Curl

---

## 🔀 Version Control (Git)

```bash
git init
git checkout -b feat:lab7

git add .
git commit -m "feat(lab7): implement REST API with CRUD operations"
git push origin feat:lab7
```

---

## 👥 Pair Programming

This project was completed using **pair programming**:

* Driver: Writes code
* Navigator: Reviews and suggests improvements
* Roles switched after each task

---

## 📌 Notes

* Data is stored **in-memory only** (not persistent)
* Server runs on **port 8080**
* Restarting the app resets all data

---

## ✅ Status

✔ Project initialized
✔ CRUD API implemented
✔ HTTP standards applied
✔ Tested successfully

---

## 👤 Author

**Dizon,JudyMarie A.
Colele,Shella
**Course:** WS101

---
