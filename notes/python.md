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
## Operators
### in Operator
Checks whether certain character(s) occur within a string and returns a boolean value.
```py
course = "Python for Beginners"
print("Python" in course)
```
> **Terminal:** True
### Arithmetic Operators
#### Addition ( + )
```py
print(10 + 3)
```
> **Terminal:** 13
#### Subtraction ( - )
#### Multiplication ( * )
#### Division
There are two types of division in Python.

* Single Slash ( / ) returns a float.
* Double Slash ( // ) returns an integer.
```py
print("Float: " + str(10 / 3))
print("Integer: " + str(10 // 3))
```
> **Terminal:**  
Float: 3.33333333333  
Integer: 3
#### Modulus ( % )
Returns the remainder of the division.
```py
print(10 % 3)
```
> **Terminal:** 1
#### Exponent ( ** )
```py
print(10 ** 3) #represents 10 raised to the power 3
```
> **Terminal:** 1000
### Augmented Assignment Operator
An operator in which the assignment operator ( = ) is augmented/enhanced.
#### Example
x = 10  
We want to increment the value of x by 3.
#### Method 1:
```py
x = 10
x = x + 3 #It will add 3 to 10 and store the new value as x
```
Method 2: 
```py
x = 10
x += 3 #achieves the same effect as the expression above
```
* += is the Augmented Assignment Operator in which the assignment operator ( = ) is augmented by +
* We can also augment = with other symbols as per our needs.
### Operator Precedence
* Determines the order in which arithmetic operators are applied.
* Python, like maths, follows the rule of DMAS.
```py
x = 10 + 3 * 2
print(x)
```
> **Terminal:** 16

We can still dictate the order using parenthesis.
```py
x = (10 + 3) * 2
print(x)
```
> **Terminal:** 26
### Comparison Operators
They are used to compare values.
```py
x = 3 > 2
print(x)
```
> **Terminal:** True (3 > 2 is a boolean expression bcz it produces a boolean value)
#### Types of Comparison Operators
* Greater than (>)
* Less than (<)
* Greater than or equal to (>=)
* Less than or equal to (<=)
* Equal to (==)
* Not Equal to (!=)
```py
x = 3 == 2
print(x)
```
> **Terminal:** False

Don't confuse Equality Operator (==) with Assignment Operator (=).
```py
x = 3 != 2
print(x)
```
> **Terminal:** True
### Logical Operators
They are used to build complex rules and conditions.
#### AND Operator
```py
price = 25
#we want to check if the price is between 10 and 30
print(price > 10 and price < 30)
#we can simplify the chained expression as follows:
print(10 < price < 30)
```
When both boolean expressions are true, the result of the entire expression will be true.
> **Terminal:**  
True  
True
#### OR Operator
If atleast one of the boolean expressions is true, then the result of the entire expression will be true.
```py
price = 5
print(price > 10 or price < 30)
```
> **Terminal:** True (because 5 is less than 30)
#### NOT Operator
Inverses any value you give it.
```py
price = 5
print(not price > 10)
```
> **Terminal:** True
## If Statement
* Used to make decisions in programs.
* Print messages on the terminal window depending on the value of the variable.
```py
temperature = 35
```
We want to print a message on the terminal if the temperature rises above 30.
```py
temperature = 35
if temperature > 30: #the block of code will be executed if the condition is true
    print("It's a hot day.")
    print("Drink plenty of water.")
```
> **Terminal:**  
It's a hot day.  
Drink plenty of water.

* In C-based programming languages (C++, C-sharp, Java, JavaScript), we present a block of code with curly brackets.
* In Python, we use indentation instead of curly brackets to present a block of code.
### Adding more conditions
You can add as many conditions as you like.
```py
temperature = 25
if temperature > 30: 
    print("It's a hot day.")
    print("Drink plenty of water.")
elif temperature > 20:
    print("It's a nice day.")
elif temperature > 10:
    print("It's a bit cold.")
else: #this block of code will get executed if none of the above conditions are true
    print("It's cold.")
```
> **Terminal:**  
It's a nice day.

#### Comments
Anything after # is treated as an comment and Python won't execute it.
### Exercise
**Program a weight converter**  
Weight: 170  
(K)g or (L)bs: l or L  
Weight in kg: 76.5
### Solution
```py
weight = float(input("Weight: "))
unit = input("(K)g or (L)bs: ")
if unit.upper() == "K": #.upper() will return the value of the unit variable as uppercase
    print("Weight in lbs: " + str(weight / 0.45))
else:
    print("Weight in kg: " + str(weight * 0.45))
```

















