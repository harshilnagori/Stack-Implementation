
# Experiment 19- Implementation of Stack using Array


- **Name:** Harshil Nagori
- **Class:** ENTC A2
- **PRN:** 24070123046
- **Title:** Implementation of Stack using Array in C++  

---

## Aim
To implement a **Stack data structure** using arrays in C++ with operations **push, pop, and display**, and to demonstrate conditions of **overflow and underflow**.

---

## Objectives
1. To understand the concept of **stack** as a linear data structure.  
2. To implement stack operations using **arrays** in C++.  
3. To apply the concepts of **object-oriented programming (OOP)** such as **classes and objects**.  
4. To simulate real-life stack functionality (Last-In-First-Out - LIFO).  
5. To analyze **overflow** and **underflow** conditions in stack.  

---

## Theory

### What is a Stack?
A **stack** is a linear data structure that follows the **Last In First Out (LIFO)** principle, i.e., the element that is inserted last will be the first one to be removed. Think of a stack like a **pile of plates** – you add new plates at the top, and when you need one, you take the top plate first.  

In this experiment, the stack is implemented using a **fixed-size array**. The **top pointer/index** is used to keep track of the current top element in the stack.

### Key Operations
1. **Push (Insertion):**  
   Adds an element to the top of the stack. If the stack is full (i.e., `top == MAX-1`), it results in a **Stack Overflow**.  

2. **Pop (Deletion):**  
   Removes the topmost element from the stack. If the stack is empty (i.e., `top == -1`), it results in a **Stack Underflow**.  

3. **Display:**  
   Traverses the stack from bottom to top and prints elements in the stack. If the stack is empty, a message is shown.  

### Applications of Stack
- **Expression evaluation** (Postfix/Prefix conversion).  
- **Function calls and recursion handling** in programming languages.  
- **Undo/Redo functionality** in text editors.  
- **Backtracking algorithms** (maze problems, puzzles).  
- **Memory management** in operating systems.  

---

## Comparison: Stack vs Queue

| Feature            | Stack (LIFO)                         | Queue (FIFO)                        |
|--------------------|---------------------------------------|--------------------------------------|
| Order of Access    | Last In, First Out (LIFO)            | First In, First Out (FIFO)           |
| Insertion Point    | Always at the **top**                | Always at the **rear**               |
| Deletion Point     | Always at the **top**                | Always at the **front**              |
| Example            | Pile of books, undo operations       | Waiting line at a ticket counter     |
| Applications       | Function calls, recursion, undo      | Scheduling, data buffering, printers |

---

## Concepts Used
- **Classes and Objects:** Encapsulation of stack behavior inside a `Stack` class.  
- **Arrays:** Used as the underlying storage structure for the stack.  
- **Data Abstraction:** User interacts only with `push`, `pop`, and `display` without internal details.  
- **Access Specifiers:** `private` for data protection (`arr`, `top`), `public` for operations.  
- **Control Structures:** Conditional statements to check overflow/underflow.  

---
## Algorithm and summaries

## Program Summary
This program demonstrates the implementation of a **stack using arrays** in C++. The class `Stack` encapsulates the stack behavior with the following features:
- A private integer array of size `MAX`.  
- A `top` variable initialized to `-1` to track the stack’s current top element.  
- **push()** function to insert values and check overflow condition.  
- **pop()** function to delete values and check underflow condition.  
- **display()** function to print current stack contents.  

The `main()` function demonstrates the stack operations by pushing elements until overflow, and popping elements until underflow, showcasing both conditions effectively.

---

## Algorithm

### Algorithm for Push Operation
1. Check if `top >= MAX - 1`.  
   - If **true**, display "Stack Overflow".  
   - Else, increment `top` and insert the element at `arr[top]`.  

### Algorithm for Pop Operation
1. Check if `top < 0`.  
   - If **true**, display "Stack Underflow".  
   - Else, decrement `top`.  

### Algorithm for Display Operation
1. Check if `top < 0`.  
   - If **true**, display "Stack is empty".  
   - Else, iterate from `0` to `top` and print elements.  

---

## Conclusion
- The stack was successfully implemented using arrays in C++.  
- Operations such as **push**, **pop**, and **display** were demonstrated.  
- The program clearly showed conditions of **Stack Overflow** and **Stack Underflow**.  
- This experiment enhanced the understanding of **linear data structures**, **LIFO principle**, and **object-oriented programming** in C++.  

---
