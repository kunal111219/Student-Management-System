# Student Management System

## Overview

The Student Management System is a desktop application built using Python's Tkinter library for the graphical user interface (GUI) and MySQL for the backend database. This application allows users to manage student records, including adding, updating, deleting, and searching student data.

## Features

- **Add Student**: Allows users to add new student records.
- **Update Student**: Enables users to update existing student records.
- **Delete Student**: Provides functionality to remove student records.
- **Search Student**: Allows users to search for student records based on Roll Number, Name, or Contact.
- **View All Students**: Displays all student records in a table format.

## Requirements

- Python 3.x
- `mysql-connector-python` library
- Tkinter (included with standard Python distributions)

## Installation

1. **Install MySQL Connector**

    You can install the MySQL Connector using pip:

    ```bash
    pip install mysql-connector-python

2. **Set Up the MySQL Database**

    Ensure that you have MySQL installed and running. Create a database named `{Your Database name}` and a table named `students` with the following structure:

    ```bash
    CREATE TABLE students (
    Roll_No VARCHAR(50) PRIMARY KEY,
    Name VARCHAR(100),
    Email VARCHAR(100),
    Gender VARCHAR(10),
    Contact VARCHAR(15),
    DOB DATE,
    Address TEXT
    );
    ```

## Usage

1. **Clone the Repository**

    ```bash
    git clone https://github.com/username/Student-Management-System.git
    cd Student-Management-System


2. **Run the Script**

    Execute the script to manage hotel and user data:

    ```bash
    python Student_Management_System.ipynb

3. **Interact with the Application**

    - **Add**: Enter student details and click "Add" to insert a new record into the database.
    - **Update**: Select a student record from the table, modify the details, and click "Update" to save changes.
    - **Delete**: Select a student record and click "Delete" to remove it from the database.
    - **Clear**: Click "Clear" to reset the input fields.
    - **Search**: Use the search functionality to find specific student records.
    - **Show All**: Display all student records in the table.

## Code Overview

- **Student Class**: Handles the main application functionality including GUI creation, database operations, and event handling.
- **add_students()**: Adds new student records to the database.
- **fetch_data()**: Fetches and displays all student records from the database.
- **clear()**: Clears the input fields.
- **get_cursor()**: Fetches and displays the selected student record from the table.
- **update_data()**: Updates existing student records.
- **delete_data()**: Deletes student records from the database.
- **search_data()**: Searches for student records based on user input.

## Acknowledgments

- `Python` and `Tkinter` for GUI development.
- `MySQL` for database management.

## Contributing

Feel free to contribute to this project by submitting issues or pull requests. For major changes, please open an issue first to discuss what you want to change.

## Contact

For any questions or feedback, please reach out to <rastogikunal19@gmail.com>.
