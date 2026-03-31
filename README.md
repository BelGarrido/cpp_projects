# 42 School C++ Modules (CPP 00 - CPP 04)

This repository showcases my journey through the initial C++ modules at 42 School, marking a significant transition from procedural C programming to Object-Oriented Programming (OOP) paradigms. These projects are designed to build a strong foundation in C++ fundamentals, memory management, and core OOP concepts.

## Project Overview

The 42 School curriculum emphasizes hands-on learning and strict adherence to coding standards. This collection of projects reflects my progression from basic C++ syntax to more advanced topics like polymorphism and inheritance. Each module introduces new concepts, reinforcing the principles of robust and efficient C++ development.

## Technical Constraints & Standards

Throughout these modules, strict technical constraints were applied to ensure a deep understanding of C++ mechanics:

*   **C++98 Standard:** All code is written to conform to the C++98 standard, avoiding modern C++ features introduced in later standards. This constraint encourages a thorough understanding of fundamental language constructs.
*   **Orthodox Canonical Form (OCF):** Classes are implemented following the Orthodox Canonical Form, which typically includes:
    *   A default constructor
    *   A copy constructor
    *   A copy assignment operator
    *   A destructor
    This practice ensures proper resource management and predictable object behavior, especially when dealing with dynamic memory.

## Module Breakdown

### CPP 00: Basics & Syntax

This module served as the introduction to C++, focusing on the fundamental building blocks of the language.

*   **Namespaces:** Understanding how to organize code and prevent naming conflicts.
*   **Classes:** Defining custom data types and encapsulating data with member functions.
*   **Member Functions:** Implementing behaviors associated with class objects.
*   **Standard I/O Streams (`iostream`):** Utilizing `cin`, `cout`, `cerr`, and `clog` for input and output operations.

### CPP 01: Memory & Pointers

Building upon the basics, CPP 01 delved into C++'s explicit memory management and advanced pointer usage.

*   **Dynamic Memory Allocation (`new`/`delete`):** Managing memory on the heap for objects and arrays.
*   **References:** Understanding aliases to existing variables and their use cases.
*   **Pointers to Members:** Working with pointers that refer to non-static members of a class.

### CPP 02: Ad-hoc Polymorphism

This module introduced the concept of ad-hoc polymorphism through operator overloading and explored fixed-point number representation.

*   **Operator Overloading:** Customizing the behavior of operators for user-defined types, enhancing code readability and expressiveness.
*   **Fixed-Point Number Representation:** Implementing a custom class to handle fixed-point arithmetic, providing insights into numerical precision and data representation.

### CPP 03: Inheritance

CPP 03 focused on one of the core pillars of OOP: inheritance, and the "is-a" relationship.

*   **Class Hierarchies:** Designing and implementing base and derived classes.
*   **'is-a' Relationship:** Understanding how inheritance models real-world relationships where a derived class "is a" type of its base class.
*   **Access Specifiers:** Managing visibility and access to members within inheritance hierarchies.

### CPP 04: Subtype Polymorphism

The final module in this series explored subtype polymorphism, a powerful concept for flexible and extensible designs.

*   **Virtual Functions:** Enabling dynamic method dispatch based on the actual type of the object at runtime.
*   **Abstract Classes:** Defining interfaces and enforcing common behaviors for derived classes.
*   **Interfaces (Pure Virtual Functions):** Creating contracts for classes to adhere to, promoting loose coupling and extensibility.

## Key Takeaways: What I Learned

This initial set of C++ modules provided invaluable lessons that extend beyond mere syntax:

*   **Memory Safety:** A profound appreciation for explicit memory management, the dangers of memory leaks, double frees, and dangling pointers, and the importance of the Rule of Three/Five/Zero.
*   **Deep vs. Shallow Copies:** A clear understanding of when and why deep copies are necessary to prevent unintended side effects and ensure data integrity, especially with dynamically allocated members.
*   **Importance of the `vtable`:** Gaining insight into how virtual functions are implemented under the hood using the virtual table (`vtable`), which is crucial for understanding runtime polymorphism and its performance implications.
*   **Design Principles:** The foundational importance of encapsulation, inheritance, and polymorphism in creating modular, maintainable, and extensible software.

## How to Compile

Each module typically contains its own set of source files and a `Makefile`. To compile a specific project:

1.  Navigate to the respective module directory (e.g., `cd cpp00/ex01`).
2.  Run `make` to compile the project.
```
make 
```
3.  Execute the compiled program (e.g., `./a.out` or `./program_name`).
```
zombie.out
```
4.  Run `make fclean` to remove all compiled files and objects.
```
make fclean
```

5.  Run `make re` to recompile the project from scratch.
```
make re
```


