---
title: Data and Variables
layout: post
permalink: /data-and-variables/
---

## Program data
When coding, we are processing data in many ways.
We use *variables* to give names to data.
In the example below, `a`, `b`, and `sum` are variables.

**Example B1**
```python
a = int(input("Enter a number: "))
b = int(input("Enter another number: "))
sum = a + b
print("The sum is:", sum)
```

Now, the names have to be meaningful and related to the data they represent.
For example, `a` and `b` are not meaningful names.

Let's change the names and see if the code makes more sense.

**Example B2**
```python
number_of_kids = int(input("Enter the number of kids: "))
number_of_adults = int(input("Enter the number of adults: "))
total_people = number_of_kids + number_of_adults
print("The total number of people in class:", total_people)
```

In the examples, we will often use not-so-meaningful names to keep the code short.
But when solving a real problem, we should always use meaningful names.

Variables are called variables because their value can change.
For example, in the code below, the value of `a` is changed from 5 to 10.

**Example B3**
```python
a = 5
print(a)
a = 10
print(a)
```

## Assignment
In the examples above, we used the `=` sign to assign a value to a variable.
On the left is the variable name, and on the right is the value.
You can assign a variable to another variable.

**Example B4**
```python
a = 5
b = a
print(b)
```

## Declaring variables
A variable must be declared *before* it is used.
For example, the code below will raise an error.

**Example B5**
```python
print(a)
a = 5
```

## Data types
Data in a program can be of different types.
You can perform different operations on different types of data.

### Numbers
So far, we have only seen numbers, specifically integers.
Numbers can be fractions as well, which are called floating-point numbers, or floats.

**Example B6**
```python
a = 5
b = 3.5
sum = a + b
print("The sum is: ", sum)

c = a / 2
print("Half of a is: ", c)
```

### Text
Text type data are is commonly known as string.
All the *things* you saw between quotes in the code above are strings.

You can *add* strings together, which is called concatenation.

**Example B7**
```python
first_name = "Abdullah"
father_name = "Zubair"

full_name = first_name + " bin " + father_name
print("Full name: ", full_name)
```

### Boolean
Boolean data type can have only two values: `True` or `False`.
Boolean data type is used in conditions and logics, which we will discuss in a later class.

## Type conversion
Recall that when we asked the user for a number, we used the `input` function.
However, the `input` function returns a string, not a number.
Therefore, we used the `int` function to convert the string to a number.
This is an example of type conversion.

**Example B8**
```python
number_as_text = '5'
number = int(number_as_text)
```

Try running the code below. What will it print? `7` or `52`?
```python
number = '5'
print(number + 2)
```

## Exercises
- `B9` Predict the output of the following code before running it:
```python
x = 10
y = x
x = 20
print(y)
```
- `B10` Take a number as input and print its square. For example, if the input is `5`, print `square of 5 is 25`.

## Explore
Try running below examples. If there is an error, read the error and try to understand what went wrong.

**Example B13**
```python
a = "hello"
print(int(a))
```

**Example B14**
```python
a = "5.5"
print(int(a))
```

## More on this topic
For those who are interested, may look into `datetime` and `timedelta` data types.
But we will not cover them in this course.
