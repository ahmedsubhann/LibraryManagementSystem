# Java Library Management System

This is a simple, console-based Library Management System built in Java. It simulates the key operations of a library and demonstrates essential object-oriented programming concepts.

## Overview

The system allows two types of users: **Staff** and **Members**. Staff can manage library inventory and user records, while members can browse, borrow, and return items.

## Functionalities

### Staff Functions
- Manage library items (Books and Magazines): add, update, delete
- Manage members: register, edit, remove
- View all items and active loans
- Authentication (login/logout)

### Member Functions
- View available books and magazines
- Borrow and return items
- View current loans and any overdue charges
- Authentication (login/logout)

## Object-Oriented Design

This project applies the four pillars of object-oriented programming:

- **Encapsulation**: Attributes are kept private and accessed through getters and setters.
- **Inheritance**: Shared features are inherited through base classes (`User`, `LibraryItem`).
- **Abstraction**: Abstract classes like `LibraryItem` hide common behavior.
- **Polymorphism**: Overridden methods in subclasses provide custom behavior (e.g., `toString()`).

## Technical Details

- The system runs entirely in memory (no persistent storage).
- All data is temporary and exists only during the program's execution.

## Input Handling

- Input validation ensures data is clean and reliable:
  - String fields are checked for emptiness
  - Dates must follow `yyyy-mm-dd` format
  - Numeric values (e.g., membership IDs) must be positive
- Errors are handled with try-catch blocks, and clear messages are shown to users.

## Testing and Edge Cases

The system was manually tested for:

- Correct behavior in standard operations (borrowing, returning, logging in)
- Edge cases such as:
  - Borrowing unavailable items
  - Logging in with incorrect credentials
  - Handling invalid or duplicate data entries
  - Returning items late and calculating overdue charges

## Technologies Used

- **Language**: Java
- **Interface**: Text-based console
- **Design Approach**: Object-Oriented Programming

