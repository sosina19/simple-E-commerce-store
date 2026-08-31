# Simple E-commerce Store

A basic full-stack e-commerce web application where users can browse products, view product details, add products to a shopping cart, create an account, log in, and place orders.

## 📌 Project Overview

This project is being built as a simple e-commerce system to demonstrate the fundamentals of full-stack web development.

The application has three main parts:

* **Frontend** — HTML, CSS, and JavaScript
* **Backend** — Django and Python
* **Database** — PostgreSQL

The main flow of the application is:

```text
User
  ↓
Frontend
  ↓
Django Backend
  ↓
Database
```

The frontend is responsible for displaying information and interacting with the user. Django handles the application's logic and communicates with the database. The database stores persistent information such as products, users, and orders.

---

## 🎯 Project Objectives

The application should allow a customer to:

* Browse available products
* View detailed information about a product
* Add products to a shopping cart
* Remove products from the cart
* Change product quantities
* Create a user account
* Log in and log out
* Proceed to checkout
* Place an order
* View previous orders

The system should also allow an administrator to manage products and orders through Django's admin interface.

---

## ✨ Main Features

### 1. Product Listing

Users can view all available products.

Each product should contain information such as:

* Product name
* Product image
* Description
* Price
* Available stock

### 2. Product Details

Users can select a product to view its full information.

### 3. Shopping Cart

Users can:

* Add products
* Remove products
* Increase quantity
* Decrease quantity
* View the total price

### 4. User Authentication

Users can:

* Register
* Log in
* Log out

Authentication will use Django's built-in authentication system.

### 5. Checkout

Users can review their cart and submit an order.

### 6. Order Processing

When an order is submitted, the system stores:

* The user who placed the order
* The products ordered
* The quantity of each product
* The price at the time of purchase
* The total order price
* The order status
* The date the order was created

### 7. Order History

Logged-in users can view their previous orders.

### 8. Admin Management

Administrators can use Django Admin to:

* Add products
* Edit products
* Delete products
* View orders
* Update order status

---

## 🗄️ Database

The application will use a relational database.

The main data will include:

```text
Users
Products
Orders
Order Items
```

### User

Represents a customer using the system.

### Product

Represents an item available for purchase.

Example:

```text
Product
------------------
Name: Wireless Mouse
Price: 20.00
Stock: 25
```

### Order

Represents a completed checkout request made by a user.

Example:

```text
Order
------------------
User: sosi
Total: 70.00
Status: Pending
```

### Order Item

Represents a specific product inside an order.

Example:

```text
Order Item
------------------
Product: Mouse
Quantity: 2
Price: 20.00
```
---

## 🔄 Application Flow

The basic customer flow is:

```text
Visit Website
     ↓
View Products
     ↓
View Product Details
     ↓
Add Product to Cart
     ↓
View Cart
     ↓
Login / Register
     ↓
Checkout
     ↓
Place Order
     ↓
Order Saved in Database
     ↓
View Order History
```

---

## 🛠️ Technologies

| Technology | Purpose                      |
| ---------- | ---------------------------- |
| HTML       | Web page structure           |
| CSS        | Web page styling             |
| JavaScript | Frontend behavior            |
| Python     | Backend programming language |
| Django     | Backend web framework        |
| PostgreSQL | Relational database          |
| Git        | Version control              |

---

## 🚧 Development Plan

The project will be developed gradually.

### Phase 1 — Project Setup

* Create project repository
* Create Python virtual environment
* Install Django
* Create Django project
* Create Django app
* Configure database

### Phase 2 — Database

* Create Product model
* Create Order model
* Create OrderItem model
* Run migrations
* Configure Django Admin

### Phase 3 — Products

* Create product listing
* Create product details page
* Add product images
* Display stock and price

### Phase 4 — Authentication

* User registration
* User login
* User logout
* Protect authenticated pages

### Phase 5 — Shopping Cart

* Add product to cart
* Remove product
* Update quantity
* Calculate total

### Phase 6 — Orders

* Create checkout page
* Create orders
* Create order items
* Update product stock
* Display order history

### Phase 7 — Frontend

* Improve layout
* Add responsive design
* Add JavaScript interactions
* Improve user experience

### Phase 8 — Testing

* Test registration
* Test login
* Test product browsing
* Test cart functionality
* Test checkout
* Test order creation
* Test stock handling
* Test unauthorized access

---

## 🔐 Security Considerations

The application should:

* Never store passwords as plain text
* Use Django's authentication system
* Validate user input
* Protect authenticated routes
* Use CSRF protection for forms
* Keep database credentials and secret keys out of Git
* Store sensitive configuration in environment variables

---

## 📚 Learning Goals

This project is intended to help understand:

* Frontend and backend communication
* Django project structure
* Django applications
* URL routing
* Views
* Templates
* Models
* Database relationships
* Migrations
* Authentication
* Sessions
* Shopping carts
* Order processing
* CRUD operations
* Git and GitHub
* Basic web security

---

## 🚀 Future Improvements

Possible improvements after the basic version is complete:

* Product categories
* Product search
* Product filtering
* Pagination
* Reviews and ratings
* Wishlist
* Payment integration
* Email notifications
* REST API
* React frontend
* Docker deployment

---

## 📄 License

This project is for educational purposes.
