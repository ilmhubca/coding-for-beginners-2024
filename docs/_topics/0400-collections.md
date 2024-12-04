---
title: Collections
layout: post
permalink: /collections/
---

Collections are used to store multiple values in a single variable. Python has several built-in collection data types: `List`, `Set`, `Dictionary` etc. 

### Lists
Lets say we want to store the names of students in a class. We can use a list to store the names of students. 

**Example E1**
```python
students = ["Abdullah", "Asad", "Zulqarnayn", "Huzaifa", "Freicy", "Nasrullah"]
print("number of students in the class:", len(students))
print(students)
```

The `len()` function is used to get the number of elements in a list.

You can access the elements of a list using their *index*. The index of the first element is 0, the index of the second element is 1, and so on.

**Example E2**
```python
print(students[0])
print(students[3])
```

You can also use negative indices to access elements from the end of the list. The index of the last element is -1, the index of the second last element is -2, and so on.

**Example E3**
```python
print(students[-1])
print(students[-4])
```

You can add elements to a list using `append()`.
**Example E4**
```python
students.append("Ahmed")
print(students)
```

You can remove elements from a list using `remove()`.
**Example E5**
```python
students.remove("Ahmed")
print(students)
```

You can also remove elements by their index using `pop()`.
**Example E6**
```python
students.pop(4)
print(students)
```

You can use the `in` operator to check if an element is present in a list.
**Example E7**
```python
if "Ali" in students:
    print("Ali is in the class")
if "Asad" in students:
    print("Asad is in the class")
```

Similarly, you can use the `not in` operator to check if an element is not present in a list.
**Example E8**
```python
if "Ali" not in students:
    print("Ali is not in the class")
if "Asad" not in students:
    print("Asad is not in the class")
```

### Sets
Sets are like lists, but they do not allow duplicate elements.

For example, if we want to know the countries where each students were born, we wouls use a set.

**Example E9**
```python
countries = {"Pakistan", "Bangladesh", "Dominiac Republic"}
print(countries)
```

Now, lets say another student registers, and he is from India. We can add his country to the set using `add()`.
**Example E10**
```python
countries.add("India")
print(countries)
```

Now, yet another student from Dominiac Republic registers. We can add his country to the set using `add()`.

**Example E11**
```python
countries.add("Dominiac Republic")
print(countries)
```
Notice that Dominican Republic still appears only once in the set.

Similar to lists, you can use the `in` operator to check if an element is present in a set.

**Example E12**
```python
if "Pakistan" in countries:
    print("Pakistan is in the set")
if "USA" in countries:
    print("USA is in the set")
```

### Dictionaries
Lists can be used to store values in sequence of indexes starting from 0. But what if we want to store values with custom indexes? For example, we want to store the age of each student. We can use a dictionary to store the age of each student.

**Example E13**
```python
ages = {
    "Abdullah": 11,
    "Asad": 10,
    "Zulqarnayn": 12,
    "Huzaifa": 12,
    "Freicy": 23,
    "Nasrullah": 32
}
print(ages)
```

You can access the values of a dictionary using their keys.
**Example E14**
```python
print(ages["Abdullah"])
print(ages["Freicy"])
```


### More on collections
There are more collection types and operations built-in to python. But these are the basics that you need to know to get started with collections.


### No exercises
We will skip the exercises for this topic because it is difficult to have meaningful exercises on collections without learning loops, which is the next topic.

