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
## Terminal
- It displays the output of the Python program when we run it.
- Comments are prefixed with the # symbol. They don't get executed.
## Python Data Types (Basic/Primitive)
### String
* It represents a sequence of characters or textual data.
* It is always enclosed in single quotes or double quotes.
```py
print("Hello World")
print("1") # represents the character '1' and not the number '1'
```
> **Terminal:**  
Hello World  
1
### Number
1) **Integer:**  
Represents a whole number.
2) **Float:**  
Represents a decimal number
3) **Complex Number:**  
    * It's created from two real numbers.
    * It's written in the form of $x + yj$ where $x$ and $y$ are real numbers and $j$ is an imaginary number called **iota**. The value of iota is $\sqrt{-1}$
    * It can be created directly (e.g. $1 + 3j$) or by using the complex function.
    ```py
    z = complex(1, 3)
    print(z)
    ```
    > **Terminal:** (1+3j)
### Boolean
* It's binary in nature.
* It can be either True or False.
#### Boolean Expression
An expression that produces a boolean value when evaluated.
```py
print(1 > 5)
```
> **Terminal:** False
## Python Data Types (Complex)
Useful in building real applications.
### Lists
- Used to store a sequence of objects and is **mutable**.
- Defined by square brackets [ ]
- Individual objects within a list are separated by commas.
```py
names = ["John", "Bob", "Mosh", "Sam", "Mary"]
values = [1, 2, 'a', 3]
print(names)
print(values)
```
> **Terminal:**  
['John', 'Bob', 'Mosh', 'Sam', 'Mary']  
[1, 2, 'a', 3]

We can also retrieve individual objects from the list by calling their index within square brackets.
```py
names = ["John", "Bob", "Mosh", "Sam", "Mary"]
print(names[0])
```
> **Terminal:** John

In Python, we can also call negative indexes, a feature not available in other programming languages.
```py
names = ["John", "Bob", "Mosh", "Sam", "Mary"]
print(names[-1]) # -1 refers to the last object in the list
```
> **Terminal:** Mary

We can also change an object in the list at a particular index.
```py
names = ["John", "Bob", "Mosh", "Sam", "Mary"]
# we want to change the spelling from John to Jon
names[0] = "Jon"
print(names)
```
> **Terminal:** ['Jon', 'Bob', 'Mosh', 'Sam', 'Mary']

We can also print a range of values from the list.
```py
names = ["John", "Bob", "Mosh", "Sam", "Mary"]
# we want to print John, Bob and Mosh
print(names[0:3])
# where:
# 0 is the starting index
# 3 is the ending index which should be +1 to the index of the object you want to print
```
> **Terminal:** ['John', 'Bob', 'Mosh']
### Tuples
- Like lists, they are used to store a sequence of objects.
- They are **immutable**, meaning they cannot be changed after creation.
- They are defined by ( )
- Like lists, they are **ordered** which means you can refer to an item by its index.
- Tuples don't support item assignment. Unlike a list, we can't replace an item in a tuple afterwards.
```py
numbers = (1, 2, 3)
numbers [0] = 10
```
> **Terminal:** TypeError: 'tuple' object does not support item assignment
### Sets
- A set is a collection which is unordered, immutable and unindexed.
- **Unordered:** The items in a set do not have a defined order. Set items can appear in a different order every time you use them.
- **Immutable:** Once a set is created, you cannot change its items, but you can remove items and add new items.
- **Unindexed:** Set items cannot be referred to by index or key.
- Sets are defined by curly brackets and **don't allow duplicates**.
```py
values = {1, 2, 2, 3, 4, 1, 'm', 5, 'a'}
print(values)
```
> **Terminal:** {'a', 1, 2, 3, 4, 5, 'm'}

As you can see, all the duplicates are removed and the set items appear out of order.
### Dictionaries
- A dictionary is a collection of **key : value pairs**.
- Dictionaries are ordered, it means that the items have a defined order, and that order will not change.
- In a real dictionary, a specific word maps to its definition. So when you look up a word, you're actually looking for the definition. The word only acts as the key.
- In Python, dictionary works the same way. Values are assigned keys and you look up the value by entering the key.
- Dictionaries are defined by curly brackets.
```py
emm = {1:"a", 2: "b", 3: "c"}
print(emm[1]) # 1 is the key
```
> **Terminal:** a

