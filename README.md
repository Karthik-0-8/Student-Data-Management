# Student Management System in C++

## Overview

This is a simple Student Management System implemented in C++ using a singly linked list. The program allows for the creation, management, and manipulation of student records, including adding new records, searching for records, and deleting records based on various criteria (ID, Name, Phone Number). The system stores the following information for each student:
- Student ID
- Name
- GPA (Grade Point Average)
- Phone Number

## Features

### 1. Insert New Student Record
- The `insertion()` function allows you to add a new student's details to the linked list.
- If the list is empty, the new student becomes the head of the list.
- Otherwise, the new student is appended to the end of the list.

### 2. Display All Student Records
- The `display()` function traverses the linked list and displays the details of all the students in the list, including their ID, Name, GPA, and Phone Number.

### 3. Search for a Student Record
- The `check()` function allows you to search for a student by their ID, Name, or Phone Number.
- If a match is found, the student's details are displayed.
- If no match is found, a message indicating that the student was not found is displayed.

### 4. Delete a Student Record
- The `Delete()` function allows you to remove a student's record from the list based on their ID, Name, or Phone Number.
- If the student is found and deleted, a success message is displayed.
- If the student is not found, a message indicating that the student was not found is displayed.

### 5. User Interaction
- The `main()` function provides a simple console-based menu for interacting with the system.
- Users can choose to search, display, or delete records, or exit the program.

## How to Use

1. **Compile the Program:**
   - Use a C++ compiler to compile the code. For example:
     ```
     g++ student_management.cpp -o student_management
     ```

2. **Run the Program:**
   - Run the compiled executable:
     ```
     ./student_management
     ```

3. **Interacting with the Program:**
   - Follow the on-screen instructions to manage the student records.
   - You can add student records by modifying the `main()` function where the `insertion()` calls are made.
   - Use the menu options to search, display, or delete records as needed.

## Example

Here’s a simple example of how the program might be used:

1. **Insert New Records:** Automatically done by the initial code.
2. **Display Records:** Choose option `2` from the menu to display all student records.
3. **Search for a Record:** Choose option `1` from the menu, then select `1`, `2`, or `3` to search by ID, Name, or Phone Number, respectively.
4. **Delete a Record:** Choose option `3` from the menu, then select `1`, `2`, or `3` to delete by ID, Name, or Phone Number, respectively.
5. **Exit:** Choose option `4` to exit the program.

## Notes

- The linked list implementation ensures that operations like insertion, search, and deletion are straightforward and efficient.
- The program is designed to handle basic error-checking, such as checking if a student record exists before attempting to delete it.

## Future Improvements

- **Dynamic Memory Management:** Currently, `free()` is used to delete nodes, but consider using `delete` in C++ for proper memory management.
- **Input Validation:** Add more robust input validation to handle incorrect or unexpected inputs.
- **Persistence:** Implement a feature to save the records to a file and load them when the program starts.
