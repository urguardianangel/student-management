# Student Management System

## Overview
The Student Management System is a web application developed using Node.js, Express.js, EJS, and MySQL. It allows users to manage student records and demonstrates web development, database integration, version control, and AI-assisted software development.

## Technologies Used
- Node.js
- Express.js
- EJS
- MySQL
- Git and GitHub
- AI tools for code explanation and debugging

## Features
- View student records
- Add student records
- Search for students
- Edit student information
- Delete student records
- Store student data in a MySQL database

## Requirements
- Node.js and npm
- MySQL or MariaDB
- Git
- Visual Studio Code
- XAMPP (for MySQL and phpMyAdmin, if used)

## Installation and Setup

### 1. Open the Project
Open the `student-management` folder in Visual Studio Code.

### 2. Install Dependencies

```bash
npm install
```

If you have not installed the required packages yet, run:

```bash
npm install express ejs mysql2
```

### 3. Create the Database

Open phpMyAdmin and execute the following SQL:

```sql
CREATE DATABASE student_management;

USE student_management;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    student_id VARCHAR(20) NOT NULL UNIQUE,
    first_name VARCHAR(100) NOT NULL,
    last_name VARCHAR(100) NOT NULL,
    course VARCHAR(100) NOT NULL,
    year_level INT NOT NULL,
    email VARCHAR(150) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);
```

### 4. Configure the Database
Make sure your database connection in `app.js` uses the correct host, username, password, and database name.

Database name: `student_management`

### 5. Run the Application

```bash
node app.js
```

Open your browser and visit:

`http://localhost:3000`

Keep the terminal running while using the application.

## Testing

Test the following features if they are implemented:

1. Open the student list.
2. Add a new student.
3. Search for a student.
4. Edit student information.
5. Delete a student.
6. Check how the application handles invalid input.
7. Verify that student records are saved in the database.

## Git and GitHub

Initialize Git if the project is not yet a repository:

```bash
git init
git status
```

Create a `.gitignore` file containing:

```gitignore
node_modules/
.env
```

Commit your project:

```bash
git add .
git commit -m "Initial student management system"
```

Connect your GitHub repository:

```bash
git remote add origin YOUR_REPOSITORY_URL
git branch -M main
git push -u origin main
```

Replace `YOUR_REPOSITORY_URL` with your actual GitHub repository URL. If a remote is already configured, check it using `git remote -v`.

### Feature Branch Workflow

Create a feature branch:

```bash
git checkout -b feature/student-search
```

After implementing and testing the feature:

```bash
git add .
git commit -m "Add student search feature"
git push -u origin feature/student-search
```

Create a Pull Request on GitHub to review the changes before merging them into the main branch.

## AI-Assisted Development

AI tools can help explain code, identify errors, suggest improvements, and create test cases.

Before using AI-generated suggestions:
1. Understand the suggested changes.
2. Review the code carefully.
3. Test the changes in the application.
4. Document the errors encountered and how they were resolved.
5. Never share passwords, tokens, or other confidential information.

## Troubleshooting

**Node.js is not recognized**

Install Node.js and reopen the terminal. Check the installation using `node -v` and `npm -v`.

**Database connection failed**

Make sure MySQL is running and check the database name and connection credentials.

**Cannot find module**

Run `npm install` inside the project folder.

**Port 3000 is already in use**

Stop the application using the port or configure your server to use another available port.

## Learning Outcomes

This activity provides experience in building a web application, connecting to a database, testing student management features, using Git and GitHub, and applying AI tools responsibly during software development.
