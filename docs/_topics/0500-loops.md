---
title: Loops
layout: post
permalink: /loops/
---

Loops are used to execute a block of code multiple times. There are two types of loops in Python: `while` loop and `for` loop.

The below code prints numbers from 1 to 5 using a loop.

**Example F1**
```python
i = 1
while i <= 5:
    print(i)
    i += 1
```

Now, this is not very helpful because you could have printed the numbers without using a loop.
But what if you did not know how many times you need to print the numbers? For example, how about taking input from the user and printing the numbers that many times?

**Example F2**
```python
n = int(input("Enter a number: "))
i = 1
while i <= n:
    print(i)
    i += 1
```

The expression after the `while` keyword is a condition. The block inside the while will execute as long as the condition is true. The condition is checked before each iteration.

Can you write a loop that never ends?

**Example F3**
```python
while True:
    print("This will print forever")
```

You can use the `break` statement to exit a loop. What will the code below print?

**Example F4**
```python
i = 1
while True:
    print(i)
    i += 1
    if i > 5:
        break
```

Now, the above example is not too useful. Lets say you want to take input of student names, store them in a list, and print them. You will stop taking input when the user enters "no more students".

**Example F5**
```python
students = []
while True:
    name = input("Enter student name: ")
    if name == "no more students":
        break
    students.append(name)
```

**Food for thought**: what would happen if you have the append statement before the break?


There is also a `continue` statement that can be used to skip the rest of the code in the loop and start the next iteration.
For example, you can use the `continue` statement to skip printing a number if it is 3.

**Example F6**
```python
i = 0
while i < 5:
    i += 1
    if i == 3:
        continue
    print(i)
```

There is also a `for` loop which you can use to iterate over a collection. For example, you can use a `for` loop to iterate over a list of student names.

**Example F7**
```python
students = ["Abdullah", "Asad", "Zulqarnayn", "Huzaifa", "Freicy", "Nasrullah"]
for student in students:
    print(student)
```

### Exercises
1. Use a `while` loop to print the list of students.
2. Print the below pattern using a loop.
```
*
**
***
****
*****
```
3. Take a number, `n`, as input, and print `n` rows of the below pattern.
```
*
--
***
----
*****
------
```



