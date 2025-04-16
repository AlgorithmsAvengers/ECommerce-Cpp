# 🛒 E-commerce System

A console-based E-commerce system built with **C++** supporting **Admin and User roles**, featuring product management, secure login, shopping cart, and persistent data storage.  
This application provides a practical foundation for understanding file I/O, object management, and console interface design in C++.

---

## 📌 Project Overview

The E-commerce System is a feature-rich C++ console application designed to simulate an online shopping platform.  
It includes **user registration and login**, **product viewing and purchasing**, **admin product/inventory control**, and **data persistence** using files.  
Aimed at students or developers learning object-oriented programming and file management in C++.

---

## 🖼️ Interface Snapshots

**📋 Main Menu (Alt Text):**  
![image](https://github.com/user-attachments/assets/bdeb4031-3d06-4a2f-a6d4-35f406a9df34)
Main interface showing role selection (Admin or User), login prompts, and navigation options for product, cart, and order management.

**💼 Admin Dashboard (Alt Text):**  
![image](https://github.com/user-attachments/assets/ca69a3af-9ba9-44b2-9a84-b03c3ef796b1)
Console interface displaying admin functions like adding products, viewing orders, changing passwords, and checking site funds.

**🛍️ User Menu (Alt Text):**  
![image](https://github.com/user-attachments/assets/d30e0ed9-f0d0-445c-92ae-37feb6860e63)

User screen with product listings, shopping cart access, and order history.

---

## ❓ Features & Functionality

### 👤 User Features

- 📝 **Registration** with username, password, and email  
- 🔐 **Login** with password and email validation  
- 🛍️ **Product browsing** with details  
- 🧺 **Cart management** (add/remove/view items)  
- 💸 **Order placement**  
- 📜 **View order history**

### 🛠️ Admin Features

- 🔐 Secure admin login  
- 💰 View and withdraw **site balance**  
- 🔑 Change **admin password**  
- 📦 Add and update **product inventory**  
- 📄 View all orders and mark as delivered

---

## ⚙️ Key Functionalities

- 🗂️ **File Initialization**: Automatically creates files for products, users, orders, and admins if missing
- 📤 **Product Handling**: Load, display, save product info
- 📧 **Email & Password Validation**: Ensures strong and valid credentials
- 💾 **Data Persistence**: Uses file I/O for saving users, products, and orders
- 🎨 **Console Feedback**: Includes visual enhancements like loading animations and console color changes

---

## 🧠 Code Structure Overview

### 🧱 Core Components

- `struct User` / `struct Product` / `struct Order` – Data models  
- `registerUser()` – Handles new user signups  
- `loginUser()` / `loginAdmin()` – Authenticates users/admins  
- `addProduct()`, `viewProducts()` – Product CRUD operations  
- `addToCart()`, `removeFromCart()`, `checkout()` – Cart functions  
- `saveData()`, `loadData()` – File operations  
- `viewOrders()`, `markOrderShipped()` – Admin order management  
- `changePassword()`, `withdrawFunds()` – Admin utilities

---

## 🧮 Data Types Used

- 🧱 Structs: For user, product, and order records  
- 🗃️ Linked Lists: Used instead of arrays for product storage
- 🧱 Priority Queues: For Premium Users.
- 🔤 Strings: Usernames, passwords, emails, product names  
- 📂 File Streams: For reading/writing data persistently  
- 🏷️ Enums / Flags: Used for user roles and order status

---

## ⚖️ Design Decisions

| Feature                 | ✅ Pros                                              | ⚠️ Cons                                     |
|--------------------------|------------------------------------------------------|----------------------------------------------|
| File-based persistence   | Simple, fast, and easy to debug                      | Not suitable for scaling to large data       |
| Role-based system        | Clear separation of privileges                       | Requires more validation logic               |
| Console-based UI         | Lightweight and accessible                          | Limited UX / no GUI                          |
| Validation functions     | Prevent bad data and increase security               | Slightly more complex input logic            |
| Linked list for products | Efficient dynamic memory usage                       | More overhead than vectors                   |

---

## 🚀 Getting Started

### 📦 Prerequisites

- ✅ C++ compiler (C++11 or later)
- ✅ Console/terminal environment

### 🔮 Future Enhancements
- 🛂 Role-based product filtering (VIP, discounted)
- 🧾 PDF invoice generation
- 🔎 Search and filter products
- 📈 Sales statistics and analytics
- 🌐 Export/import data to JSON/CSV
- 👥 Multi-admin support
- 💬 Chat-like customer support simulation

### ▶️ How to Run

1. **Compile the code**:

   ```bash
   g++ ecommerce_system.cpp -o ecommerce_system
