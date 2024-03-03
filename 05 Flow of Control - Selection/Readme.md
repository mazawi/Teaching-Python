# Flow of Control - Selection

## Overview

## Understanding Flow Control in Programming

- **Definition:**
  - Flow control refers to the order in which statements are executed in a program. 
  - It allows the programme to make decisions and repeat certain blocks of code based on conditions.

- **Significance:**
  - Flow control is crucial for writing dynamic and responsive programs. 
  - It enables the execution of different code blocks depending on specific conditions, leading to more intelligent and flexible software.

- **Types of Flow Control:**
  - **Selection:**
    - Involves making decisions based on conditions. 
    - Different code blocks are executed depending on whether certain conditions are met.

  - **Iteration:**
    - Involves repeating a certain block of code multiple times. It is useful for tasks that need to be performed repeatedly.

- **Importance of Selection:**
  - It plays a key role in programming by allowing the execution of specific code based on various conditions. 
  - This is vital for creating adaptable and decision-making programs.

## What is Selection?

  - Selection, in the context of programming, is the process of making decisions within a program based on certain conditions. 
  - It allows the program to execute different sets of instructions based on whether specific conditions are true or false.
  - Enables the creation of dynamic and adaptive programs that can respond to different scenarios.

  - **Conditions:**
    - Logical expressions that evaluate to either true or false.
  - **Conditional Statements:**
    - Code structures that allow the program to choose between different courses of action based on the truth value of conditions.

- **Types of Selection:**
  - **Single Selection:**
    - The program makes a decision between two alternatives.
  - **Multiple Selection:**
    - The program makes a decision between more than two alternatives using `elif` (else if) statements.
  - **Nested Selection:**
    - The inclusion of one or more selection structures within another, forming a nested decision-making structure.

- **Why Selection is Important:**
  - Efficient decision-making is fundamental to creating programs that can handle a variety of scenarios, making them more versatile and powerful.

- **Analogous to Real-World Decision-Making:**
  - The concept of selection mirrors decision-making in everyday life. For instance, if it's raining, take an umbrella; if not, proceed without one.

- **Example:**
  ```python
  temperature = 25

  if temperature > 30:
      print("It's a hot day!")
  else:
      print("The weather is pleasant.")
  ```
 
 ## Conditional Statements

  - **Conditional statements** are powerful tools in programming that allow the execution of different code blocks based on specific conditions.

- **Types of Conditional Statements in Python:**
  1. **`if` Statement:**
      - Executes a block of code if a specified condition is true.
  2. **`else` Statement:**
      - Provides an alternative block of code to execute when the condition in the `if` statement is false.
  3. **`elif` Statement:**
      - Stands for "else if" and is used to check additional conditions if the preceding `if` or `elif` conditions are false.
  4. **Nested `if` Statements:**
      - Involves placing one or more `if` statements inside another, forming a nested structure for complex decision-making.

- **Syntax:**
```python
    if condition:
        # Code block to execute if the condition is true
    elif another_condition:
        # Code block to execute if another_condition is true
    else:
        # Code block to execute if both conditions are false
```

- **Flow Diagram:**
  - Visual representation of how the program flows through different branches based on conditions.
 
  `if` statement

![image](https://github.com/mazawi/Teaching-Python/assets/45329653/fed16820-42aa-442b-bfaa-7d441b51be00)

 `if - else` structure

 ![image](https://github.com/mazawi/Teaching-Python/assets/45329653/28bdcb0e-82f1-4fa0-9539-3d1320ea4a8d)

 
  - **Proper Indentation:**
        - Python relies on proper indentation to determine the scope of code blocks within conditional statements.
      - **Example:**
        ```python
        if x > 0:
            print("Positive")
        else:
            print("Non-positive")
        ```


## Basic Syntax of `if` Statement

- The **`if` statement** is a fundamental element of selection in Python, 
- allowing the execution of a block of code only if a specified condition is true.

- **Syntax:**
```python
    if condition:
        # Code block to execute if the condition is true
 ```

- **Explanation:**
  - The `if` keyword is followed by a condition that evaluates to either true or false.
    - If the condition is true, the indented code block beneath it is executed.
    - If the condition is false, the code block is skipped.

- **Example:**
```python
    age = 18
    if age >= 18:
        print("You are eligible to vote.")
 ```
  - In this example, the program checks if the `age` is greater than or equal to 18. If true, it prints "You are eligible to vote."

- **Indentation Matters:**
        - The indented code block is crucial; it indicates the block of code to be executed if the condition is true.
      - **Example:**
 ```python
        if x > 0:
            print("Positive")
```

## `if-else` Statement

- The `if-else` statement extends decision-making by providing an alternative block of code to execute when the condition in the `if` statement is false.

- **Syntax:**
```python
    if condition:
        # Code block to execute if the condition is true
    else:
        # Code block to execute if the condition is false
```

**Explanation:**
  - The `else` keyword is followed by a code block that is executed when the condition in the `if` statement is false.
   - This allows the program to take a different course of action when the initial condition is not met.

- **Example:**
```python
  marks = 75
  if marks >= 50:
      print("You passed.")
  else:
      print("You failed.")
```
- **Output:**
  ```
  You passed.
  ```

- **Alternative Execution:**
        - Provides an alternative set of instructions to execute when the initial condition is false.
 - **Example:**
 ```python
if temperature > 30:
   print("It's a hot day!")
else:
   print("The weather is pleasant.")
```

