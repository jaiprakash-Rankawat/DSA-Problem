# <CENTER>Python full course (Part 2)</CENTER>

# List 
#### A list is a data structure that can store a collection of items. It is one of the built-in data types and is commonly used to hold an ordered sequence of elements. Lists can contain elements of different data types, including numbers, strings, and even other lists.

# Key features of lists
#### 👉 Lists maintain the order of elements as they are inserted, allowing you to access elements by their index.
#### 👉 You can modify the contents of a list by adding or removing elements.
#### 👉 You can update element of list 

# creating Lists 
```python
# Creating a list of numbers
numbers = [1, 2, 3, 4, 5]

# Creating a list of strings
fruits = ["apple", "orange", "banana", "grape"]

# Creating a mixed-type list
mixed_list = [1, "hello", 3.14, True]

# Accessing elements of a list
print(numbers[0])   # 1
print(fruits[2])    # banana
print(mixed_list[1])  # hello
```

# Updating items
```python
my_list = [1, 2, 3, 4, 5]

# Update the item at index 2
my_list[2] = 10

print(my_list)
```

# Removing / Deleting Items

## Using del
```python
my_list = [1, 2, 3, 4, 5]

# Deleting the item at index 2
del my_list[2]
print(my_list)
```

# Using remove
```python
my_list = [1, 2, 3, 4, 5]

# Removing the value 3 from the list
my_list.remove(3)
print(my_list)
```

# 1D List
```python
my_list = [1, 2, 3, 4, 5]
```

# 2D List
```python
matrix = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
]
```

# 3D List
```python
cube = [
    [
        [1, 2, 3],
        [4, 5, 6],
        [7, 8, 9]
    ],
    [
        [10, 11, 12],
        [13, 14, 15],
        [16, 17, 18]
    ],
    [
        [19, 20, 21],
        [22, 23, 24],
        [25, 26, 27]
    ]
]
```
# Lists Built-In Methods

## append(x)
#### Adds element at the end of the list 

```python
my_list = [1, 2, 3]
my_list.append(4)
# Result: [1, 2, 3, 4]
```

## extend(iterable)
```python 
my_list = [1, 2, 3]
my_list.extend([4, 5, 6])
# Result: [1, 2, 3, 4, 5, 6]
```
## insert(index, element)
```python
my_list = [1, 2, 3]
my_list.insert(1, 4)
# Result: [1, 4, 2, 3]
```
## remove(x)
```python
my_list = [1, 2, 3, 2]
my_list.remove(2)
# Result: [1, 3, 2]
```

## pop(index)
```python
my_list = [1, 2, 3]
popped_element = my_list.pop(1)
# Result: popped_element=2, my_list=[1, 3]
```

## count(x)
```python
my_list = [1, 2, 3, 2]
count_of_2 = my_list.count(2)
# Result: count_of_2=2
```

## sort 
```python
my_list = [3, 1, 4, 1, 5, 9, 2, 6, 5, 3]
my_list.sort()
# Result: [1, 1, 2, 3, 3, 4, 5, 5, 6, 9]
```

## reverse
```python
my_list = [1, 2, 3]
my_list.reverse()
# Result: [3, 2, 1]
```

## copy
```python 
original_list = [1, 2, 3]
copied_list = original_list.copy()
# Result: copied_list=[1, 2, 3]
```
# Iterating over list 

```python 
List = ["ram", "shyam", "Radha", "sita", "hanuman"]
for i in List:
    print(i)
```
# In Operator
#### The in operator is used to check if a specified value is present in a sequence, such as a string, list, tuple, or dictionary. The result is a boolean value (True or False).

## In Strings
```python
text = "Hello, World!"
result = 'o' in text
print(result)  # Output: True
```

## In Lists
```python
numbers = [1, 2, 3, 4, 5]
result = 3 in numbers
print(result)  # Output: True
```

## In Tuples
```python
fruits = ('apple', 'banana', 'cherry')
result = 'banana' in fruits
print(result)  # Output: True
```
## In Dictionaries (Checking Keys)
``` python
person = {'name': 'John', 'age': 30, 'city': 'New York'}
result = 'age' in person
print(result)  # Output: True
```

## In Sets
```python
colors = {'red', 'green', 'blue'}
result = 'yellow' in colors
print(result)  # Output: False
```
## In Substrings
```python
sentence = "Python is powerful"
result = "power" in sentence
print(result)  # Output: True
```

# LIst Unpacking
```python
my_list = [1, 2, 3]

# Unpacking the list into variables a, b, c
a, b, c = my_list
print(a)  # 1
print(b)  # 2
print(c)  # 3
```
# *rest
```python
my_list = [1, 2, 3, 4, 5]

# Unpacking the first two elements, and collecting the rest into a variable
first, second, *rest = my_list
print(first) # 1
print(second) # 2
print(rest) # [3, 4, 5]
```

