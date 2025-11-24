



PROBLEM STATEMENT-
The lack of tracking all the daily tasks throughout the day and keeping up with the schedule

Solution-
A simple programme which can keep track of all the user’s task, according to the time, record if it has been completed or not.
The programme should be able to add, remove, update, search, display the data and create new file to store data.

1. Project Overview
This project is a command-line based Task Manager application written in Python. The main purpose is to allow users to create, view, search, update, and delete personal task records efficiently. All operations are performed on structured data stored securely in a binary data file using Python's pickle module.


FUNCTIONS
•	Create a New Data File: The system must let the user start with a new, empty to-do file and enter multiple records.
•	Add Task: The system must allow the user to add new tasks, with serial numbers assigned automatically, and all fields (date, hour, description, etc.) entered and validated.
•	Display Tasks: The system must be able to read all task records from the file and display them in a tabular format.
•	Search Tasks:
By serial number: The user can search for a specific task using its serial number.
By date: The user can search for all tasks scheduled on a specific date (day, month, year).
•	Update Task: The user can select a task by serial number and update any or all fields.
•	Delete Task: The user can select a task by serial number and delete it from the file.
•	Mark Task as Completed: The user can update the status of a task to "completed".
•	Menu Navigation: The user can choose and access any feature through a clear, interactive menu.
•	Input Validation: All operations must check for valid data (no empty tasks, valid dates/times, etc.).
•	Error Reporting: If invalid inputs or missing records are encountered, the system informs the user clearly.


NON FUNCTIONAL REQUIREMENTS-
•	Create a New Data File: The system must let the user start with a new, empty to-do file and enter multiple records.
•	Add Task: The system must allow the user to add new tasks, with serial numbers assigned automatically, and all fields (date, hour, description, etc.) entered and validated.
•	Display Tasks: The system must be able to read all task records from the file and display them in a tabular format.
•	Search Tasks:
•	By serial number: The user can search for a specific task using its serial number.
•	By date: The user can search for all tasks scheduled on a specific date (day, month, year).
•	Update Task: The user can select a task by serial number and update any or all fields.
•	Delete Task: The user can select a task by serial number and delete it from the file.
•	Mark Task as Completed: The user can update the status of a task to "completed".
•	Menu Navigation: The user can choose and access any feature through a clear, interactive menu.
•	Input Validation: All operations must check for valid data (no empty tasks, valid dates/times, etc.).
•	Error Reporting: If invalid inputs or missing records are encountered, the system informs the user clearly.



2. Modules Used
pickle: For object serialization—storing and retrieving lists representing tasks.

tabulate: For displaying tasks in well-formatted tables.

time: For simulating delays and providing user feedback.

3. Data Structure
Each task is stored as a list with fields:

Serial Number (S.No)

Hour

Day

Month

Year

Completion Status (Boolean)

Task Description (String)

All task lists are pickled individually into a single binary file named todo.dat.


4. Key Features and Functionality
Create File: Start with a new (or reset) data file and populate it with a user-defined number of records, each validated for correctness before saving.

Add Task: Append new tasks, which are assigned unique serial numbers. Input validation ensures only meaningful records are stored.

Display All Tasks: Read all tasks, collect them into a list, and display them using an attractive table format.

Search Task: Allow searching by either serial number or date to quickly locate specific tasks.

Update Task: Find a task by serial number, allow user to update any field using prompts, and write the updated set of tasks back to the file.

Delete Task: Remove a specified record by serial number, rewriting the remaining tasks for consistency.

Interactive Menu: Present a user-friendly menu loop for operation selection—ensuring repeat usability and easy navigation.

7.Testing approach
Repeated iterations of running the programme in the terminal to test various functions and a final test with all the functions, creating a new file from scratch.






9.Possible Enhancements
Migrate to storing tasks as a single list for more efficient updates and deletions.

Add features like task priorities, due notifications, or a graphical/user interface.

Port to a web framework (e.g., Flask) for browser-based interaction.

8. Conclusion
This Task Manager is a robust Python-based app for basic personal productivity, illustrating practical file handling, serialization, and menu-driven user interaction. The modular codebase and input validation make it both reliable and extensible for further development.
