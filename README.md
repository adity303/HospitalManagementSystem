README File for Hospital Management System Login Module
Project Overview
This project is a Login Module for a Hospital Management System, implemented in Java using the Swing framework. The application provides a graphical interface for user authentication by validating credentials from a database.

Key Features
Graphical User Interface (GUI): A user-friendly login interface built with JFrame and Swing components.
Credential Validation: Verifies username and password against stored database credentials.
Database Integration: Retrieves user details using SQL queries.
Secure Password Handling: Uses JPasswordField for masking password input.
Navigation Support: Redirects to the reception dashboard (Reception class) upon successful login.
Error Handling: Displays appropriate error messages for invalid login attempts.
Exit Option: Includes a Cancel button to close the application gracefully.
How It Works
Login Screen:

// For Login Page:
Enter Username and Password in the respective fields.
Click Login to authenticate credentials.
If valid, the application navigates to the reception dashboard.
If invalid, displays an "Invalid" error message.
Use Cancel to terminate the application.
Database Integration:

Executes a query against the login table with the input credentials.
Assumes the existence of a conn class handling database connectivity.
How to Run the Project
Clone the repository or copy the code to your local machine.
Ensure you have Java installed and set up.
Configure the conn class for database connectivity.
Set up the database table login with columns ID and PW.
Provide the correct database credentials in the conn class.
Compile and run the Login class:
bash
Copy
Edit
javac Login.java
java hospital.management.system.Login
Requirements
Java Development Kit (JDK): Version 8 or higher.
Database: MySQL or any other compatible database.
Swing Library: Bundled with JDK.
Code Highlights
GUI Components:

JTextField and JPasswordField for user input.
JLabel for labels and icons.
JButton for login and cancel actions.
Event Handling:

Implements ActionListener to manage button clicks.
SQL Query Execution:

Retrieves user data using SELECT statements.
Basic SQL query:
sql
Copy
Edit
SELECT * FROM login WHERE ID = 'username' AND PW = 'password';
Security Note:

The current implementation uses raw SQL queries, which are vulnerable to SQL Injection. It is recommended to use Prepared Statements for enhanced security.
Future Enhancements
Implement password hashing for secure credential storage.
Replace raw SQL queries with Prepared Statements.
Add validation for empty fields and username/password formats.
Enhance UI with modern libraries like JavaFX.
Implement error logging for better debugging.
Important Points from the Code
Database Connection Dependency:

Ensure the conn class is correctly implemented for database connectivity.
Event Handling:

Buttons (Login, Cancel) are configured with appropriate actions using the actionPerformed method.
Field Access and Formatting:

JTextField and JPasswordField styling ensures better user experience.
Font and Color settings make the interface visually appealing.
Icon Usage:

An image icon is included for a professional look (icon/Login.png).
Application Flow:

Successful login navigates to the Reception screen.
Invalid login triggers an error message.
Graceful Exit:

The Cancel button closes the application with an exit code.
