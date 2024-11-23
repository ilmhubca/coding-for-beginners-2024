---
title: Operators
layout: post
permalink: /operators/
---
We used some operators in the previous lessons.
For example, we used the `+` operator to add two numbers, as well as to join (or concatenate) two strings.
For example:

**Example C1**    
```python
sum = 5 + 3
join = "5" + "3"

print(sum)
print(join)
```

## Arithmetic operators
Arithmetic operators are used to perform mathematical operations.

**Example C2**
```python
a = 5
b = 3
print("addition", a + b)
print("subtraction", a - b)
print("multiplication", a * b)
print("division", a / b)
print("modulus", a % b)
print("exponent", a ** b)
print("floor division", a // b)
```

## Comparison operators
Comparison operators are used to compare two values.
Result of comparison operators is a boolean value: `True` or `False`.

**Example C3**
```python
a = 5
b = 6
print("greater than", a > b)
print("less than", a < b)
print("equal", a == b)
print("not equal", a != b)
print("greater than or equal", a >= b)
print("less than or equal", a <= b)
```

String data can also be compared using comparison operators.

**Example C4**
```python
city_1 = "Edmonton"
city_2 = "Calgary"
print("greater than", city_1 > city_2)
print("less than", city_1 < city_2)
print("equal", city_1 == city_2)
print("not equal", city_1 != city_2)
print("greater than or equal", city_1 >= city_2)
print("less than or equal", city_1 <= city_2)
```

## Logical operators
`and`, `or`, and `not` are logical operators.
`and` and `or` are used to combine two boolean values.

For example, if you want to check if a number is between 3 and 10, you can use the `and` operator.

**Example C5**
```python
number = 5
print("between 3 and 10", number > 3 and number < 10)

number = 2
print("between 3 and 10", number > 3 and number < 10)
```

`or` operator is used to check if at least one of the conditions is true.  

**Example C6**
```python
number = 5
print("either 3 or 10", number < 3 or number > 10)
```

`not` operator is used to negate a boolean value.

**Example C7**
```python
number = 5
print("not 3", not number == 3)
```

When the expressions are complex, you can use parentheses to group them.
For example, to check if a number is between 3 and 10 or between 20 and 30, you can write:
**Example C8**
```python
number = 25
print("between 3 and 10 or between 20 and 30", (number > 3 and number < 10) or (number > 20 and number < 30))
```


## Assignment operators
We have used the assignment operator `=` to assign a value to a variable.
There are also `+=`, `-=`, `*=`, `/=`, `%=`, `**=`, and `//=` operators to perform the operation and assign the result to the variable.

**Example C9**
```python
a = 5
a += 3
print(a)
```

The above code is equivalent to:
**Example C10**
```python
a = 5
a = a + 3
print(a)
```

## Operator precedence
When multiple operators are used in an expression, the order of evaluation is determined by the precedence of the operators.
For example, multiplication and division have higher precedence than addition and subtraction.
You can use parentheses to change the order of evaluation.

**Example C11**
```python
result = 5 + 3 * 2
print(result)
```

The above code is equivalent to:
**Example C12**
```python
result = 5 + (3 * 2)
print(result)
```

But if you want to add 5 and 3 first, you can use parentheses.
**Example C13**
```python
result = (5 + 3) * 2
print(result)
```

For a complete list of operators and their precedence, see the [Python documentation on operator precedence](https://docs.python.org/3/reference/expressions.html#operator-precedence).

## Exercises
You may need `if`, `elif`, and `else` statements to solve the following exercises.
We will discuss details about these statements in the next lesson. However, we did use them in the previous lessons a little bit, which should be enough to solve these exercises.

1. `C14` Write a program that takes input a month of the year as number and prints the number of days in that month. If February, print `28 or 29`.
   
2. `C15` Write a program that takes input two numbers. The first one is the month, and the second one is the day of the month. Print `Yes` if the date is valid, otherwise print `False`. If the date is valid for some years but not for others, print `Maybe`.

3. `C16` Write a program that takes input a number and prints `Yes` if the number is a multiple of 3 and 5, otherwise print `No`.

4. Build a simple calculator that takes input two numbers and an operator (`+`, `-`, `*`, `/`) and prints the result.

5. Write a program that takes input three numbers and prints the largest and smallest among them.