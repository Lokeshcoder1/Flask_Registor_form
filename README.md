This project is a Flask-based user registration system using MySQL for data storage and Bcrypt for secure password handling. It provides a clean user interface with HTML templates and custom CSS styling.

**Project Overview**
This web application allows users to register with a username, email, and password. 
It validates user input, hashes passwords for security, displays helpful messages to users, and stores registration data in a MySQL database.
**File Explanations**
*app.py*
1.The main backend code written in Flask.
2.Handles routing for registration (/register), home (/), and login (/login) pages.
3.Integrates MySQL for storing user data; connection configuration is included.
4.Uses Bcrypt to hash passwords before storing, ensuring they are never saved as plain text.
5.Implements input validation: checks if fields are empty, usernames/emails already exist, email formatting, and password matching.
6.Displays feedback messages to users after registration attempts.

*layout.html*
1.Acts as the base template for the application.
2.Ensures consistent structure and styling for all pages by including common HTML components.

*register.html*
1.The HTML template for the registration form.
2.Includes fields for username, email, password, and password confirmation.
3.Displays success/error messages passed from Flask.

*style.css*
1.Provides custom styling for the application's frontend.
2.Styles the form container, input fields, labels, buttons, and feedback messages.
3.Ensures the interface appears modern, user-friendly, and responsive.

**Features**
1.User Registration: Users fill out a form with strict validation, preventing duplicate accounts and enforcing format requirements.
2.Password Security: Passwords are securely hashed using Bcrypt; actual passwords are never stored in the database.
3.User Feedback: Success and error messages guide users through the registration process and highlight any mistakes in form input.
4.Frontend Design: Responsive and visually clear layout thanks to custom CSS, making the registration experience pleasant and intuitive.

**How It Works**
1.User visits the home page and is redirected to the /register form.
2.Upon form submission, backend checks all inputs for validity using regular expressions and database queries.
3.If all checks pass, the password is hashed and the new user is added to the database.
4.If registration is successful, the user is redirected to a login page; otherwise, appropriate error messages are displayed.

**Technologies Used**
1.Flask: Lightweight web framework for Python.
2.Flask-MySQLdb: MySQL integration for data storage.
3.Flask-Bcrypt: Cryptographically secure password storage.
4.HTML/CSS: Frontend layout and styling.

This project is an ideal starting point for learning how to build secure, database-driven web applications with Python and Flask
