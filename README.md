# Student Management System

A simple web-based Student Management System developed using:

- Node.js
- Express.js
- EJS
- MySQL
- Git
- GitHub

## Features

- View students
- Add students
- Search students
- (Coming soon) Edit students
- (Coming soon) Delete students
- (Coming soon) Form validation

## Installation

Clone the repository:

    git clone https://github.com/urguardianangel/student-management.git

Install dependencies:

    npm install

Create the database:

1. Start Apache and MySQL in XAMPP.
2. Open phpMyAdmin and run the SQL script that creates the `student_management` database and `students` table.

Configure the database connection in `app.js` (host, user, password, database).

Run:

    node app.js

Open:

    http://localhost:3000