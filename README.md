Employee Management System (Java + Swing + MySQL)
1. Introduction

This project is a complete Employee Management System developed using Java (Swing GUI) and MySQL.
It allows organizations to efficiently manage employee information with features such as adding employees, updating employee records, viewing employee details, and removing employees from the system.
It is an excellent project for understanding Java GUI development, JDBC database connectivity, and CRUD operations.

2. Features

User login and authentication
Add new employee details
View existing employee information
Update employee data
Remove employee records
Attractive and interactive Swing-based user interface
JDBC connectivity with MySQL database

3. Technologies Used
Component	Technology
Programming Language	Java
GUI Framework	Swing, AWT
Database	MySQL
Connectivity	JDBC
IDE	IntelliJ IDEA / VS Code / Eclipse


4. Project Folder Structure
employee_management_system/
│
├── src/
│   └── employee/management/system/
│       ├── AddEmployee.java
│       ├── UpdateEmployee.java
│       ├── RemoveEmployee.java
│       ├── View_Employee.java
│       ├── Login.java
│       ├── Splash.java
│       ├── Main_class.java
│       └── conn.java
│
├── icons/
│   ├── front.gif
│   ├── home.jpg
│   ├── delete.png
│   ├── login.jpg
│   └── other images...
│
└── README.md

5. Database Setup (MySQL)
Step 1: Create Database
CREATE DATABASE employee_management;

Step 2: Create Employee Table
CREATE TABLE employee (
    emp_id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255),
    age INT,
    salary DOUBLE,
    phone VARCHAR(20),
    email VARCHAR(255),
    job VARCHAR(255)
);

Step 3: Configure Database Connection

Update the conn.java file with your MySQL username and password:

String url = "jdbc:mysql://localhost:3306/employee_management";
String username = "root";
String password = "your_password";

Step 4: Add MySQL Connector JAR

Download and add mysql-connector-j-<version>.jar to your project's classpath.

6. How to Run the Project
Method 1: Run Using IDE

Open the project in IntelliJ IDEA / VS Code / Eclipse

Add MySQL connector JAR to the project

Run the file:

Main_class.java

Method 2: Run from Terminal
javac *.java
java Main_class

7. Future Enhancements
Implement role-based access (Admin / HR) ,
Add search and filter features ,
Export employee data to Excel or PDF ,
Add attendance management module ,
Improve UI using JavaFX .