Dictionaries are **mutable**, meaning that we can change, add or remove items after the dictionary has been created.
```py
emm = {1:"a", 2: "b", 3: "c"}
emm[1] = "e"
print(emm)
```
> **Terminal:** {1: 'e', 2: 'b', 3: 'c'}

Dictionaries **don't allow duplicates**. There can't be two items with the same key. Duplicate values will overwrite existing values.
```py
car_specs = {
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964,
  "year": 2020
}
print(car_specs)
```
> **Terminal:** {'brand': 'Ford', 'model': 'Mustang', 'year': 2020}
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
### Len
Returns the numbers of characters in a string.
```py
language = "Python"
print(len(language))
```
> **Terminal:** 6

Returns the number of items in a list.
```py
numbers = [1, 2, 3, 4, 5]
print(len(numbers))
```
> **Terminal:** 5
### Range
Returns a sequence of numbers, starting from 0 by default, and increments by 1 (by default), and **stops before a specified number**.
```py
numbers = range(5) # will return a range object
print(numbers)
```
> **Terminal:** range(0, 5)

range(0, 5) is the default representation of a range object and represents numbers 0 till 4. In order to see the actual numbers, we need to iterate over this range object using a for loop just like we iterate over a given list.
```py
numbers = range(5)
for number in numbers:
    print(number)
```
> **Terminal:**  
0  
1  
2  
3  
4

We can also define the starting point ourselves instead of the default value of 0.
```py
numbers = range(5, 10)
# where:
# 5 is the starting number
# 10 is the ending number which is to be excluded
for number in numbers:
    print(number)
```
> **Terminal:**  
5  
6  
7  
8  
9

We can also define the incremental value ourselves instead of the default value of 1.
```py
numbers = range(5, 10, 2) # 2 is the incremental value
for number in numbers:
    print(number)
```
> **Terminal:**  
5  
7  
9

You don't need to store the range function in a separate variable. You can use it directly as part of a for loop.
```py
for number in range(5):
    print(number)
```
> **Terminal:**  
0  
1  
2  
3  
4
## Variables
- Variables are used to temporarily store data in a computer's memory.
- They are declared using the assignment operator (=).

If `x = 5` and `y = x` then both variables (**x** and **y**) point to the value 5.

![alt text](<Screenshot 2024-12-06 120746.png>)

If we change `x = "cake"` then only **y** keeps pointing to the value 5.

![alt text](<Screenshot 2024-12-06 120803.png>)

Variable names can only contain alphanumeric characters and underscores. That means no special characters are allowed.
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

Variable names can only start with an alphabetical character or underscore.
```py
city = 'London'
_year = '2024'
print(city + _year)
```
> **Terminal:** London2024

When using multiple words in the name of a variable, separate them with an underscore for better readibility.
```py
unit_price = 19.95
```
Variable names are case-sensitive.
```py
KAREN = 'Manager'
karen = 'Employee'
print(f'{karen} reports to {KAREN}.')
```
> **Terminal:** Employee reports to Manager.

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
- Objects in programming are like objects in the real world. They have certain capabilities.
- When a function is part of an object, it's called a method.
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

### List Methods
```py
numbers = [1, 2, 3, 4, 5]
```
Lists are also objects, so they have certain methods available.
#### Append Method
Adds a new value at the end of the list.
```py
numbers = [1, 2, 3, 4, 5]
numbers.append(6)
print(numbers)
```
> **Terminal:** [1, 2, 3, 4, 5, 6]

#### Insert Method
Inserts the specified value at the specified position.
```py
numbers = [1, 2, 3, 4, 5]
numbers.insert(0, -1)
# where:
# 0 is the index of the specified position
# -1 is the specified value
print(numbers)
```
> **Terminal:** [-1, 1, 2, 3, 4, 5]

