---

---

## What is Python?

Python is a dynamically typed, general purpose programming language that supports an       object-oriented programming approach as well as a functional programming approach. Python is an interpreted and a high-level programming language. It was created by __`Guido Van Rossum`__
in 1989. 
## Key Features of Python

-   Python is simple and easy to understand.
-   It is Interpreted and platform-independent which makes debugging very easy.
-   Python is an open-source programming language.
-   Python provides very big library support. Some of the popular libraries include _NumPy,                 Tensorflow, Selenium, OpenCV, Pandas_ etc.
-   It is possible to integrate other programming languages within python.

## Use of python in various Domains

-   Python is used in Data Visualization to create plots and graphical representations.
-   Python helps in Data Analytics to analyze and understand raw data for insights and trends.
-   It is used in AI and Machine Learning to simulate human behavior and to learn from past data     without hard coding.
-   It is used to create web applications.
-   It can be used to handle databases.
-   It is used in business and accounting to perform complex mathematical operations along with     quantitative and qualitative analysis.


# Modules and pip in Python!

Module is like a code library which can be used to borrow code written by somebody else in our python program. There are two types of modules in python:
1. __Built in Modules__ - These modules are ready to import and use and ships with the python interpreter. there is no need to install such modules explicitly. e.g. `int(), float() and list()`
2. __External Modules__ - These modules are imported from a third party file or can be installed using a package manager like `pip or conda`. Since this code is written by someone else, we can install different versions of a same module with time.

## pip command  - package installer for Python

