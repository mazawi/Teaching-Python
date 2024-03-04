
## Flow of Control - Loops in Python 

#### **Understanding Flow of Control - Loops in Python**

- **Importance of Repetition:**
  - In programming, repetition is a fundamental concept. Loops provide a mechanism for efficiently executing a block of code repeatedly.

- **Types of Loops in Python:**
 1. **`for` Loop:**
      - Iterates over a sequence (e.g., list, tuple, string).
 2. **`while` Loop:**
      - Repeats a block of code as long as a specified condition is true.

- **Efficiency and Readability:**
  - Loops enhance the efficiency and readability of code by reducing redundancy and allowing for dynamic iteration.

- **Flow Control in Loops:**
  - The flow of control in loops is determined by conditions, making them powerful tools for handling repetitive tasks.


## What are Loops?

  - Loops are control structures that facilitate the repeated execution of a block of code as long as a specific condition remains true.

- **Purpose:**
  - Enable automation and efficiency in handling repetitive tasks within a program.

- **Key Concepts:**
  - - **Iteration:**
        - The process of repeatedly executing a set of statements.
      - **Example:**
        ```python
        for i in range(5):
            print("Iteration", i+1)
        ```
    - **Condition:**
        - The loop continues to execute as long as a specified condition is true.
      - **Example:**
        ```python
        while x < 10:
            print(x)
            x += 1
        ```

- **Types of Loops in Python:**
1. **`for` Loop:**
      - Used for iterating over a sequence (e.g., list, tuple, string).
      - Controlled by the number of elements in the sequence.
 2. **`while` Loop:**
      - Continues executing as long as a specified condition is true.
      - Controlled by the truth value of the condition.

- **Importance:**
  - - **Efficiency:**
        - Simplifies and streamlines code, making it more readable and maintainable.
      - **Example:**
        ```python
        for item in collection:
            process(item)
        ```


## `for` Loop

- The `for` loop is a fundamental construct in Python for iterating over a sequence of elements. It simplifies repetitive tasks by allowing the execution of a block of code for each item in the sequence.

  ```python
  for variable in sequence:
      # Code block to repeat
  ```

- The `for` keyword is used to initiate the loop, followed by a variable that represents each item in the sequence.
- The `in` keyword is used to specify the sequence to iterate over.
- The indented code block beneath the loop is executed for each item in the sequence.

- **Example:**
  ```python
  fruits = ["apple", "banana", "orange"]
  for fruit in fruits:
      print(fruit)
  ```
  
- **Output:**
  ```
  apple
  banana
  orange
  ```

- **Iterable Objects:**
- Sequences like lists, tuples, and strings are iterable, making them suitable for `for` loops.
**Example:**
        ```python
        for char in "Python":
            print(char)
        ```
  - **`range()` Function:**
    - Often used with `for` loops to generate a sequence of numbers.
    - **Example:**
      ```python
      for i in range(1, 6, 2):
          print(i)
      ```
  

## `while` Loop

  - The `while` loop is a fundamental construct in Python that allows the repeated execution of a block of code as long as a specified condition is true.

- **Syntax:**
  ```python
  while condition:
      # Code block to repeat
  ```

- The `while` keyword is followed by a condition that evaluates to either true or false.
- The indented code block beneath it is executed as long as the condition is true.
- The loop continues until the condition becomes false.

- **Example:**
  ```python
  count = 0
  while count < 5:
      print(count)
      count += 1
  ```

- **Output:**
  ```
  0
  1
  2
  3
  4
  ```

- **Dynamic Repetition:** The `while` loop dynamically repeats the code block as long as the condition remains true.
**Example:**
```python
        while temperature > 20:
            print("It's a warm day!")
            temperature -= 1
```

## Infinite Loops

- While loops are powerful, caution must be taken to avoid **infinite loops**, which run indefinitely.
  
- **Example of Infinite Loop:**
  ```python
  while True:
      print("This is an infinite loop!")
  ```
  
