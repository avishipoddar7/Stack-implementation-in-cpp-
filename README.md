# Stack-implementation-in-cpp-
# C++ Stack Implementation using Arrays  

This repository contains a C++ program demonstrating a **stack** data structure using arrays.  

---

## What is a Stack?  
A **stack** is a linear data structure that follows the **LIFO (Last In, First Out)** principle.  
- **Push**: Insert an element on top of the stack  
- **Pop**: Remove the top element  
- **Peek/Top**: Retrieve the top element without removing it

<img width="1152" height="582" alt="image" src="https://github.com/user-attachments/assets/69c98860-b0ef-437c-8176-3301ef9a2099" />


---

## Program Overview  

| Feature | Description |
|---------|-------------|
| Class | `Stack` with array of fixed size (`MAX = 5`) |
| Operations | `push(value)` – insert element<br>`pop()` – remove top element<br>`peek()` – retrieve top element<br>`display()` – show all elements |
| Top Pointer | `top` keeps track of the topmost element in the stack |
| Overflow & Underflow | Handles stack overflow and underflow conditions with messages |

---

## Algorithm  

1. **Initialization:**  
   - Set `top = -1`  
   - Create array `array[MAX]` to store elements  

2. **Push Operation:**  
   - If `top == MAX-1`, print "Stack Overflow"  
   - Else, increment `top` and insert `value`  

3. **Pop Operation:**  
   - If `top == -1`, print "Stack Underflow"  
   - Else, remove `array[top]` and decrement `top`  

4. **Peek Operation:**  
   - If stack is empty, return dummy value (-1)  
   - Else, return `array[top]`  

5. **Display Operation:**  
   - If stack is empty, print "Stack is empty"  
   - Else, loop from `0` to `top` and print elements  

6. **Main Function:**  
   - Create a `Stack` object  
   - Perform `push`, `pop`, `peek`, and `display` operations to demonstrate functionality  

---

## Concepts Demonstrated  
- Array-based stack implementation in C++  
- Stack operations: push, pop, peek, display  
- Handling overflow and underflow  
- Use of class, private members, and methods  
