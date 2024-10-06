# Python
## Introduction
* It is a multi-purpose programming language and is very helpful is automating repetitive tasks.
* A code editor (IDE) is needed to run Python code and PyCharm is one of the best ones available.
* Python is a case-sensitive language.
## Applications of Python
* Data Science
* Machine Learning
* Web Development (Python + Django Framework)
## Websites Powered by Python
* YouTube
* Instagram
* Spotify
* Dropbox
* Pinterest
## Terminal Window
It displays the output of the Python program when we run it.
## Python Data Types
### String
* It represents a sequence of characters or textual data.
* It is always enclosed in single quotes or double quotes.
#### String Contatenation
Combine one string with another string.
```py
print("Hello " + "Friend")
```
> **Terminal:** Hello Friend
### Number
* **Integer:** represents a whole number
* **Float:** represents a decimal number
### Boolean
* It can be True or False.
## Type Conversion
Converts the value of a variable from one type to another.
```py
birth_year = input("Enter your birth year: ")
age = 2024 - birth_year
print(age)
```
> **Terminal:** TypeError: 'int' and 'str'

The error occurs because the input function will always return a string even if we enter a number in the terminal and Python can't subtract a string from an integer. You have to first convert the string to an integer to do that.
### Int Function
Converts the value to an integer.
```py
birth_year = input("Enter your birth year: ")
age = 2024 - int(birth_year)
print(age)
```
> **Terminal:**  
Enter your birth year: *1996*  
28
### Float Function
Converts the value to a floating point number. In programming languages, it's the number with the decimal point.
### Bool Function
Converts the value to a boolean (True or False).
### Str Function
Converts the value to a string.
### Exercise
Show the following on the Terminal:  
>First: 10.1  
Second: 20  
SUM: 30.1

### Solution
Method 1:
```py
first = input("First: ")
second = input("Second: ")
sum = float(first) + float(second)
print("SUM: " + str(sum))
```
Method 2:  
Pass the value from the input function through the float function before storing it in a variable.
```py
first = float(input("First: "))
second = float(input("Second: "))
sum = first + second
print("SUM: " + str(sum))
```
## Inbuilt Python Functions
### Print
It prints the data within the parenthesis on the terminal window.
```py
print("Hello World")
```
> **Terminal:** Hello World
### Input
Reads a value from the terminal window.
```py
input("What is your name? ")
```
> **Terminal:** What is your name? *John*

After pressing enter, the input function will return the value we entered in the terminal. We can store that value in a variable.
```py
name = input("What is your name? ")
print("Hello " + name)
```
> **Terminal:**  
What is your name? *John*  
Hello John
## Variables
Variables are used to temporarily store data  in a computer's memory.
```py
age = 20
print(age)
```
> **Terminal:** 20

Here age is the variable and 20 is the value that's assigned to it.
```py
age = 20
age = 30
print(age)
```
> **Terminal:** 30

**Imp: Python code gets executed from top to bottom.**

When using multiple words in the name of a variable, separate them with an underscore for better readibility.
```py
unit_price = 19.95
```
We can also assign a string value or a boolean to a variable.
```py
first_name = "Levi"
is_online = True
```
### Exercise
We check in a patient named John Smith. He's 20 years old. He's a new patient.
### Solution
```py
patient_name = "John Smith"
age = 20
status = "new"
print(patient_name, age, status)
```
> **Terminal:** John Smith, 20, new
## Methods
When a function is part of an object, it's called a method.
### String Methods
```py
course = "Python for Beginners"
```
where course is the variable and "Python for Beginners" is a string object.
#### Upper Method
Converts string to uppercase.
```py
course = "Python for Beginners"
print(course.upper())
```
> **Terminal:** PYTHON FOR BEGINNERS

Since **strings are immutable**, methods don't change the original string. Instead a new string is returned each time a method is applied.
#### Lower Method
Converts string to lowercase.
```py
course = "Python for Beginners"
print(course.lower())
```
> **Terminal:** python for beginners

#### Find Method
* Finds a particular character or sequence of characters within a string.
* Returns the index of the first occurence.
* In Python, the index of the first character in a string is 0.
* The Find Method is case-sensitive.
```py
course = "Python for Beginners"
print(course.find("y"))
```
> **Terminal:** 1

#### Replace Method
Replaces character(s) within a string.
```py
course = "Python for Beginners"
print(course.replace("for", "4"))
```
> **Terminal:** Python 4 Beginners













