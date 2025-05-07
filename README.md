# Compiler Design for Stack Operations

This project implements the **first three phases of a compiler**—**Lexical Analysis, Syntax Analysis, and Semantic Analysis**—to simulate and validate **stack operations** such as `PUSH`, `POP`, and `DISPLAY`. The project is built using **Flex** (Lexical Analyzer) and **Bison** (Parser Generator), simulating how compilers process and verify source code input.

---

## 🧠 Project Objective

To design a basic compiler that can:
- Tokenize input stack commands (Lexical Analysis)
- Parse valid command sequences (Syntax Analysis)
- Simulate correct stack behavior (Semantic Analysis)

---

## 🛠️ Tech Stack

- **Languages:** C
- **Tools:** Flex (Lex), Bison (Yacc)
- **Concepts Used:** 
  - Compiler Front-End
  - Context-Free Grammars (CFG)
  - Syntax-Directed Translation
  - Stack Simulation

---

## 🚀 Features

- **Lexical Analyzer:** Recognizes tokens like `PUSH`, `POP`, `DISPLAY`, and integers.
- **Parser:** Validates syntax using defined grammar rules for stack operations.
- **Semantic Analyzer:**
  - Implements a simulated stack.
  - Enforces valid stack behavior.
  - Reports semantic errors like popping from an empty stack.
- **Output:** Displays operation results or error messages based on input correctness.

---

## 📂 File Structure

```bash
├── lex.l # Lexical analyzer (Flex)
├── parser.y # Syntax and semantic analyzer (Bison)
├── input.txt # input file
```

---

## 🧑‍💻 How to Run

1. **Install Flex and Bison:**

2. **Compile the program**
```bash
flex lex.l
bison -d parser.y
gcc parser.tab.c lex.yy.c -o stack_simulator
```
3. **Run the executable**
```bash
./stack_simulator
```
---
## 📝 Notes
1. The implementation is educational and simulates how real-world compilers operate in the front-end.
2. Good for understanding compiler theory concepts and applying them to practical problems like stack simulations.

---
## 📌 Future Enhancements
1. Add Intermediate Code Generation
2. Build a GUI to visualize the stack behavior
3. Extend support to more complex data structures (queues, trees)
