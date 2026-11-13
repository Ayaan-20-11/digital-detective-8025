# Mission 4: Programs and Python

## 1. Task / Objective

The objective of this mission was to understand what a computer program is, write and execute a basic Python program, and learn the difference between a compiler and an interpreter.

I used Python 3 on macOS to create and execute my first program.

## 2. Work Completed

### Task 4.1 — Understanding a Computer Program

A computer program is a set of instructions written in a programming language that tells a computer what tasks to perform.

Programming languages make it easier for humans to communicate instructions to computers. These instructions are processed and executed using suitable language translators and runtime environments.

For example, the Python statement:

`print("Hello, World!")`

instructs Python to display the text `Hello, World!` on the screen.

### Task 4.2 — Writing and Executing a Python Program

I created a Python file named `hello.py` inside the `mission-04-programs` directory.

**Program:**

```python
print("Hello, World!")
print("Welcome to Mission 4!")
print("I am learning Python programming.")
```

**Command used to execute the program:**

```bash
python3 hello.py
```

**Output:**

```text
Hello, World!
Welcome to Mission 4!
I am learning Python programming.
```

The program executed successfully and displayed all three messages in the Terminal.

### Task 4.3 — Compiler vs Interpreter

A compiler and an interpreter are language translation and execution mechanisms that help computers process programs written in programming languages.

**Compiler:**

A compiler translates source code into another form, commonly machine code or an intermediate representation, before the program is executed.

Examples of commonly compiled languages include C, C++, and Rust.

**Interpreter:**

An interpreter processes and executes a program through an execution environment, without requiring a separate native executable to be produced first.

Examples of commonly interpreted languages include Python, Ruby, and JavaScript in many environments.

**Difference between a Compiler and an Interpreter:**

| Feature | Compiler | Interpreter |
|---|---|---|
| Translation | Translates the program before execution. | Processes instructions during execution. |
| Output | Often produces a separate executable or compiled output. | Usually does not require a separate native executable. |
| Execution | Executes the compiled output. | Executes through an interpreter or runtime. |
| Error reporting | Compilation errors are reported during compilation. | Errors can be reported as execution reaches the problematic code. |
| Examples | C, C++, Rust | Python, Ruby |

**How Python executes code:**

Python is commonly described as an interpreted language. However, CPython first compiles Python source code into bytecode and then executes that bytecode using its virtual machine.

This helped me understand that real programming language implementations can combine compilation and interpretation techniques.

## 3. Commands / Tools Used

| Command / Tool | Purpose |
|---|---|
| `cd mission-04-programs` | Navigates into the Mission 4 directory. |
| `pwd` | Displays the current working directory. |
| `touch hello.py` | Creates an empty Python file. |
| `python3 hello.py` | Executes the Python program using Python 3. |
| Visual Studio Code | Used to write and edit the Python program. |
| macOS Terminal | Used to execute the program and observe its output. |

## 4. My Understanding

Through this mission, I understood that a computer program is a collection of instructions that tells a computer what to do.

I learned how to create a Python file, write basic print statements, and execute the program using the Python 3 interpreter.

I also understood the difference between compilation and interpretation. A compiler translates source code before execution, whereas an interpreter processes instructions through an execution environment.

I learned that CPython uses both compilation into bytecode and execution through a virtual machine.

## 5. Difficulties Faced

Initially, I executed the Python file before adding any code, so the Terminal displayed no output. I also needed to understand how Python executes a source file and how compilation differs from interpretation.

## 6. How I Resolved Them

I added the required print statements to `hello.py`, saved the file, and executed it again using:

`python3 hello.py`

The program then displayed the expected output successfully.

I also studied the execution flow of compilers and interpreters and learned about Python's bytecode execution process.

## 7. Evidence / Files

- `mission-04-programs/hello.py` — Python program created and executed during this mission.
- `mission-04-programs/README.md` — Documentation of the tasks, commands, output, and concepts learned.
- Terminal output showing the successful execution of the Python program.

## 8. Commit Details

- Commit message: `Complete programs and Python mission`
- Changes pushed to the GitHub repository after completing Mission 4.
