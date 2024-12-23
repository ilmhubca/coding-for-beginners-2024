---
title: Introduction to coding
layout: post
permalink: /intro/
---

## Reading code
Below are some examples of Python code.
What do you think each code does?

**Example A1**
```python
1+2
```

**Example A2**
```python
a = 5
b = 3
sum = a + b
print("The sum is:", sum)
```

**Example A3**
```python
a = int(input("Enter a number: "))
b = int(input("Enter another number: "))
sum = a + b
print("The sum is:", sum)
```

**Example A4**
```python
number = int(input("Enter a number: "))

if number > 0:
    print("The number is positive.")
elif number < 0:
    print("The number is negative.")
```
What is missing in the code above?

## Running code online
Ideally, you would run the code on your computer.
But it will require some installation, so let's start by running them online.
Open [https://www.programiz.com/python-programming/online-compiler/](https://www.programiz.com/python-programming/online-compiler/) and paste any of the code above, then press run.


## Writing your first code
Now that you have seen some code, let's write our first code.
We will use the code editor Visual Studio Code to write code.

First, create a folder on your computer where you will save your code.
Name the folder `<your-name>-cfb` without the angle brackets.
We will use this same folder throughout the course.

Now, open Visual Studio Code and click on `File` > `Open Folder`.
Show the folder you just created and click `Open`.

From within Visual Studio Code, create a new file in the project, and name it `greet.py`.
Copy and paste the code below into the file.

**Example A5**
```python
name = input("Enter your name: ")
print("Salam, " + name + ".")
print("Welcome to Coding for Beginners!")
```

Save the file.

Now it is time to run the code.
We will use the *terminal* in Visual Studio Code to run the code.
Press `Ctrl + ~` to open the terminal.
Alternatively, you can click on `View` > `Terminal`.

In the terminal, type `python greet.py` and press `Enter`.
It will ask your name, and welcome you to the course.

Congratulations! You have written and run your first code.

## Exercises
Try to write the following codes.

- `A6` Write a code that asks the user for their age and prints it.
- `A7` Write a code that asks the user for their name and age, and prints them.
- `A8` Write a code that asks the user for two numbers and prints their sum.
- `A9` Write a code that asks the user for a number and prints `+` if it is positive, `-` if it is negative and `zero` if it is zero.


