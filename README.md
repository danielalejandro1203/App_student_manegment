# Student Management System – PyQt6

Desktop application built with **Python and PyQt6** that implements a complete **CRUD system**
(Create, Read, Update, Delete) for managing student records stored in a **MySQL database**.
The application provides a graphical interface to register, search, update, and delete students.

---

## 📌 Features

- Add new students to the database
- Display all student records in a table
- Update existing student information
- Delete student records with confirmation
- Search students by name
- MySQL database integration
- Graphical interface built with PyQt6
- Toolbar, status bar, dialogs, and message boxes

---

## 🧠 Tech Stack

- **Language:** Python  
- **GUI Framework:** PyQt6  
- **Database:** MySQL  
- **Database Connector:** mysql-connector-python  
- **Architecture:** Desktop application with dialog-based CRUD operations

---

## 🗄 Database Structure

This project expects a MySQL database named school with a table called students:
CREATE DATABASE school;

USE school;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    course VARCHAR(100),
    mobile VARCHAR(20)
);


🚀 Installation & Setup
1️⃣ Clone the repository
git clone https://github.com/danielalejandro1203/App_student_manegment.git
cd App_student_manegment

2️⃣ Create and activate a virtual environment
python -m venv venv
# Windows
venv\Scripts\activate
# macOS / Linux
source venv/bin/activate


3️⃣ Install dependencies
pip install PyQt6 mysql-connector-python

4️⃣ Configure the database connection
Edit the DatabaseConnection class in main.py if needed:

class DatabaseConnection:
    def __init__(self, host="localhost", user="root", password="your_password", database="school"):
        ...
Make sure your MySQL server is running.

5️⃣ Run the application
python main.py

## 🧪 How It Works

The main window displays all students in a table (QTableWidget)
Dialog windows handle:
1. Student insertion
2. Searching by name
3. Editing selected records
4. Deleting records with confirmation
5. All database operations are executed using MySQL queries
6. The UI updates automatically after each operation

## 📈 Learning Goals

This project was created to practice:
1. Desktop GUI development with PyQt6
2. CRUD operations with MySQL
3. Database connections in Python
4. Dialog-based UI workflows
5. Event handling and signals/slots

## 🖼️ Screens & Visualization


