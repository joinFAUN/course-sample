# Control Flow in Python

## What is Control Flow?

Control flow is the order in which statements are executed in a program. In Python, statements are executed from top to bottom, in the order that they appear in the program. However, there are some statements that can change the order in which statements are executed. These statements are called control flow statements.

### if Statements

The `if` statement is used to execute a block of code if a condition is true. The `if` statement has the following syntax:

```python
if condition:
    # code to execute if condition is true
```


### else Statements

The `else` statement is used to execute a block of code if a condition is false. The `else` statement has the following syntax:

```python
if condition:
    # code to execute if condition is true
else:
    # code to execute if condition is false
```

## Examples

### Example 1

```python
if 5 > 2:
    print("5 is greater than 2")
```

Output:

```
5 is greater than 2
```

### Example 2

```python
if 5 < 2:
    print("5 is less than 2")
else:
    print("5 is not less than 2")
```

Output:

```
5 is not less than 2
```