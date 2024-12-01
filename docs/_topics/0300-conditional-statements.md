---
title: Conditional statements
layout: post
permalink: /conditionals/
---

Programming involve making decisions based on certain conditions. 
Conditional statements are used to execute different code blocks based on certain conditions.
The basic conditional statement in Python is the `if` statement, which we have already seen in the previous lessons.
Then there are `elif` and `else` statements that can be used to add more conditions to the code.
Let's see some more examples to understand the conditionals better.

**Example D1**
Take an integer as input and print whether it is odd or even.
```python
number = int(input("Enter a number: "))
if number % 2 == 0:
    print("Even")
else:
    print("Odd")
```

**Example D2**
Take a number as input and print whether it is a whole number or a fraction.
```python
number = float(input("Enter a number: "))
if number % 1 == 0:
    print("Whole number")
else:
    print("Fraction")
```

**Example D3**
Take a number as input and print whether it is a whole number or a fraction. If it is a whole number, print whether it is odd or even.
```python
number = float(input("Enter a number: "))
if number % 1 == 0:
    print("Whole number")
    if number % 2 == 0:
        print("Even")
    else:
        print("Odd")
else:
    print("Fraction")
```

## Exercises
1. Write a program that takes input a month of the year as number and prints the number of days in that month. If February, print `28 or 29`.
2. Write a date validator program that takes as input a month, and year, and prints whether the date is valid or not. Accept both 28 and 29 days for February.
3. Take a year as input and print whether it is a leap year or not. A leap year is divisible by 4. But if it is divisible by 100, it is not a leap year. However, if it is divisible by 400, it is a leap year. For example, 2000 is a leap year, but 1900 is not.

