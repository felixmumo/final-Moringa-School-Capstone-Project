# final-Moringa-School-Capstone-Project
Well Styled CRUD system for Registering students.
🎓 Capstone: AI-Powered Technology Learning Toolkit
👩🏽‍💻 Felix Musyoka Mumo
🎓 Student Registration CRUD System

AI-Assisted Development of a Flask + MySQL Web Application

📍 Overview

This capstone explores how Generative AI accelerated my learning and refinement of backend web development using Flask (Python) and MySQL (XAMPP).

The project demonstrates:

Flask routing and request handling

MySQL database integration

CRUD (Create, Read, Update, Delete) operations

HTML template rendering

Form handling and validation

Backend–database communication

AI was used to:

Refine database connection logic

Improve CRUD query structure

Debug MySQL connector issues

Optimize Flask routes

Enhance error handling

🎯 Project Goal

To build a fully functional Student Registration CRUD Web Application using Flask and MySQL (XAMPP), while documenting how AI supported the backend development and debugging process.

This project connects a real MySQL database and performs live CRUD operations.

🛠 Technology Stack
Technology	Purpose
Python	Backend programming
Flask	Web framework
MySQL	Relational database
XAMPP	Local Apache & MySQL server
HTML	Frontend templates
Jinja2	Template rendering
📦 Deliverables
python-flaskcrud-student-registration-project/
├── README.md
├── app.py
├── templates/
│   ├── index.html
│   ├── add.html
│   └── edit.html

Your full project is contained in:

app.py

🚀 Quick Start
1️⃣ Clone Repository
git clone https://github.com/felixmumo/python-flaskcrud-student-registration-project.git
cd python-flaskcrud-student-registration-project

2️⃣ Start XAMPP

Start Apache

Start MySQL

3️⃣ Create Database

Open:

http://localhost/phpmyadmin


Run:

CREATE DATABASE student_db;

USE student_db;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100) NOT NULL,
    email VARCHAR(100) NOT NULL,
    course VARCHAR(100) NOT NULL
);

4️⃣ Install Dependencies

Create virtual environment (optional but recommended):

python -m venv venv
venv\Scripts\activate   # Windows


Install requirements:

pip install flask mysql-connector-python

5️⃣ Configure Database Connection

Inside app.py:

db = mysql.connector.connect(
    host="localhost",
    user="root",
    password="",
    database="student_db"
)

6️⃣ Run the Application
python app.py


Open browser:

http://127.0.0.1:5000/

💡 Project Features
📋 Student Registration System

Add new student records

View all students in table format

Edit student information

Delete students

Real-time MySQL database updates

🗄 CRUD Functionality
➕ Create

Insert new student into MySQL database.

📖 Read

Retrieve and display all students.

✏ Update

Modify student details using ID.

❌ Delete

Remove student record permanently.

🔁 Backend Logic Overview

The core system runs inside:

add_student()

update_student(id)

delete_student(id)

index()

Example Insert Logic:

cursor.execute(
    "INSERT INTO students (name, email, course) VALUES (%s, %s, %s)",
    (name, email, course)
)
db.commit()


Expected Behavior:

Submit form

Data saved to MySQL

Redirect to homepage

Table updates automatically

🧠 What I Learned

Through AI-assisted prompting, I learned:

How Flask connects to MySQL

How to use mysql.connector

Writing parameterized SQL queries

Preventing SQL injection

Using Jinja2 templates

Handling form submissions

Debugging database errors

Structuring backend projects properly

🤖 AI Prompt Journal ✨
Prompt	AI Response Summary	Helpfulness
"How do I connect Flask to MySQL using XAMPP?"	Provided connector setup example	⭐⭐⭐⭐⭐
"Fix MySQL access denied error"	Explained root password issue	⭐⭐⭐⭐
"Show CRUD structure in Flask"	Provided route-based example	⭐⭐⭐⭐⭐
"How to prevent SQL injection?"	Introduced parameterized queries	⭐⭐⭐⭐⭐
"Why is my template not rendering?"	Explained Flask template folder structure	⭐⭐⭐⭐
🐞 Common Issues & Fixes
Issue	Cause	Fix
MySQL not connecting	Server not running	Start MySQL in XAMPP
Access denied for user	Incorrect credentials	Verify root password
ModuleNotFoundError	Package not installed	Run pip install
Page not updating	Missing redirect	Use redirect() after commit
Template not found	Wrong folder structure	Use templates/ folder
📊 Reflection on AI’s Role

AI significantly accelerated:

Backend structuring

SQL query formulation

Debugging connector errors

Improving route organization

Understanding CRUD patterns

However:

Manual testing was required

Database configuration needed verification

Some syntax errors required debugging beyond AI suggestions

AI served as:

A development assistant that enhanced learning speed while requiring validation and testing.

📚 References

Flask Documentation

MySQL Documentation

mysql-connector-python Docs

MDN Web Docs

XAMPP Official Guide

💎 Project Strengths

✔ Functional full CRUD system
✔ Real database integration
✔ Clean route structure
✔ Secure SQL queries
✔ Beginner-friendly implementation
✔ AI-assisted documentation

Built With AI Assistance

This project demonstrates how structured prompting can accelerate backend development and deepen understanding of full-stack web application architecture.

© 2026 Felix Mumo
Moringa School Capstone Project
