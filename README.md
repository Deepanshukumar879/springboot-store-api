# Spring Boot E-commerce Product API

A simple backend REST API for managing Products in an e-commerce application using **Spring Boot**.
This project demonstrates basic CRUD operations along with image upload functionality.

---

## 🧾 Features

✅ Add a new product (with image)  
✅ Get all products  
✅ Get product by ID  
✅ Update existing product (with image)  
✅ Delete a product  
✅ Search products by keyword  
✅ Fetch product image by product ID  

Images are stored as **byte[] in the database** along with type.

---

## ⚙️ Technology Stack

- Java 17
- Spring Boot
- Spring Data JPA
- PostgreSQL (or H2 for local development)
- Multipart File Upload
- REST API

---

## 🛠 Endpoints

| Method | Endpoint                       | Description                          |
|--------|--------------------------------|--------------------------------------|
| GET    | `/products`                    | Get all products                     |
| GET    | `/product/{id}`                | Get a product by ID                  |
| POST   | `/product`                     | Add a new product (with image)       |
| PUT    | `/product/{id}`                | Update product details and image     |
| DELETE | `/product/{id}`                | Delete a product by ID               |
| GET    | `/product/{id}/image`          | Get the stored image of product      |
| GET    | `/products/search?keyword=xyz` | Search products by keyword           |

---

## 📦 Product JSON Example

```json
{
  "name": "Apple iPhone 15",
  "description": "Latest iPhone with amazing features",
  "price": 79999.0,
  "category": "Electronics"
}