#### Remove Method
Removes the first occurrence of the element with the specified value.
```py
numbers = [1, 2, 3, 4, 3, 5]
numbers.remove(3)
print(numbers)
```
> **Terminal:** [1, 2, 4, 3, 5]

#### Clear Method
Clears all values in a list.
```py
numbers = [1, 2, 3, 4, 5]
numbers.clear()
print(numbers)
```
> **Terminal:** [ ]
### Tuple Methods
Tuples have certain methods available:
#### Count Method
Returns the number of occurences of an element.
```py
numbers = (1, 3, 2, 3)
print(numbers.count(3))
```
> **Terminal:** 2
#### Index Method
Returns the index of the first occurence of a given element.
```py
winners = ("Harry", "Ron", "Hermoine", "Luna", "Harry")
print(winners.index("Luna"))
print(winners.index("Harry"))
```
> **Terminal:**  
3  
0
#### Magic Methods
These methods start with an underscore.
## Operators
### Membership Operators
#### in Operator
Checks whether certain character(s) exist within a string and returns a boolean value.
```py
course = "Python for Beginners"
print("Python" in course)
```
> **Terminal:** True

Checks whether certain item(s) exist within a list/tuple/set and returns a boolean value.
```py
numbers = [1, 2, 3, 4, 5]
letters = {'a', 's', 'd', 'f'}
print(1 in numbers)
print(1 and 6 in numbers)
print('s' in letters)
```
> **Terminal:**  
True  
False  
True

Checks whether certain keys exist within a dictionary.
```py
countries = {'GER':'Germany', 'FRA':'France', 'ENG':'England'}
print('GER' in countries)
```
> **Terminal:** True
#### not in Operator
Checks if a value is **not present** in an iterable, returning True if the value is not found and False if the value is found.
```py
numbers = [1, 2, 3, 4, 5]
countries = {'GER':'Germany', 'FRA':'France', 'ENG':'England'}
print(2 not in numbers)
print(6 not in numbers)
print('ENG' not in countries)
```
> **Terminal:**  
False  
True  
False
### Arithmetic Operators
#### Addition ( + )
```py
print(10 + 3)
```
> **Terminal:** 13

You can also concatenate strings and lists using the + operator.
```py
print("Hello " + "Friend")
print([1, 2] + ['a', 'b'])
```
> **Terminal:**  
Hello Friend  
[1, 2, 'a', 'b']
#### Subtraction ( - )
```py
print(10 - 3)
```
> **Terminal:** 7
#### Multiplication ( * )
```py
print(10 * 3)
```
> **Terminal:** 30
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
### Assignment Operator (=)
Assigns a value to a variable.
```py
x = 3
print(x)
```
> **Terminal:** 3
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
> **Terminal:** True (3 > 2 is a boolean expression that produces a boolean value)
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

**Don't confuse Equality Operator (==) with Assignment Operator (=).**
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
## Loops
### While Loops
Used to repeat a block of code multiple times. The while loop will keep executing the block of code until the while condition is no longer true.
```py
i = 1 # i is the loop variable
while i <= 5:
    print(i)
    i = i + 1
```
> **Terminal:**  
1  
2  
3  
4  
5

In Python, we can multiply a number with a string and it will repeat that string based on the value of the number.
```py
i = 1
while i <= 10:
    print(i * "P")
    i += 1
```
> **Terminal:**  
P  
PP  
PPP  
PPPP  
PPPPP  
PPPPPP  
PPPPPPP  
PPPPPPPP  
PPPPPPPPP  
PPPPPPPPPP  
### For Loops
Used to iterate over a sequence and access each item individually.
```py
numbers = [1, 2, 3, 4, 5]
for item in numbers:
    print(item)
# item is the loop variable. In each iteration, it will hold one value.
```
> **Terminal:**  
1  
2  
3  
4  
5

The for loop prints each 'item' within the 'numbers' list on a seperate line.
#### Exercise
Achieve the same result as above but this time, use a while loop instead.
#### Solution
```py
numbers = [1, 2, 3, 4, 5]

i = 0  
while i < len(numbers):
    print(numbers[i]) # 'i' acts as the index
    i += 1
```
> **Terminal:**  
1  
2  
3  
4  
5


















