🧮 Simple Calculator with History (Python)
📌 Project Overview

This project is a command-line based Simple Calculator developed using Python.
It performs basic arithmetic operations and also maintains a calculation history using a text file.

The calculator supports:
Addition
Subtraction
Multiplication
Division
Along with extra features like:
Vizwing calculation history
Clearing history
Exiting the program safely

🎯 Objective of the Project

The main objective of this project is to:
Understand Python functions
Learn file handling
Practice string manipulation
Implement loops and conditional statements
Build a real-world console-based application

🛠️ Technologies Used

Programming Language: Python

Concepts Used:

Functions

File handling

Conditional statements

Loops

String operations

Exception handling (basic)

📂 File Used

history.txt
This file stores all previous calculations performed by the user.

🧩 Explanation of Code Components
🔹 1. HISTORY_FILE
HISTORY_FILE = "history.txt"


This variable stores the filename where calculation history is saved.

🔹 2. show_history() Function

Purpose:
Displays all past calculations stored in history.txt.

Working:

Opens the file in read mode

Reads all lines

Prints history in reverse order (latest first)

If file is empty, shows a message

🔹 3. clear_history() Function

Purpose:
Deletes all saved calculation history.

Working:

Opens the file in write mode ('w')

This automatically clears file content

Prints confirmation message

🔹 4. save_to_history(equation, result) Function

Purpose:
Stores each calculation in the history file.

Working:

Opens file in append mode ('a')

Saves equation and result in format:

8 + 8 = 16

🔹 5. calculate(user_input) Function

Purpose:
Performs arithmetic calculations.

Steps:

Splits user input into number, operator, number

Converts numbers to float

Checks operator (+, -, *, /)

Performs calculation

Handles division by zero

Saves result to history if valid

Input Format Example:

8 + 8
10 / 2

🔹 6. main() Function

Purpose:
Acts as the main control loop of the program.

Features:

Displays menu options

Accepts user input continuously

Handles commands:

history → show history

clear → clear history

exit → exit program

Calls calculate() for arithmetic operations


🔁 Program Flow
Start Program
   ↓
Show Menu
   ↓
User Input
   ↓
Command or Calculation?
   ↓
Perform Action
   ↓
Repeat until Exit


🧪 Sample Execution
--- SIMPLE CALCULATOR ---
Enter calculation: 5 + 3
Result: 8

Enter calculation: history
5 + 3 = 8

Enter calculation: clear
History cleared.

Enter calculation: exit
Bye


✅ Advantages
Easy to use
Stores calculation history
Clear separation of logic using functions
Beginner-friendly code structure

⚠️ Limitations
Supports only two numbers at a time
No advanced operations (power, modulus)
No GUI (command-line only)
🚀 Future Enhancements
Add GUI using Tkinter
Support more operators
Add error handling using try-except
Improve input flexibility

📝 Conclusion
This project demonstrates how Python can be used to build a functional, real-world console application using basic programming concepts.
It is ideal for students learning Python fundamentals and file handling.