It can be used as a package manager [pip](https://pip.pypa.io/en/stable/) to install a python module.
Lets install a module called pandas using the following command

```bash
pip install pandas
```

## Using a module in Python
We use the import syntax to import a module in Python. Here is an example code:

```python
import pandas as pd

# Read and work with a file named 'words.csv'
df = pd.read_csv('words.csv')
print(df) # This will display first few rows from the words.csv file
 
```


# Comments in python 

A comment is a part of the coding file that the programmer does not want to execute, rather the programmer uses it to either explain a block of code or to avoid the execution of a specific part of code while testing.

- Comments can be used to explain Python code.
- Comments can be used to make the code more readable.
- Comments can be used to prevent execution when testing code.

#### Single-Line Comments:

To write a comment just add a ‘#’ at the start of the line.

### Example 1

```python
#This is a 'Single-Line Comment'
print("This is a print statement.")
``` 

Output:

```markup
This is a print statement. 
``` 

### Example 2

```python
print("Hello World !!!") #Printing Hello World
```

Output:

```markup
Hello World !!!
``` 

### Example 3:

```python
print("Python Program")
#print("Python Program")
``` 

### Output: 

```markup
Python Program
``` 
#### Multi-Line Comments:

To write multi-line comments you can use ‘#’ at each line or you can use the multiline string.

**Example 1:** The use of ‘#’.

```python
#It will execute a block of code if a specified condition is true.
#If the condition is false then it will execute another block of code.
p = 7
if (p > 5):
    print("p is greater than 5.")
else:
    print("p is not greater than 5.")
```


Output:

```markup
p is greater than 5.
```


**Example 2:** The use of multiline string.

```python
"""This is an if-else statement.
It will execute a block of code if a specified condition is true.
If the condition is false then it will execute another block of code."""
p = 7
if (p > 5):
    print("p is greater than 5.")
else:
    print("p is not greater than 5.")
```


### Output

```markup
p is greater than 5.
```

# Escape Sequence Characters

To insert characters that cannot be directly used in a string, we use an escape sequence character.
An escape sequence character is a backslash  `\`  followed by the character you want to insert.
An example of a character that cannot be directly used in a string is a double quote inside a string that is surrounded by double quotes:

```python
print("This doesnt "execute")
print("This will \" execute")
```

Escape Sequence | Description
-------- | -------
| `\\`   | Backslash (`\`)  
| `\'`       | Single quote (`'`) 
| `\"`       | Double quote (`"`)
| `\n` | Newline
| `\t` | Tab
| `\r` | Carriage return
| `\b` | Backspace
| `\f` | Form feed
|`\ooo`| Character with octal value ooo
|`\xhh`| Character with hex value hh




# More on Print statement
The syntax of a print statement looks something like this:

```python
print(object(s), sep=separator, end=end, file=file, flush=flush)
```

## Other Parameters of Print Statement 

1. object(s): Any object, and as many as you like. Will be converted to string before printed
2. sep='separator': Specify how to separate the objects, if there is more than one. Default is ' '
3. end='end': Specify what to print at the end. Default is '\n' (line feed)
4. file: An object with a write method. Default is sys.stdout

Parameters 2 to 4 are optional


# Variables and Data Types
### What is a variable?
Python variables are simply **containers for storing data values**. Unlike other languages, such as Java, Python has no command for declaring a variable, so you create one the moment you first assign a value to it. Python variables are simply containers for storing data values. Variable is like a container that holds data. Very similar to how our containers in kitchen holds sugar, salt etc.
Creating a variable is like creating a placeholder in memory and assigning it some value. In Python its as easy as writing:
```python
a = 1
b = True
c = "AR"
d = None
```

These are four variables of different data types.

### What is a Data Type?

Data type specifies the type of value a variable holds. This is required in programming to do various operations without causing an error.
In python, we can print the type of any operator using type function:
```python
a = 1
print(type(a))
b = "1"
print(type(b))
```

output:

```markup
<class 'int'>
<class 'str'>
```


By default, python provides the following built-in data types:

## 1. Numeric data: int, float, complex


 - int: 3, -8, 0
 - float: 7.349, -9.0, 0.0000001
 - complex: 5 + 4i 
  
 
## 2.Text data: str
 
	str: "Hello World!!!", "Python Programming"

## 3. Boolean data:
    Boolean data consists of values True or False.

## 4. Sequenced data: list, tuple
    

**list:**  A list is an ordered collection of data with elements separated by a comma and enclosed within square brackets. Lists are ``mutable`` and can be modified after creation.

**Example:**

```python
list1 = [8, 2.3, [-4, 5], ["apple", "banana"]]
print(list1)
```


Output:

```markup
[8, 2.3, [-4, 5], ['apple', 'banana']]
```


**Tuple:**  A tuple is an ordered collection of data with elements separated by a comma and enclosed within parentheses. Tuples are ``immutable`` and can not be modified after creation. 

**Example:**

```python
tuple1 = (("parrot", "sparrow"), ("Lion", "Tiger"))
print(tuple1)
```


Output:

```python
(('parrot', 'sparrow'), ('Lion', 'Tiger'))
```


## 5. Mapped data: dict

**dict**: A dictionary is an unordered collection of data containing a ``key:value`` pair. The key:value pairs are enclosed within curly brackets.

**Example:**

```python
dict1 = {"name":"Sakshi", "age":20, "canVote":True}
print(dict1)
```


Output:

```python
{'name': 'Sakshi', 'age': 20, 'canVote': True}
```




# Operators

Operators are used to perform operations on variables and values. Python has different types of operators for different operations. To create a calculator we require arithmetic operators.
# Arithmetic operators

|   Operator             |Operator Name                          |Example                         |
|----------------|-------------------------------|-----------------------------|
|+|`Addition`            |``` 15+7 ```            |
|-|`Subtraction`            |``` 15-7 ```            |
|*|`Multiplication`            |``` 5*7 ```            |
|**|`Exponential`            |``` 5**3 ```            |
|/|`Division`            |``` 5/3 ```            |
|%|`Modulus`            |``` 15%7 ```            |
|//|`Floor Division`            |``` 15//7 ```            |

### Exercise  - a mini calculator

```python
n = 15
m = 7
ans1 = n+m
print("Addition of",n,"and",m,"is", ans1)
ans2 = n-m
print("Subtraction of",n,"and",m,"is", ans2)
ans3 = n*m
print("Multiplication of",n,"and",m,"is", ans3)
ans4 = n/m
print("Division of",n,"and",m,"is", ans4)
ans5 = n%m
print("Modulus of",n,"and",m,"is", ans5)
ans6 = n//m
print("Floor Division of",n,"and",m,"is", ans6)
```
# Explaination
Here 'n' and 'm' are two variables in which the integer value is being stored. Variables 'ans1' , 'ans2' ,'ans3', 'ans4','ans5' and 'ans6' contains the outputs corresponding to addition, subtraction,multiplication, division, modulus and floor division respectively.

[[Mini Calculator | Click to see solution of mini Calculator exercise]]

# Typecasting in python

The conversion of one data type into the other data type is known as type casting in python or type conversion in python.
Python supports a wide variety of functions or methods like: ``int(), float(), str(), ord(), hex(), oct(), tuple(), set(), list(), dict()`` etc. for the type casting in python.

## Two Types of Typecasting:

1. Explicit Conversion (Explicit type casting in python)
2. Implicit Conversion (Implicit type casting in python).
### Explicit typecasting:

The conversion of one data type into another data type, done via developer or programmer's intervention or manually as per the requirement, is known as explicit type conversion. 

It can be achieved with the help of Python’s built-in type conversion functions such as int(), float(), hex(), oct(), str(), etc .
### Example of explicit typecasting:
```python
string = "15"
number = 7
string_number = int(string) #throws an error if the string is not a valid integer
sum= number + string_number
print("The Sum of both the numbers is: ", sum)
```
### Output:
```
The Sum of both the numbers is 22
```
### Implicit type casting:
Data types in Python do not have the same level i.e. ordering of data types is not the same in Python. Some of the data types have higher-order, and some have lower order. While performing any operations on variables with different data types in Python, one of the variable's data types will be changed to the higher data type. According to the level, one data type is converted into other by the Python interpreter itself (automatically). This is called, implicit typecasting in python.

Python converts a smaller data type to a higher data type to prevent data loss.
### Example of implicit type casting:
```python
# Python automatically converts
# a to int
a = 7
print(type(a))
 
# Python automatically converts b to float
b = 3.0
print(type(b))
 
# Python automatically converts c to float as it is a float addition
c = a + b
print(c)
print(type(c))
```
### Ouput:
```
<class 'int'>
<class 'float'>
10.0
<class 'float'>
```


# Taking User Input in python

In python, we can take user input directly by using ``input()`` function. This input function gives a return value as string/character hence we have to pass that into a variable

**input ():** This function first takes the input from the user and converts it into a string. The type of the returned object always will be <class ‘str’>. It does not evaluate the expression it just returns the complete statement as String. For example, Python provides a built-in function called input which takes the input from the user. When the input function is called it stops the program and waits for the user’s input. When the user presses enter, the program resumes and returns what the user typed.
## Syntax:
```python
variable=input()
```

**How the input function works in Python :**   
- When input() function executes program flow will be stopped until the user has given input.
- The text or message displayed on the output screen to ask a user to enter an input value is optional i.e. the prompt, which will be printed on the screen is optional.
- Whatever you enter as input, the input function converts it into a string. if you enter an integer value still input() function converts it into a string. You need to explicitly convert it into an integer in your code using [[#Typecasting in python | typecasting]].
## Example:
```python
variable=int(input())
variable=float(input())
```

We can also display a text using input function. This will make input() function take user input and display a message as well
## Example:
```python
a=input("Enter the name: ")
print(a)
```
## Output:
```
Enter the name: AR
AR
```



