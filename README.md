# EXPANSE-TRACKER-MANAGER
An expense tracker is a software or application using python tkinter that helps to keep an accurate record of your money inflow and outflow. Many people in India live on a fixed income, and they find that towards the end of the month they don’t have sufficient money to meet their needs. While this problem can arise due to low salary, invariably it is due to poor money management skills. Using a daily expense manager can help you keep track of how much you spend every day and on what.
Benefits of Using Daily Money Manager:-Prioritize Your Spending,· Become Aware of Poor Spending Habits,Identify Fraud,Take Control of Your Finances, Saving and Investment.


Overview:
1.	Main Application (Expanse Manager):
o	Title: "Expanse Manager"
o	Geometry: 1366x768
o	The application starts with a main window (project) that allows users to either log in or sign up.
o	It includes functionality for forgotten passwords (forgot function).

2.	Sign Up (signup function):
o	Opens a new window (new_project) for user registration.
o	Collects user details like first name, last name, email, occupation, mobile number, security question, and password.
o	Provides a security question and answer option for password recovery.
o	Validates and inserts these details into a MySQL database (PROJECT).
3.	Forgot Password (forgot function):
o	Opens a new window (f_project) for resetting passwords.
o	Requires users to provide their email, mobile number, new password, and confirm the new password.
o	Updates the password in the MySQL database after validation.

4.	Login (login function):
o	Checks if the entered email and password match records stored in a MySQL database (PROJECT).
o	If successful, opens a new window (main_window) for managing expenses.
o	Allows showing total debit and credit balances, adding credit and debit details, and displaying detailed credit and debit information.
o	Uses tkinter widgets like Label, Entry, Button, Text, and Combobox for user input and display.
o	Database operations (SELECT, INSERT, UPDATE) are performed using MySQL Connector (mysql.connector).

5.	Expense Management (main_window functions):
o	Provides options to add credit and debit details.
o	Shows total debit and credit balances.
o	Includes functionality to display detailed credit and debit information from the MySQL database (CREDIT and DEBIT tables).

6.	Database Connection:
o	Connects to MySQL database running locally (localhost).
o	User credentials and database name are provided within the script.
o	Uses mysql.connector for executing SQL queries (SELECT, INSERT, UPDATE) against the database.
