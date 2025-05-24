## 🔍 Assignment Overview  
This C++ program automates the process of calculating coursework grades for a class, designed to help lecturers easily manage and evaluate student performance. The system reads raw assessment marks from an input file (`CPT111_CWMarks.txt`) and calculates the weighted total based on user-specified percentages for each assessment component which are Test 1, Test 2, Assignment 1 and Assignment 2

By using this system the lecturer will provides:
- The total coursework marks
- Number of students
- The weightage for each assessment component (e.g., 10 10 15 15)

The program then calculates each student's:
- Individual weighted scores
- Total coursework marks
- Normalized marks over 100
- Final letter grade based on the following schema:

| Marks    | Grade |
|----------|-------|
| 80–100   | A     |
| 70–79    | B     |
| 60–69    | C     |
| 50–59    | D     |
| Below 50 | F     |

The results are written to `CPT111_CWMarks_Output.txt` in a clean, structured CSV format. The program uses a console-based menu interface to interact with the user, allowing grading or quitting the system.

---

## 💡 Concepts Used  

This project demonstrates a practical implementation of fundamental C++ programming concepts, including:

- **File Input/Output**:  
  - Reading structured data from an input file using `ifstream`
  - Writing calculated results to an output file using `ofstream` in CSV format

- **Functions**:  
  - `read()`: Parses the input file and loads student data  
  - `calculate()`: Computes weighted scores based on input percentages  
  - `calculateGrade()`: Assigns letter grades based on the final scores  
  - `write()`: Outputs all processed data to the output file

- **Pointers and Arrays**:  
  - Arrays are used to store data for multiple students  
  - Pointers are used in function parameters to allow manipulation of arrays across functions

- **Control Structures**:  
  - `for` loops are used to iterate through student data  
  - `switch` and `if-else` structures manage user choices and grading logic

- **Input Validation**:  
  - Ensures weightage percentages and menu choices are valid  
  - Prevents negative or invalid input for assessment components

- **User-Friendly Console Interface**:  
  - Presents a menu-driven experience with clear prompts and structured output messages
  - Provides feedback on both input reading and output generation
