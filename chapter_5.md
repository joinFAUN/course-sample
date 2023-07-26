# Error Handling and Exceptions in Python

## What is an Exception?

An exception is an error that occurs during the execution of a program. When an exception occurs, the program stops running and displays an error message. Exceptions can occur for many reasons, including invalid input, missing files, and network problems.

## Handling Exceptions

Exceptions can be handled using the `try` and `except` keywords. The `try` keyword is used to execute a block of code that might raise an exception. The `except` keyword is used to handle the exception that was raised.

```python
try:
    # code that might raise an exception
except:
    # code to handle the exception
```

## Raising Exceptions

Exceptions can be raised using the `raise` keyword. The `raise` keyword is followed by the name of the exception to raise.

```python
raise Exception
```
