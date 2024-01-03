# Loan Management System

## Overview

This project is a Flask-based web application designed for managing loans and borrowers. It provides functionalities for creating, updating, and deleting loan details, borrowers' information, and payments. The application allows employees to log in, view, and manage loan-related data.

## Technologies Used

- Flask
- SQLAlchemy
- SQLite (for development)
- HTML/CSS
- Bootstrap

## Project Structure

The project consists of the following main components:

1. **`main.py`**: This file initializes the Flask application, configures the database, and defines the routes for different functionalities. It also includes the logic for starting the application.

2. **`config.py`**: Configuration file containing settings for different environments (e.g., Local Development).

3. **`database.py`**: Defines the SQLAlchemy database and initializes it.

4. **`models.py`**: Contains the SQLAlchemy models for the Employee, Account_holders, LO_TY, LO_PL, Borrowers, and Payment entities.

5. **`templates`**: Folder containing HTML templates for different pages of the application.

6. **`static`**: Folder for storing static files such as images.

## How to Run the Project

1. Ensure you have Python installed on your machine.
2. Install the required dependencies using the following command:

    ```bash
    pip install -r requirements.txt
    ```

3. Execute the `main.py` file to start the Flask application:

    ```bash
    python main.py
    ```

4. Access the application in your web browser at `http://localhost:5000`.

## Usage Instructions

1. **Login Page (`/`):** Users can log in with their username and password. Upon successful login, the application redirects to the home page.

2. **Home Page (`/home`):** Displays an overview of the system, including the number of borrowers, loans, and other relevant information.

3. **Loans Page (`/loans`):** Allows users to create new loans, view existing loans, and make payments. Users can input borrower details, loan type, loan plan, loan amount, and purpose.

4. **Payments Page (`/payments`):** Enables users to view and manage payments made by borrowers. Users can also make new payments and see the remaining loan amounts.

5. **Borrowers Page (`/borrowers`):** Shows a list of borrowers and the number of loans associated with each borrower.

6. **Loan Types Page (`/loantypes`):** Displays information about different loan types, including their names, descriptions, interest rates, and maximum loan amounts.

7. **Loan Plans Page (`/loanplans`):** Provides details about various loan plans, such as their durations.

8. **Payments History Page (`/borrowers/<int:bor_pay_id>`):** Allows users to view the payment history of a specific borrower.
