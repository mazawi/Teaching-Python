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

## `elif` Statement

  - The `elif` statement, short for "else if," is used when there are multiple conditions to be checked after the initial `if` condition is false.

- **Syntax:**
 ```python
    if condition1:
        # Code block to execute if condition1 is true
    elif condition2:
        # Code block to execute if condition2 is true
    else:
        # Code block to execute if both conditions are false
```

- If `condition1` is true, the code block beneath it is executed, and the subsequent `elif` and `else` blocks are skipped.
- If `condition1` is false, the program checks `condition2`.
- If `condition2` is true, the corresponding code block is executed.
- If both conditions are false, the code block under `else` is executed.

- **Example:**
  ```python
  score = 75
  if score >= 90:
      print("A Grade")
  elif score >= 80:
      print("B Grade")
  elif score >= 70:
      print("C Grade")
  else:
      print("You need improvement.")
  ```

- **Output:**
  ```
  C Grade
  ```

- **Sequential Checking:**
        - Conditions are checked sequentially, and the first true condition's block is executed.
      - **Example:**
 ```python
if x > 0:
	print("Positive")
elif x < 0:
	print("Negative")
```


## Nested `if` Statements

  - **Nested `if` statements** involve placing one or more `if` statements inside another, creating a nested structure for complex decision-making.

- **Syntax:**
 ```python
if condition1:
	# Outer if block
		if condition2:
            # Nested if block
		else:
            # Nested else block
else:
	# Outer else block
```

 - The outer `if` statement is evaluated first.
- If its condition is true, it proceeds to the inner `if` statement.
- The inner `if` statement's code block is executed if its condition is true.
- If the outer `if` condition is false, the `else` block is executed.

- **Example:**
  ```python
  num = 15
  if num > 10:
      print("Number is greater than 10.")
      if num % 2 == 0:
          print("Number is even.")
      else:
          print("Number is odd.")
  else:
      print("Number is 10 or less.")
  ```

- **Output:**
  ```
  Number is greater than 10.
  Number is odd.
  ```

  - - **Hierarchical Decision-Making:**
        - Nested `if` statements allow for a hierarchical structure, evaluating conditions at different levels.
      - **Example:**
        ```python
        if weather == "rainy":
            if has_umbrella:
                print("You're prepared for the rain.")
            else:
                print("Consider taking an umbrella.")
        ```


## Comparison Operators

  - **Comparison operators** are used to compare values in conditional statements, resulting in a Boolean outcome (True or False).

- **Common Comparison Operators:**
  - 1. **Equal to (`==`):**
      - Checks if two values are equal.
  - 2. **Not equal to (`!=`):**
      - Checks if two values are not equal.
  - 3. **Greater than (`>`):**
      - Checks if one value is greater than another.
  - 4. **Less than (`<`):**
      - Checks if one value is less than another.
  - 5. **Greater than or equal to (`>=`):**
      - Checks if one value is greater than or equal to another.
  - 6. **Less than or equal to (`<=`):**
      - Checks if one value is less than or equal to another.

- **Syntax:**
  - ```python
    x = 10
    y = 5
    if x > y:
        # Code block to execute if x is greater than y
    ```

- **Example:**
  ```python
  temperature = 25
  if temperature > 30:
      print("It's a hot day!")
  ```

   **Boolean Outcomes:**
        - Comparison operators evaluate to either True or False.
      - **Example:**
```python
if x == 10:
	print("x is equal to 10")
```


## Logical Operators

  - **Logical operators** are used to combine multiple conditions in conditional statements, providing more complex decision-making structures.

- **Common Logical Operators:**
  - 1. **AND (`and`):**
      - True if both conditions on either side of it are true.
  - 2. **OR (`or`):**
      - True if at least one of the conditions on either side of it is true.
  - 3. **NOT (`not`):**
      - True if the condition following it is false, and vice versa.

- **Syntax:**
```python
    age = 25
    if age > 18 and age < 60:
        # Code block to execute if age is between 18 and 60
```

- **Example:**
```python
  temperature = 25
  time_of_day = "afternoon"
  if temperature > 20 and time_of_day == "afternoon":
      print("It's a warm afternoon.")
```

 - **Combining Conditions:**
        - Logical operators allow combining conditions to create more nuanced decision structures.
      - **Example:**
        ```python
        if x > 0 and x < 10:
            print("x is a positive single-digit number")
        ```


### Example 1: Voting Eligibility

```python
age = 22

if age >= 18:
    print("You are eligible to vote.")
else:
    print("You are not eligible to vote.")
```

- **Output:**
  ```
  You are eligible to vote.
  ```

### Example 2: Grading System

```python
score = 85

if score >= 90:
    print("A Grade")
elif score >= 80:
    print("B Grade")
elif score >= 70:
    print("C Grade")
else:
    print("You need improvement.")
```

- **Output:**
  ```
  B Grade
  ```

### Example 3: Checking Multiple Conditions

```python
temperature = 28
time_of_day = "morning"

if temperature > 25 and time_of_day == "morning":
    print("It's a warm morning.")
else:
    print("Conditions not met.")
```

- **Output:**
  ```
  It's a warm morning.
  ```

### Example 4: Identifying Number Quadrants

```python
x = 3
y = -4

if x > 0 and y > 0:
    print("Quadrant I")
elif x < 0 and y > 0:
    print("Quadrant II")
elif x < 0 and y < 0:
    print("Quadrant III")
elif x > 0 and y < 0:
    print("Quadrant IV")
else:
    print("On an axis or at the origin.")
```

- **Output:**
  ```
  Quadrant II
  ```
## Exercises
### Exercise 1: Voting Eligibility

Write a Python program that takes the user's age as input and prints whether they are eligible to vote or not.

### Exercise 2: Temperature Classification

Create a program that takes the current temperature as input and classifies it into categories such as "Cold," "Moderate," or "Hot."

### Exercise 3: Grade Calculator

Design a program that takes a student's exam score as input and prints their corresponding letter grade based on the following scale: A (90-100), B (80-89), C (70-79), D (60-69), F (0-59).

### Exercise 4: Leap Year Checker

Write a Python script that checks if a given year is a leap year. A leap year is either divisible by 4 but not by 100, or divisible by 400.

### Exercise 5: Odd or Even

Create a program that takes an integer as input and prints whether it's an odd or even number.

### Exercise 6: ATM Withdrawal

Develop a program that simulates an ATM withdrawal. Take the user's account balance and withdrawal amount as input. Ensure the withdrawal amount is within the account balance and provide appropriate messages.

### Exercise 7: Time of Day Greeting

Design a program that takes the current time (in 24-hour format) as input and prints a greeting message based on the time of day (e.g., "Good morning," "Good afternoon," "Good evening").



