# 🧩 JDBC CRUD Console Application

A simple **Java console-based CRUD project** that performs user Registration, Login, Update, and Delete operations using **MySQL JDBC**.

---

## 🚀 Features

✅ **Create** – Register a new user with name, email, password, and address  
✅ **Read** – Login and view user details  
✅ **Update** – Modify any field dynamically  
✅ **Delete** – Remove user data securely  
✅ **Validation** – Email format & password length checks  
✅ **SQL Injection Protection** – Uses `PreparedStatement`  
✅ **Auto Resource Management** – Uses `try-with-resources`  
✅ **Modular Design** – Each operation in its own class  

---

## 🧠 Tech Stack

| Technology | Description |
|-------------|-------------|
| **Java** | Core language for application logic |
| **JDBC** | Java Database Connectivity API |
| **MySQL** | Relational database |
| **Maven / JDK** | For build and compilation (optional) |

---

## 🏗️ Project Structure
com.crud.connections → Contains DB connection details,

com.crud.registration → Handles user registration,

com.crud.login → Manages login and session flow,

com.crud.update → Handles user info updates.

com.crud.delete → Deletes user account,

com.crud.datacheck → Validation utilities,



---

## ⚙️ Setup Instructions

### 1️⃣ Create Database and Table
Run these SQL commands in your MySQL terminal:

```sql
CREATE DATABASE studentsData;

USE studentsData;

CREATE TABLE stutable (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    email VARCHAR(100),
    password VARCHAR(50),
    address VARCHAR(255)
);

```

### 2️⃣ Compile and Run

Using terminal:

javac -d bin src/com/crud/**/*.java

java -cp bin com.crud.main.JDBC_CRUD_PROJECT


Or simply run JDBC_CRUD_PROJECT.java in your IDE (Eclipse / IntelliJ).

### 💻 How It Works

Registration – Stores user data in MySQL

Login – Authenticates user credentials

Update – Lets you selectively update any field

Delete – Deletes user record permanently

Loop/Navigation – After each action, user can continue or exit

### 🧾 Example Console Flow

   Registration Page
---------------------
Enter Full Name : Bruce Wayne

Enter Email : bruce@wayne.com

Enter Password : 12345

Enter Address : Gotham


✅ You are Registered Successfully

Click 1 to login or any key to exit:


---------------------
      Login Page

Enter Email : bruce@wayne.com

Enter Password : 12345


Hello Bruce Wayne

Your Details:

ID: 1

Email: bruce@wayne.com

Address: Gotham


Enter 1 to delete or 2 to update or any key to exit:

---------------------

### 🧹 Best Practices Implemented

✅ PreparedStatement for SQL injection safety

✅ .equals() for string comparison

✅ Graceful exception handling

✅ Scanner + Connection closed using try-with-resources

✅ Minimal coupling between modules


### 🏁 Author

👤 Vikram Kumar Choudhary

💼 Java & Spring Developer | DSA Enthusiast

