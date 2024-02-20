# Operations and Operators in Python

## Introduction

In Python, operations refer to various actions or calculations that can be performed on data using operators. Operators are symbols that represent computations. This guide covers the essential operations and operators in Python, categorized by their types.

## Arithmetic Operators

Arithmetic operators perform basic mathematical operations.


| Operator   | Description          | Example          | Result   |
|------------|----------------------|------------------|----------|
| `+`        | Addition             | `5 + 3`          | `8`      |
| `-`        | Subtraction          | `10 - 4`         | `6`      |
| `*`        | Multiplication       | `2 * 3`          | `6`      |
| `/`        | Division             | `15 / 3`         | `5.0`    |
| `%`        | Modulus              | `17 % 5`         | `2`      |
| `**`       | Exponentiation       | `2 ** 3`         | `8`      |



### Addition (+)

```python
result = 5 + 3  # Output: 8
```

### Subtraction (-)

```python
result = 10 - 4  # Output: 6
```

### Multiplication (*)

```python
result = 2 * 3  # Output: 6
```

### Division (/)

```python
result = 15 / 3  # Output: 5.0
```

### Modulus (%)

```python
remainder = 17 % 5  # Output: 2
```

### Exponentiation (**)

```python
result = 2 ** 3  # Output: 8
```

## Comparison Operators

Comparison operators are used to compare values.


| Operator          | Description                | Example                 | Result   |
|-------------------|----------------------------|-------------------------|----------|
| Equal to (==)     | Checks if two values are equal.   | `5 == 5`           | `True`   |
| Not equal to (!=) | Checks if two values are not equal. | `10 != 5`        | `True`   |
| Greater than (>)  | Checks if the left value is greater than the right value. | `8 > 5`   | `True`   |
| Less than (<)     | Checks if the left value is less than the right value.    | `3 < 7`   | `True`   |
| Greater than or equal to (>=) | Checks if the left value is greater than or equal to the right value. | `10 >= 10` | `True`   |
| Less than or equal to (<=)    | Checks if the left value is less than or equal to the right value.    | `6 <= 4`  | `False`  |



### Equal to (==)

```python
result = (5 == 5)  # Output: True
```

### Not equal to (!=)

```python
result = (10 != 5)  # Output: True
```

### Greater than (>)

```python
result = (8 > 5)  # Output: True
```

### Less than (<)

```python
result = (3 < 7)  # Output: True
```

### Greater than or equal to (>=)

```python
result = (10 >= 10)  # Output: True
```

### Less than or equal to (<=)

```python
result = (6 <= 4)  # Output: False
```

## Logical Operators

Logical operators perform logical operations on boolean values.

### AND (and)

```python
result = (True and False)  # Output: False
```

### OR (or)

```python
result = (True or False)  # Output: True
```

### NOT (not)

```python
result = not True  # Output: False
```

## Bitwise Operators

Bitwise operators perform bit-level operations.


| Operator | Description         | Example            | Result (Decimal) | Result (Binary) |
|----------|---------------------|--------------------|-------------------|-----------------|
| &        | Bitwise AND         | `5 & 3`            | 1                 | `0b0001`        |
| \|       | Bitwise OR          | `5 \| 3`           | 7                 | `0b0111`        |
| ^        | Bitwise XOR         | `5 ^ 3`            | 6                 | `0b0110`        |
| <<       | Left Shift          | `2 << 1`           | 4                 | `0b0100`        |
| >>       | Right Shift         | `8 >> 1`           | 4                 | `0b0100`        |



### AND (&)

```python
result = 5 & 3  # Output: 1
```

### OR (|)

```python
result = 5 | 3  # Output: 7
```

### XOR (^)

```python
result = 5 ^ 3  # Output: 6
```

### Left Shift (<<)

```python
result = 2 << 1  # Output: 4
```

### Right Shift (>>)

```python
result = 8 >> 1  # Output: 4
```

## Assignment Operators

Assignment operators are used to assign values to variables.


Assignment operators are used to assign values to variables.

| Operator | Example     | Equivalent to |
|----------|-------------|---------------|
| `=`      | `x = 10`    |               |
| `+=`     | `x += 5`    | `x = x + 5`   |
| `-=`     | `y -= 3`    | `y = y - 3`   |
| `*=`     | `z *= 2`    | `z = z * 2`   |
| `/=`     | `w /= 4`    | `w = w / 4`   |

- **Assignment (`=`):** Assigns the value on the right to the variable on the left.

- **Add and Assign (`+=`):** Adds the value on the right to the current value of the variable.

- **Subtract and Assign (`-=`):** Subtracts the value on the right from the current value of the variable.

- **Multiply and Assign (`*=`):** Multiplies the current value of the variable by the value on the right.

- **Divide and Assign (`/=`):** Divides the current value of the variable by the value on the right.


### Assignment (=)

```python
x = 10
```

### Add and Assign (+=)

```python
x += 5  # Equivalent to: x = x + 5
```

### Subtract and Assign (-=)

```python
y -= 3  # Equivalent to: y = y - 3
```

### Multiply and Assign (*=)

```python
z *= 2  # Equivalent to: z = z * 2
```

### Divide and Assign (/=)

```python
w /= 4  # Equivalent to: w = w / 4
```

## Membership Operators

Membership operators test whether a value is a member of a sequence.

### In

```python
result = 'a' in 'Python'  # Output: True
```

### Not In

```python
result = 'x' not in 'Hello'  # Output: True
```

## Identity Operators

Identity operators compare the memory locations of two objects.

### is

```python
result = (x is y)  # Output: False
```

### is not

```python
result = (x is not y)  # Output: True
```

