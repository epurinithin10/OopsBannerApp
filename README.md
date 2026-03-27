# OOPS Banner App

## Overview
The OOPS Banner App is built incrementally using multiple use cases.
Each use case extends the previous one while following a structured Git workflow.

---

## Use Case 1 (UC1)
Prints the literal text `OOPS` to the console using a simple Java program.

---

## Use Case 2 (UC2): Print OOPS as Banner

### Goal
Extend UC1 by displaying the word **OOPS** in a large banner format using
asterisks (`*`) and spaces.

### Description
In this use case, the program prints a **multi-line ASCII banner** representation
of the word **OOPS**.  
Each letter is constructed manually using `*` and spaces and printed using
individual `System.out.println()` statements.

This use case focuses on understanding:
- ASCII art creation
- Manual string construction
- Sequential print statements
- Output alignment and readability

No loops, functions, or data structures are used in this use case, as the goal
is to understand the basic visual construction before refactoring in later use cases.

---

### Key Concepts Used
- ASCII Art using characters
- String literals and string concatenation
- Multiple print statements
- Console output formatting
- Incremental development using Git feature branches

---

## Use Case 3 (UC3): String.join Refactor

UC3 refactors the banner rendering logic from UC2 by replacing
string concatenation using the `+` operator with the `String.join()` method.

This improves memory efficiency by reducing intermediate String object creation
while preserving the same visual banner output.

---
## Use Case 4 (UC4): Array and Loop Refactor

UC4 improves code modularity by storing all banner lines
in a String array and printing them using an enhanced for loop.
This removes repetitive print statements and improves maintainability
while preserving the same banner output.

---
## Use Case 5 (UC5): Inline Array Initialization

UC5 improves code conciseness by declaring and initializing
the banner lines array in a single statement using inline
String.join() calls, while preserving the same banner output.

---
## Use Case 6 (UC6): Static Helper Methods

UC6 refactors banner generation logic into static helper methods
for each character (O, P, S). This improves modularity, reusability,
and readability while preserving the same banner output.

---
## Use Case 7 (UC7): Inner Static Class for Character Patterns

UC7 introduces an inner static class to encapsulate banner character
patterns. This improves modularity, scalability, and reusability by
centralizing character-to-pattern mapping while preserving the same
banner output.
---
## Use Case 8 (UC8): Map-based Character Pattern Rendering

UC8 replaces array-based character pattern management with a HashMap,
allowing efficient lookup and reuse of ASCII patterns. The banner is
rendered using utility functions and nested loops while preserving the
same visual output.
### How to Run
```bash
javac OOPSBannerApp.java
java OOPSBannerApp
