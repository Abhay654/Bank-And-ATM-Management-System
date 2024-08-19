# Bank & ATM Management System in C++

## Overview

This project is a terminal-based Bank & ATM Management System implemented in C++. The system allows for a variety of banking operations such as user account management, deposit, withdrawal, funds transfer, bill payment, and ATM functionalities. The project makes use of Object-Oriented Programming (OOP) principles, file handling for data persistence, and basic UI functions using the console.

## Features

### 1. **Bank Management**
   - **New User Registration**: Allows the creation of a new bank account.
   - **Existing User Management**: Facilitates login for existing users.
   - **Deposit Funds**: Users can deposit funds into their accounts.
   - **Withdraw Funds**: Allows withdrawal of funds from user accounts.
   - **Fund Transfer**: Users can transfer funds between accounts.
   - **Bill Payment**: Users can pay bills directly from their account.
   - **User Search**: Allows searching for user information based on the user ID.
   - **Edit User Details**: Users can update their personal information.
   - **Delete User Account**: Provides the option to delete a user account.
   - **View All Records**: Displays all user accounts and details.
   - **View Payment Records**: Shows all bill payments made.

### 2. **ATM Management**
   - **User Login & Check Balance**: Allows users to login and check their account balance via an ATM interface.
   - **Withdraw Funds**: Provides the functionality to withdraw money using the ATM.
   - **Account Details**: Users can view their account details.

## Techniques Used

### 1. **Object-Oriented Programming (OOP)**
   - **Classes and Objects**: The `bank` class encapsulates all the functionalities related to banking operations. This class contains private attributes for storing user information and public methods for interacting with these attributes.
   - **Encapsulation**: Data members such as `balance`, `id`, `pass`, etc., are kept private to ensure they are only accessible through public methods, providing security and integrity of the data.
   - **Function Overloading**: The class includes various member functions that serve different functionalities within the banking and ATM system.

### 2. **File Handling**
   - **File Streams**: The system uses file streams (`fstream`) to read from and write to files, ensuring that user data is saved persistently even after the program terminates.
   - **Data Storage**: User data is stored in text files (`bank.txt` and `bill.txt`), enabling the storage and retrieval of records such as user details and transaction histories.
   - **File Manipulation**: The system handles various file operations such as appending new records, editing existing records, and removing or renaming files during updates or deletions.

### 3. **Console Input/Output**
   - **Console UI**: The system is designed to interact with users via the console, using `cin` and `cout` for input and output operations.
   - **Masked Input for Sensitive Data**: The password and PIN are masked using `getch()` to enhance security during input.

### 4. **Conditional Statements and Loops**
   - **Control Flow**: The system makes extensive use of `if-else` statements and `switch-case` structures to handle different user choices and actions.
   - **Loops**: Loops are used to continuously prompt the user for input until a valid choice is made or to repeat certain operations (e.g., displaying the menu after a transaction).

### 5. **System Commands**
   - **System Calls**: The system uses commands like `system("cls")` to clear the console screen and improve the user experience by keeping the interface clean and focused on the current task.

## Getting Started

### Prerequisites
- A C++ compiler (e.g., GCC, MSVC)
- A terminal or command prompt to run the executable

### Running the Program
1. Compile the code using a C++ compiler.
2. Run the executable in the terminal.
3. Follow the on-screen instructions to interact with the Bank & ATM Management System.

### Note
- The default administrator credentials are hardcoded as `email: Abhay@gmail.com`, `pin: 12345`, and `password: 12345`.
- The data is stored in plain text files, so ensure the integrity and security of these files as they contain sensitive user information.

## Conclusion

This Bank & ATM Management System demonstrates the application of OOP principles and file handling in C++ to create a functional and interactive banking application. The system, though basic, covers essential banking operations and provides a strong foundation for further enhancement and development.
