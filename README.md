# Address-Book-using-Python

Overview:
This is a simple Address Book application developed using Python, SQLite, and Tkinter. It allows users to manage a list of contacts with their names and phone numbers. The application supports the following functionalities:

• Add a new contact
• Edit a contact's phone number
• Delete a contact
• View all contacts
• Search for a contact by name
• Reset the input fields
• Exit the application


Features:
• SQLite Database: All contacts are stored in an SQLite database.
• Validation: Phone numbers must be exactly 10 digits, and names cannot be duplicated.
• User Interface: Tkinter is used for the graphical user interface (GUI), with buttons for each function.

Requirements:
• Python 3.x
• SQLite
• Tkinter (typically included with Python)

Installation
• Clone or download the repository.
• Install the required libraries (SQLite and Tkinter are standard with most Python installations).
• Run the Python script to start the application.
• Database Structure
• Database Name: addressbook.db
• Table Name: tasks
• id: Primary key (integer)
• name: Contact name (text)
• status_id: Phone number (integer, 10 digits)

Application Functionality
1. Add a Contact
Users can add a contact with a name and phone number.
Validation ensures the name is not empty, the phone number is exactly 10 digits, and the name does not already exist in the database.
2. Edit a Contact
Users can edit the phone number of an existing contact.
The application checks if the contact exists before allowing changes.
3. Delete a Contact
Users can delete a contact by name. If the contact does not exist, a warning is shown.
4. View All Contacts
Displays all saved contacts from the database in a new window.
5. Search by Name
Users can search for a contact by name. If the contact is found, the corresponding phone number is displayed.
6. Reset Fields
Clears the input fields for name and phone number.
7. Exit Application
Closes the application.

Usage:
• Run the Script: Execute the script to launch the application.
• Add Contacts: Input a name and a 10-digit phone number, then click the "ADD" button.
• View or Edit Contacts: Use the corresponding buttons to view, search, or modify contacts.
• Exit: Click the "EXIT" button to close the application.

Code Explanation
Database Operations:

• create_connection: Establishes a connection to the SQLite database.
• create_table: Creates the tasks table if it does not exist.
• create_task: Adds a new contact to the database.
• update_task: Updates the phone number of an existing contact.
• delete_task: Deletes a contact from the database.
• select_task_by_name: Searches for a contact by name.
• select_all_tasks: Displays all contacts in a new window.

UI Components:

The GUI is built using Tkinter, with buttons for each operation (Add, Edit, Delete, View All, View by Name, Reset, Exit).
MyDialog: Displays warning messages when a contact is not found.

Notes:
Make sure that the SQLite database file (addressbook.db) is in the correct directory, as specified in the database variable.
The application performs basic validation but could be extended with more sophisticated checks or additional features like email or address fields.

Author: Nilesh Parmar https://www.linkedin.com/in/nilesh-parmar-/

License:
This project is open source and free to use.
