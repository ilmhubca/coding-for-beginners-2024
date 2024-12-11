---
title: Using and writing functions
layout: post
permalink: /functions/
---

We use functions to group code that performs a specific task. Functions help in organizing code and making it more readable. Functions also help in reusing code.

We previously used built-in functions like `print`, `input`, `int`, `str`, `float`, `len`, etc. We can also write our own functions.
Recall the code we wrote to check if a number is even or odd. We had the below code:

**Example G1**
```python
number = int(input("Enter a number: "))
if number % 2 == 0:
    print("Even")
else:
    print("Odd")
```

We can convert the part of code that checks if a number is even or odd into a function. We will write a function called `is_even` that takes a number as input and returns `True` if the number is even, and `False` otherwise.

**Example G2**
```python
def is_even(number):
    return number % 2 == 0

number = int(input("Enter a number: "))
if is_even(number):
    print("Even")
else:
    print("Odd")
```

Now, this is a simple example. But as the code grows, functions help in organizing the code better.
Lets write a function that takes a year as input and returns `True` if it is a leap year, and `False` otherwise.

**Example G3**
```python
def is_leap_year(year):
    if year % 4 == 0:
        if year % 100 == 0:
            if year % 400 == 0:
                return True
            else:
                return False
        else:
            return True
    else:
        return False
```

In the example above, `year` is the parameter to the function `is_leap_year`. 
The function can *return* a value using the `return` statement.
The parameters are often called "input" and the return value is often called "output".
We can describe the above function as: "The function `is_leap_year` takes a year as input and returns `True` if it is a leap year, and `False` otherwise."

A function can have multiple parameters. For example, lets write a function that takes two numbers, and checks if the first number is divisible by the second number.

**Example G4**
```python
def is_divisible(number, divisor):
    return number % divisor == 0
```

A function can use another function in it.
For example, we can now rewrite the `is_leap_year` function using the `is_divisible` function.

**Example G5**
```python
def is_leap_year(year):
    if is_divisible(year, 4):
        if is_divisible(year, 100):
            if is_divisible(year, 400):
                return True
            else:
                return False
        else:
            return True
    else:
        return False
```


## Exercise
Go over all the code examples we have seen so far, and try to convert them into functions.
