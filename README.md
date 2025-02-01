# Operating Systems Assignment: I/O and Process Management

This repository contains two C programs that demonstrate concepts related to **I/O operations**, **process management**, and **timers** in an operating systems context. The programs are designed to explore the efficiency of file I/O and the use of multiple processes to perform tasks concurrently.

---

## **Problem 1: File I/O and Process Forking**

### **Description**
This program writes all odd numbers from 1 to 100,000 to an output file. It performs the following tasks:
1. **Single Process**:
   - Opens and closes the file 50,000 times (inefficient I/O).
   - Measures the elapsed time to complete the task.
2. **Multiple Processes**:
   - Forks 10 child processes, each handling a range of 10,000 numbers (e.g., 1–10,000, 10,001–20,000, etc.).
   - Each child writes to a separate file.
   - Measures the elapsed time for all processes to complete.
   - Combines the 10 files into one final output file.

### **Goal**
- Demonstrate that breaking up I/O tasks across multiple processes can reduce total elapsed time.

### **How to Run**
1. Compile the program:
   ```sh
   gcc -o problem1 problem1.c
## **Problem 2: Enhanced Quiz Program**

### **Description**
This interactive C program presents arithmetic questions to the user while implementing a timer mechanism.

### **Features:**
- Parent process generates math problems.
- User must answer within **5 seconds**.
- If no answer is provided within **10 seconds**, the question is marked as missed.
- Keeps track of:
  - Correct answers.
  - Incorrect answers (wrong responses within the time limit).
  - Missed questions (timeout occurrences).
- Displays final quiz performance.

### **How to Run**
1. Compile the program:
   ```sh
   gcc -o quiz_program quiz_program.c