- **Caution:**
  - An infinite loop can result in a program that doesn't progress further, leading to resource exhaustion and unintended consequences.
  
- **Avoiding Infinite Loops:**
  - Always ensure there is an **exit condition** in the loop that becomes false at some point to break out of the loop.
  
- **Using `break`:**
  - The `break` statement can be used to forcefully exit a loop. It's often coupled with conditional statements.
  ```python
  while True:
      user_input = input("Enter 'exit' to end: ")
      if user_input.lower() == 'exit':
          break
  ```

## Loop Control Statements

- Loop control statements provide additional control over the flow of loops, allowing for more flexibility in handling specific situations.

- **`break` Statement:**
  - - The `break` statement is used to exit the loop prematurely, regardless of whether the loop condition is still true.
    - It is often used to terminate a loop when a specific condition is met.
  - **Example:**
    ```python
    for i in range(10):
        if i == 5:
            break
        print(i)
    ```
  - **Output:**
    ```
    0
    1
    2
    3
    4
    ```

- **`continue` Statement:**
  - - The `continue` statement is used to skip the rest of the code inside the loop for the current iteration and move to the next iteration.
  - **Example:**
    ```python
    for i in range(5):
        if i == 2:
            continue
        print(i)
    ```
  - **Output:**
    ```
    0
    1
    3
    4
    ```

- **Use Cases:**
  - - `break` and `continue` statements are handy for handling specific conditions within loops, providing more control over the loop's execution.
  - - They help in creating more dynamic and responsive loop structures.

### Slide 9: Nested Loops

- **Nested Loops:**
  - **Definition:** Nested loops involve placing one loop inside another.
  - **Purpose:** To perform more complex and intricate iterations over multiple sets of data.

- **Syntax:**
  ```python
  for outer_item in outer_sequence:
      for inner_item in inner_sequence:
          # Code block to repeat
  ```

- **Example: Multiplication Table**
  ```python
  for i in range(1, 6):
      for j in range(1, 6):
          print(i * j, end="\t")
      print()  # Move to the next line for a new row
  ```
  - **Output:**
    ```
    1    2    3    4    5
    2    4    6    8   10
    3    6    9   12   15
    4    8   12   16   20
    5   10   15   20   25
    ```

- **Explanation:**
  - - The outer loop iterates through each row (1 to 5).
    - The inner loop iterates through each column (1 to 5) for the current row.
    - The multiplication of `i` and `j` gives the values for each cell in the table.

- **Key Points:**
  - - **Hierarchy of Loops:**
        - The inner loop completes its iterations for each iteration of the outer loop.
      - **Example:**
        ```python
        for category in categories:
            for item in items_of_category:
                process(item)
        ```

### Slide 9: Nested Loops

- **Nested Loops:**
  - **Definition:** Nested loops involve placing one loop inside another.
  - **Purpose:** To perform more complex and intricate iterations over multiple sets of data.

- **Syntax:**
  ```python
  for outer_item in outer_sequence:
      for inner_item in inner_sequence:
          # Code block to repeat
  ```

- **Example: Multiplication Table**
  ```python
  for i in range(1, 6):
      for j in range(1, 6):
          print(i * j, end="\t")
      print()  # Move to the next line for a new row
  ```
  - **Output:**
    ```
    1    2    3    4    5
    2    4    6    8   10
    3    6    9   12   15
    4    8   12   16   20
    5   10   15   20   25
    ```

- **Explanation:**
  - - The outer loop iterates through each row (1 to 5).
    - The inner loop iterates through each column (1 to 5) for the current row.
    - The multiplication of `i` and `j` gives the values for each cell in the table.

- **Key Points:**
  - - **Hierarchy of Loops:**
        - The inner loop completes its iterations for each iteration of the outer loop.
      - **Example:**
        ```python
        for category in categories:
            for item in items_of_category:
                process(item)
        ```


