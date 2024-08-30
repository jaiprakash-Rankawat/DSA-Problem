# <center> Python full course (Part 1) </center>

# Variables 
A variable is used to store and represent data values.

```python
name = "jai prakash"
print("Good Morning", name)
```
`here name is variable`

# updating value 
```python
age = 20
age = 21
print(age) //21
```

# comment 
It is denoted by `#` and it is used to add explanations of code. 

```python
# Age of user is 21
age = 21
print(age)
```

# Identifier
Identifier is a name given to entities like variables, function, classes, modules, etc. It helps to uniquely identify these entities in the program. 

# Rules of Identifier
1. It must start with a letter (a-z, A-Z) or an underscore (_)
2. The remaining characters can be letters, underscores, or digits (0-9)
3. Python is case-sensitive, so variable and Variable are different identifiers.
4. Reserved keywords are not allowed.

# Data type 
Python Data types are the classification or categorization of data items.  
![Remote image](https://media.geeksforgeeks.org/wp-content/uploads/20191023173512/Python-data-structure.jpg)


# Numbers
python provides various ways to work with numbers, including integers, floating-point numbers, and complex numbers.

# Basic Arithmetic operation
```python
num1 = 10
num2 = 3
print(num1 + num2)  # addition
print(num1 - num2)  # subtraction
print(num1 * num2)  # multiplication
print(num1 / num2)  # division
print(num1 // num2) # floor division
print(num1 % num2)  # remainder
print(num1**num2)   # power
```

# Input function
input() function is used to take input from the user during the execution of a program. The input() function reads a line of text from the user as a "string" and returns that "string".
```python
name = input("Enter Your Name :")
print("Good Morning", name)
```

# Assignment Operators
1. ## Assignment (=)
    ```python 
    x = 10  # Assigns the value 10 to the variable x
    ```
2. ## Addition Assignment (+=)
    ```python
    x += 5  # Equivalent to x = x + 5
    ```
3. ## Subtraction Assignment (-=)
    ```python
    y -= 3  # Equivalent to y = y - 3
    ```
4. ## Multiplication Assignment (*=)
    ```python
    z *= 2  # Equivalent to z = z * 2
    ```
5. ## Division Assignment (/=)
    ```python
    a /= 4  # Equivalent to a = a / 4
    ```
6. ## Floor Division Assignment (//=):
    ```python
    b //= 3  # Equivalent to b = b // 3
    ```
7. ## Exponentiation Assignment (**=)
    ```python
    c **= 3  # Equivalent to c = c ** 3
    ```
8. ## Modulus Assignment (%=)
    ```python
    d %= 3  # Equivalent to d = d % 3
    ```

# Strings
A string is a sequence of characters, and it is one of the fundamental data types used to represent textual data.
```python
# Using single quotes
single_quoted_string = 'Hello, World!'

# Using double quotes
double_quoted_string = "Python Programming"

# Multiline string using triple quotes
multiline_string = '''This is a
multiline
string.'''
```
# Concatenation
```python
firstName = "jai prakash"
lastName = "Rankawat"
fullName = firstName + " " + lastName
print(fullName)
```

# String length
```python
name = "jai"
print(len(name)) # 3
```
# String indexing and slicing 
Indexing start from 0 to n-1, where n is length of string.

```python
a ="python"
print(a[0])  # p
print(a[-1]) # n
print(a[1:5])# ytho
```

# String Methods 
```python
name = "Jai Prakash"
about = " i like python "
print(name.upper())
print(name.lower())
print(name.strip()) # strip is used to remove left and right space
print(about.capitalize()) # capitalizes first letter only
print(about.title()) # capitalizes first letter of every word
```

# String Fromating

```python
name ="Jai Prakash"
age = 21
print(f"My name is {name} and i am {age} years old")
# My name is Jai Prakash and i am 21 years old
```
# Escape Characters
```python 

string = "Get text from \n next line"
print(string)
```

# Booleans 
A boolean is a data type that represents one of two values: True or False.
```python
x = True
y = False 
```

# Checking Data type
```python
name = "jai"
age = 21
isPass = False
print(type(name))    # class 'str'>
print(type(age))     # <class 'int'>
print(type(isPass))  # <class 'bool'>
```


# Type Casting 
Type casting refers to the process of converting one data type into another. 

# int()
```python
pi = 3.14
print(int(pi)) # 3
```

# float()
```python
num = 5
print(float(num)) # 5.0
```
# str()
```python
num = 5
print(str(num)) # '5'
```

# bool()
```python
num = 5
print(bool(num)) # True
```

# Some popular String method

```python
file = "index.py"
print(file.startswith("index")) # True
print(file.endswith("py"))      # True
```
```python
name = "jp"
newName = name.replace("jp", "jai prakash")
print(newName) # jai prakash
```
```python
intro = "My name is jai prakash"
print(intro.count("a"))       # 4
print(intro.find("jai"))      # give index value
print(intro.index("prakash")) # give index value

List = intro.split(" ")
print(List) # ['My', 'name', 'is', 'jai', 'prakash']
newIntro = " ".join(List)
print(newIntro) # My name is jai prakash 
```

# Comparison Operators 
Comparison operators are used to compare two values, expressions, or variables. These operators return a boolean value (True or False) based on the comparison result.

# Equality (==)
```python
a = 5
b = 10
result = (a == b)  # Result is False
```
# Inequality (!=)
```python
a = 5
b = 10
result = (a != b)  # Result is True
```
# Greater Than (>)
```python
a = 5
b = 10
result = (a > b)  # Result is False
```
# Less Than (<)
```python
a = 5
b = 10
result = (a < b)  # Result is True
```

# Greater Than or Equal To (>=)
```python
a = 5
b = 5
result = (a >= b)  # Result is True
```

# Less Than or Equal To (<=)
``` python
a = 5
b = 10
result = (a <= b)  # Result is True
```

# Logical Operators
Logical operators are used to perform logical operations on boolean values. These operators allow you to combine or modify boolean values and make more complex decisions in your code.

# Logical AND (and)
```python
x = True
y = False
result = x and y  # Result is False
```
# Logical OR (or)
```python
x = True
y = False
result = x or y  # Result is True
```

# Logical NOT (not)
```python
x = True
result = not x  # Result is False
```

# Conditional Statements 
Conditional statements are used to control the flow of a program based on certain conditions. They allow you to execute different blocks of code depending on whether a specified condition evaluates to True or False.

# if Statement
```python
x = 10

if x > 5:
    print("x is greater than 5")
```

# if - else Statement
```python
x = 3

if x % 2 == 0:
    print("x is even")
else:
    print("x is odd")
```
# if - elif - else Statement
```python
x = 3

if x % 2 == 0:
    print("x is even")
else:
    print("x is odd")
```

# Range 
`range(start, stop, step)`  
range is a built-in function that generates a sequence of numbers within a specified range. It is commonly used with for loops to iterate over a sequence of numbers.

# Loops
Loops allow us to repeatedly execute a block of code as long as a certain condition is met or iterate over a sequence of elements. Python supports two main types of loops: for loops and while loops.

# for loop
```python
# program to genrate table 
number = int(input("Enter Number :"))
for i in range(1, 11):
    print(f"{number} x {i} = {number*i}")
```

# while loop 
```python
# program to find factorial of a number 
number = int(input("Enter Number :"))
fact = 1
if number > 0:
    while number != 0:
        fact = fact * number
        number += -1
elif number == 0:
    print("Factorial : 1")
else:
    print("please Enter a valid Input")
print("Factorial :", fact)
```