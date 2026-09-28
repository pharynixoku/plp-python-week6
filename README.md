# PLP Python Week 6 Assignment

## Assignment Title
Safe Functions and Error Handling

## Description
This assignment practices Python error handling using `try` and `except`. The program catches specific errors and prevents the program from crashing when it receives invalid input.

## Files

- **`safe_tools.py`** - Contains three safe functions for division, number conversion, and dictionary field lookup.
- **`unbreakable.py`** - Contains the unbreakable program for practicing error handling.
- **`README.md`** - Describes the assignment, files, and error-handling concepts used.

## Functions in safe_tools.py

### `safe_divide(a, b)`
Divides two numbers and returns `Cannot divide by zero` when the second number is zero.

### `safe_number(text)`
Converts text into a whole number. If the text cannot be converted, it returns `Not a number`.

### `get_field(learner, key)`
Looks up a key in a dictionary. If the key does not exist, it returns `Field not found`.

## Why can the `if` check not catch `abc` on its own?

An `if` statement can check conditions, but it does not automatically catch errors caused by converting invalid text to a number. When `int("abc")` is executed, Python raises a `ValueError`, so `try/except` is needed to catch the error and keep the program running.

## Expected Output

```text
5.0
Cannot divide by zero
42
Not a number
82
Field not found
```

## Conclusion

This assignment demonstrates how `try/except` can handle specific errors safely and allow a Python program to continue running instead of crashing.
