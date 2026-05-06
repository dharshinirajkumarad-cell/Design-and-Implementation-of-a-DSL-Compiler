#  DSL Compiler in C

##  Project Overview

This project demonstrates the design and implementation of a **simple Domain-Specific Language (DSL) compiler** using C. It simulates the core phases of a compiler such as lexical analysis, syntax analysis, semantic analysis, and intermediate code generation.

The compiler processes basic assignment statements and arithmetic expressions and converts them into an intermediate representation.



##  Objectives

* Simulate the working of a compiler
* Understand different phases of compilation
* Process simple arithmetic expressions
* Generate intermediate code (Three-Address Code)
* Build a modular and easy-to-understand system

##  Sample Input

```
x = 10
y = 5
z = x + y
```

##  Compiler Phases

### 🔹 1. Lexical Analysis

* Breaks input into tokens
* Identifies:

  * Identifiers → `x, y, z`
  * Numbers → `10, 5`
  * Operators → `+, =`

---

### 🔹 2. Syntax Analysis

* Validates statement structure
* Ensures format:

```
variable = expression
```

---

### 🔹 3. Semantic Analysis

* Checks correctness of variable usage
* Ensures all variables are valid and properly used

---

### 🔹 4. Intermediate Code Generation

* Converts expressions into **Three-Address Code**

#### Example:

```
t1 = x + y
z = t1
```

##  Logic Used

* Character-by-character scanning using `isalpha()` and `isdigit()`
* Simple validation for assignment statements
* Predefined valid input to avoid runtime errors
* Use of temporary variables (`t1`, `t2`) for intermediate code


##  How to Run

###  Compile

```
gcc program.c -o program
```

###  Execute

```
./program
```

> If using C++ compiler:

```
g++ program.cpp -o program
./program
```

---

##  Project Structure

```
DSL-Compiler/
│
├── program.c        # Main source code
├── README.md        # Project documentation
```

---

##  Features

* Simple and modular compiler design
* Clear demonstration of all compiler phases
* Easy to understand and extend
* Clean and readable output

---

##  Learning Outcomes

* Understanding of compiler design basics
* Knowledge of lexical, syntax, and semantic analysis
* Experience in generating intermediate code
* Insight into modular programming

---

## Conclusion

This project provides a clear and structured approach to understanding how a compiler works. It demonstrates how input statements are processed step-by-step and converted into intermediate code, making it a great foundation for learning advanced compiler concepts.

---

##  Author

**Dharshini Rajkumar**

---