# Tuples?
#### Tuple is an ordered, immutable collection of elements. This means that once you create a tuple, you cannot modify its contents - you can't add, remove, or change elements in a tuple after it has been created. Tuples are defined by enclosing a comma-separated sequence of values in parentheses ()

# Basic Syntax
```python
my_tuple = (1, 2, 3, 'hello', 3.14)
print(my_tuple[0])  # Output: 1
print(my_tuple[3])  # Output: 'hello'
```
# Error
```python
my_tuple = (1, 2, 3, 'hello', 3.14)
# This will raise an error since tuples are immutable
# my_tuple[0] = 5

# Creating a new tuple with modified content
new_tuple = my_tuple + (5, 'world')
print(new_tuple)  # Output: (1, 2, 3, 'hello', 3.14, 5, 'world')
```

# Dictionaries?
#### A dictionary is a built-in data type that represents a collection of key-value pairs. It is a highly flexible and efficient data structure used for mapping keys to values.

# Key features of dictionaries
#### 👉 Each element in a dictionary consists of a key and its corresponding value. The key is a unique identifier for the value.
#### 👉 Unlike lists, dictionaries are unordered collections, which means the order of elements is not guaranteed.
#### 👉 Dictionaries can be modified after creation. You can add, remove, or update key-value pairs.
#### 👉 Dictionaries can grow or shrink in size as needed.
#### 👉 Each key in a dictionary must be unique. If you try to add a key that already exists, the new value will overwrite the existing one.

# Empty Dictionary 
```python
empty_dict = {}
```
# Dictionary with Key-Value Pairs
```python
student_info = {'name': 'Alice', 'age': 20, 'grade': 'A'}
```

# Using the dict() Constructor
```python
person = dict(name='Bob', age=25, city='London')
```
# Dictionary with Different Data Types
```python
mixed_dict = {'name': 'Charlie', 'age': 30, 'grades': [85, 90, 78], 'is_student': True}
```
# Nested Dictionary
```python
nested_dict = {'person': {'name': 'David', 'age': 22}, 'location': {'city': 'Paris', 'country': 'France'}}
```

# Using a List of Tuples
```python
tuple_list = [('name', 'Eva'), ('age', 28), ('city', 'Berlin')]
from_tuples_dict = dict(tuple_list)
```

# Accessing Items 

## Using Square Brackets
```python
my_dict = {'name': 'John', 'age': 25, 'city': 'New York'}
print(my_dict['name'])  # John
print(my_dict['age'])   # 25
```

## Using the get() Method
```python
my_dict = {'name': 'John', 'age': 25, 'city': 'New York'}
print(my_dict.get('name'))  # John
print(my_dict.get('grade', 'Not Available'))  # Not Available
```
## Iterating Through Keys
```python
my_dict = {'name': 'John', 'age': 25, 'city': 'New York'}
for key in my_dict:
    print(f"{key}: {my_dict[key]}")
```

## Iterating Through Items (Key-Value Pairs)
```python
my_dict = {'name': 'John', 'age': 25, 'city': 'New York'}
for key, value in my_dict.items():
    print(f"{key}: {value}")
```

# Updating Dictionaries ?
## Adding a New Key-Value Pair
```python
my_dict = {'name': 'John', 'age': 25}
my_dict['city'] = 'New York'
```

## Modifying an Existing Value
```python
my_dict = {'name': 'John', 'age': 25}
my_dict['age'] = 26
```
# Updating with Another Dictionary 
```python
my_dict = {"name": "John", "age": 25}
update_dict = {"age": 26, "city": "New York"}
my_dict.update(update_dict)
print(my_dict) #{'name': 'John', 'age': 26, 'city': 'New York'}
```
# Updating with keyword Arguments
```python
my_dict = {'name': 'John', 'age': 25}
my_dict.update(age=26, city='New York')
```
# Deleting in Dictionaries
## del Statement
```python
my_dict = {'name': 'John', 'age': 25, 'city': 'New York'}
del my_dict['age']
```
## pop() Method
```python
my_dict = {'name': 'John', 'age': 25, 'city': 'New York'}
my_dict.pop('age')
```

## popitem() Method
```python
my_dict = {'name': 'John', 'age': 25, 'city': 'New York'}
my_dict.popitem() # remove last element 
```

## clear() Method to Remove All Items
```python
my_dict = {'name': 'John', 'age': 25, 'city': 'New York'}
my_dict.clear()
```

# Sets ?
#### A set is an unordered collection of unique elements. Sets are defined by enclosing a comma-separated sequence of values in curly braces {}. Unlike lists or tuples, sets do not allow duplicate elements, and the order of elements is not guaranteed.

# Example of set 
```python
my_set = {1, 2, 3, 4, 5}
```
# list to set
```python
my_list = [1, 2, 2, 3, 4, 4, 5]
converted_set = set(my_list)
print(converted_set)  # Output: {1, 2, 3, 4, 5}
```