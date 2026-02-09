# Student Management System – PyQt6
![Python](https://img.shields.io/badge/Python-3-blue)
![Django](https://img.shields.io/badge/Django-6-green)
![HTML](https://img.shields.io/badge/HTML5-orange)
![CSS](https://img.shields.io/badge/CSS3-blue)
![Bootstrap](https://img.shields.io/badge/Bootstrap-5-purple)
![CRUD](https://img.shields.io/badge/CRUD-✔️-yellow)
![Student Management](https://img.shields.io/badge/Management-Students-lightblue)
![Status](https://img.shields.io/badge/Status-Completed-success)


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

<img width="804" height="633" alt="image" src="https://github.com/user-attachments/assets/6b9248f6-26b9-4aa7-972e-4c4adeaa94ee" />

<img width="803" height="633" alt="image" src="https://github.com/user-attachments/assets/c6f39d60-98c1-4dc1-b23b-ff783247f198" />

<img width="802" height="630" alt="image" src="https://github.com/user-attachments/assets/39f085e4-3417-44b0-bd9a-717a5e12d5aa" />

<img width="801" height="632" alt="image" src="https://github.com/user-attachments/assets/5d06c69d-f5de-48d7-ad1b-03acf6ac8b8c" />

<img width="802" height="631" alt="image" src="https://github.com/user-attachments/assets/e9992d28-892e-4ed4-b794-a1a0702474e6" />






