2024-07-3119:55
Status: #Incomplete 

For automation: playwright library
+matplot, numpy





Teaching yourself new programming languages:

→ Python 3:

*The sys library for Python contains several useful functions

To start writing Python, open up a file with the .py file extension often run through a compiler.

- Python is a language that allows you to easily manipulate imported data.

Variables no longer have to have their type defined. As they are declared by initialization only. Strings can be defined with the usage of single or double quotation marks.

True and False are case sensitive in python

There are only while and for loops in python

Conditional statements look like this:

```python
if y < 43 or (and, and or…) z ==15: 
#code goes here (indentation is important) 
elif y == 43
#code goes here
```

Arrays in C are lists in Python and have some different qualities. For one lists, are not fixed in size, you can delete data easily and you can store different types of variables. (Whereas arrays in C don’t have these functionalities.)

```python
Declaring lists: 
nums = list(), creates an empty list; 2. nums = [x for x in range(500)]. 
```

```python
Adding to a list:  nums = [1,2,3,4]
nums.append(5) //(add to the end), 
#or
nums.insert(4,5) //(insert after 4th term), 
#or 
nums[len(nums):] = [5] //(joining lists)
```

Python statements don’t need to end with semi-colons

No more ++ or — operator

All the data types in C are also present in python although python has some new types (If not they are represented in a more efficient manner. (bools, floats (overflow possible), ints (overflow impossible) and strings(aka str) etc.) New datatypes include:

- range =
- list =
- tuple =
- dict =
- set =
- *Str = Strings in Python are immutable as well as an object. Whereas in C strings are an array of characters/linked list. _You cannot change/append a string in Python where as you (traditionally) could in C_

…

To include libraries in Python, import (library file). If you want a specific function, use the following syntax from (library) import (function name), (function name), …

Python compiles your code for you.

Python is an object oriented language meaning that it is centered around the organization of data rather than functions and logic (an example of a function/logic based language would be C). An object is a collection of data (variables) and methods (functions) that act on that data. Similarly, a class is a blueprint for that object/prototype/template. A module is an object is an object with random attributes so that it can be referenced later. Modules can include runnable code as well as (primarily) define definitions, classes, and variables.

“Python's `property()` is the Pythonic way to avoid formal getter and setter methods in your code**. This function allows you to turn class attributes into properties or managed attributes. Since property() is a built-in function, you can use it without importing anything.”

Because you don’t assign variable types in Python you must declare contingencies for which the user inputs unexpected data. (E.g. you cannot divide a string). The try except function prompts the user for data and when it receives malicious data it outputs a user ‘error’)

`Truncate()` resizes the file to the given number of bytes. If not specified, the current position will be used.

`Trunc()` truncates the value of its argument to a whole number (truncate = cut off)

In Python if the value of an object cannot be changed over time, it it immutable

Constructors are generally used for instantiating an object: `def_int_(self)`: (Newline+ indent # body of the constructor)

Generally in Python there are no pointers, and no need to define global variables.

Positional arguments in Python are variables, objects or values passed into a function or method as an input. They need to included in the proper position in order to be run correctly Whereas named arguments use values as ‘codes’ that produce different outputs

‘end’ within a print function removes the automatically placed new line and joins together two different print functions

Command line arguments in Python are input parameters passed to the script when executing them. `Argv` is a list in python that contains all the command line arguments passed to the script.

*Interpolation is a RNG between two points

In Python, if you decide to open a file you must close it but if you want to open it once, you can use the following format (and not have to close the file): with open … as file

```python
Defining main (Although unnecessary) Follows the following format: (at the end of the file)
if _name_ ==”_main_”: 

         main()


# Source(s)