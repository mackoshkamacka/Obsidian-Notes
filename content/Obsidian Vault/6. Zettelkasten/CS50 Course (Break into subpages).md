2024-06-2501:05
Status: #Complete 
## LECTURE 0: INTRO
![[input_output.png]]

Binary (or sometimes referred to as assembly/machine code):

- 0s and 1s = on and off, Binary = a pattern of on/off switches (aka transistor)
- e.g. 0101 (in binary)= 5(in decimal)
- ASCII = assigning binary values to symbols and characters → the newer code = Unicode to include characters (16 bits) 65 thousand characters → Unicode universalizes the meaning of codes to characters (and its up to the manufacturer of a device to visualize, whether it be emojis (android vs. apple) or font)

Hexadecimal:
RGB  = __ __ __ F= full, 0 = nothing → HEX = 1,2,3,4,5,6,7,8,9,A,B,C,D,E,F (e.g. 00FF00 = green, FFFFFF =  white)

When playing a video = x frames per seconds, a composition of switches that represent colors display an image. → A sequence of 0s and 1s. The same concept applies to other formats of output audio and other ways to represent binary.
In order to save space, compression is used → lossy and lossless (as well as ZIP files)
* Lossy = some info lost, lossless = no info lost (just records patterns)
* An algorithm = step by step instructions
* An algorithm is when a computer takes an element of a variable or other piece of information, manipulating this information to follow a set of instructions.
* Pseudocode = An outline of how a problem given should be solved. (crashes and loading screens are sometimes attributed to unaccounted possibilities)
* Functions: Actions/verbs that solve smaller problems
* Conditionals: Based off of some qualities, specific functions must be executed.
* Boolean expressions: True/False
* Loops: A sequence of code that
## LECTURE 1: C (LANGUAGE)

Command line interface (CLI)--> Linux +vs. GUI
(IDEs = Text editors --> Use Visual Studio Code )
(Source code --> Compiler --> Machine code)
A terminal window allows you to run commands on code you create ($)

Header files = a menu of functions for example #include <stdio.h> and  <#include cs50.h> = are extensions to C

### Console Commands
- $ ./((file name)) = run file
- make = compile code
- cd = change directory --> current directory = ".", parent directory = ".." e.g. cd (name of directory)
- cp = copy --> duplicate a file
- cp - r = copy recursive --> duplicate an entire directory
- ls = list --> allows you to list all the different files/projects in a folder
- mkdir = make directory -> (make a new folder)
- mv = move -> e.g. ($mv lmao.c lol.c)
- rm = remove file
- rm -r = remove directory
- rm -f = remove file (force)
- rm -rf = remove directory forcefully --> very dangerous command lmao
- rmdir = remove directory
- cd ../.. go back
- cd (by itself)
- code (new file name) = create a new file
- ./ = this directory
- ctrl+l = clear directory
### Data types in C
Integer values (=4 bytes) --> range = -2^31 - 2^31 - 1 (apx. 4 billion total)
(Qualifiers) Unsigned integer --> an integer value that ignores negative values

 * bool = true/false
* char = a singular letter/symbol
* double = long decimal value
* float = decimal values
* int = whole numbers
* long = long integer values
* string = a string of characters
* %_

- Char = 1 bit (256 values) --> ASCII
- Floating point numbers (=4 bytes) --> A real number containing a decimal value.
- Double (=64 bytes) Acts like a float but has more information
- Void (is just a type (not a data type)) --> Doesn't return any information = doesn't take any arguments
- Bool = True/false
- String = A collection of characters
- Structs + type defs

(cast ___ (insert type here)) = convert to a different type
(float) y (when y is an integer --> it can be converted to a )


Constant = you cannot change a variable's properties,
### Operators
- $+$ = addition
- $-$ = subtraction
- / = divide
- * = multiply
* % = remainder (modulus)
* <,<=, >,>= = inequalities
* == = equal to
* != = not equal to
* || = or (boolean expression)
* && = and  (boolean expression)
* != not/bang = inverses true/false (boolean expression)
* ++ = +1
* -- = -1
// = notes within code
int counter = counter + 1;
(can also be written as...) counter+=1;  (you can use i as counter var.)

- → It remembers the datatype and by using the += operator, you can simplify the program

### Source
printf("hello world");
Side affect = visual output
Return values =
string answer  = get_string("What's your name? ");
string/int = specifies what variable is, answer = variable, get_string()= function, "x" = displayed text
(=) assignment operator
$\n$ = writes a new line
printf("hello, %s\n", answer);
= %s put a string placeholder
= %i put a integer placeholder
To start a program use
int main(void)
{
... put all main code in here
}
### If Else Conditionals 
```c
if //(boolean-expression)
{... }

if //(boolean-expression)
{... }

else
{...}

if//(boolean-expression)
{... }

else if
{...}

else
{....}

//(lack of breaks will entail a fall of cases)

int x = GetInt ();
switch(x)
{
case 1:
printf("One!\\n")
break;
case 2:
printf("Two!\\n")
break;
case 3:
printf("Three!\\n")
break;
default:
printf("Sorry!\\n")
}

int  x =  (expr) ? 5: 6;
//a very fast way of expressing an if else statement
```
``` c
//Loops:
//Forever loop:

While (true)
{...}

Repeat until loop:
While (expression)
{...}

//Use when the number of times used is unknown (maybe not at all)
//Do-while loop:

Do
{...}
while (expression);
//Use when you want the expression to run at least once

For loop
for (int i = 0; i < 10; i++(expression))
//for (start; expr; increment)
//set i as 0, and repeat an expression 10 times
//use for loops when you want an expression to be run a specified amount of times
```

```c
//Setting an array example
int n = get_int(”How many tests did you have?”)
int score [n]; 
for (int i = 0; i < n; i++1)

{
scores [i] - get_int(”Score:”); 
}
```
### Loops
```c
//Loops:
//Forever loop:

While (true)
{...}

Repeat until loop:
While (expression)
{...}

//Use when the number of times used is unknown (maybe not at all)
//Do-while loop:

Do
{...}
while (expression);
//Use when you want the expression to run at least once

For loop
for (int i = 0; i < 10; i++(expression))
//for (start; expr; increment)
//set i as 0, and repeat an expression 10 times
//use for loops when you want an expression to be run a specified amount of times
```

```c
//Setting an array example
int n = get_int(”How many tests did you have?”)
int score [n]; 
for (int i = 0; i < n; i++1)

{
scores [i] - get_int(”Score:”); 
}
``` 
## LECTURE 2: ARRAYS
$ clang = directly compiles code, allows for code to act in specific ways when converted to machine code (E.x $clang-o hello hello.c, -o = output)

a.out = assembly output

Compiling
- Preprocessing (#telling the compiler to find/trust that the prototypes used are real and should not output an error) Copy pasting the #…’s actual code in place of #… so that the program can actually run.
- Compiling = converting code into assembly language (basic instructions)
- Assembly = converting assembly language to binary
- Linking = stiches all libraries and code together e.g. (The binary of your code, library A, library B are all now linked together)

### Debugging
By using printf(), you can see the values assigned to strings and have a closer look into what might be causing an issue

There are also debugger commands that tell you what’s happening within your code one step at a time. (they modify only compiled code). To note it can tell you the value of a variable.

Rubber duck = explaining your code out loud to an inanimate object (duck >:))

Step over = stepping over a line, step into = stepping into a function

Int manipulated by int will output an int. An int manipulated by a float will output a float

Arrays store multiple variables of the same kind of variable in different locations denoted by their location in “[]” E.x. bool battleship[10][10] (Having two indexes allows for grid like storage) Arrays ARE passed by reference i.e. they are global regardless of if they’re in a function or not.

By adding (value type) after a variable allows you to convert a variable type from one to another

Strings are just an array of characters, characters have an ASCII value, and therefore a binary value

Nul character = \0 separates strings/values

Manual pages for functions (use CS50 version)

int main(int argc, string argv[]) =

It should be noted that `argv` is itself not a string, it is collection of string type objects. Let me tell you the structure of parameter `argv[]`(assuming that you wrote `hello.c`).

```c
argv[] = {"./hello", "This", "is", "CS50"} // this is correct
// and not argv[] = "./hello This is CS50"   //this is wrong
```

So now the following stand for the respective objects :

1. `argv[0]` for `./hello` and not for `'.'`
2. `argv[1]` for `This` and not for `'/'`
3. `argv[2]` for `is` and not for `'h'`
4. `argv[3]` for `CS50` and not for `'e'`

I think now it would be clear. Good Luck.

Exit status reasons to quit code through CLI, (having main return a non-zero value e.g. 1) e.g. ERROR 404

Functions (procedures, methods, subroutines) are black boxes with a set of 0+ inputs and 1 output

e.g. a=3, b=6, c=7, add(a, b, c) → 16

Functions allow programmers to write less code and to organize/simplify their code. It also allows for smoother debugging and reusability

Function declarations are established so that the computer knows what the program is saying. (Establishing a ‘shortcut’)

They are all structed like this:

Return-type[the kind of output] name[meaningful name of function](argument-list)[comma separated inputs to your function, each of which have a time and name]; Then using {}, add what the function does

```c
E.x. int add_two_ints(int a, int b); 
{
int sum = a + b
return sum;
}
```

Functions can have void input or output in which they output or take in no arguments

Variable scope

If a variable is within a function is is a local variable and cannot be referenced in future lines of code, where global variables can.

When referencing a global variable, you are making ‘copies’ of when used in functions. To manipulate the variable you must be overwritten to be changed

argc = count the amount of strings, argv = store an array of string values

## LECTURE 3: ALGORITHMS 
Searching:
Efficiency can be determined by a program’s overall time taken to execute, storage take, any redundancy etc. its efficiency can be denoted by ‘O’

![[Untitled.png]]

As n functions infinitely increase they are all denoted by n regardless of their rate (O), whereas log n functions are much more efficient and can be denoted by log (O) etc.

For optimal efficiency, n is as low as possible, when n is equal a constant, it has been optimized

Order of efficiency from worst (n = high) to least (n is low)

- O(n)
- O(n log n)
- O(n^2)
- O(log n)
- O(1)

The difference between Big O notation and Big Ω notation is that Big O is used to describe the worst case running time for an algorithm. But, Big Ω notation, on the other hand, is used to describe the best case running time for a given algorithm.

If the efficiency between Ω and O are the same it is denoted by theta

Linear search searching from top to bottom for a specific value

O = n in that it takes n amount of times to find the desire value

Ω = 1 because the minimum amount of searches that can be taken = 1 (if the desired value happens to be the first one listed)

Data structures:

Example of encapsulation of multiple data types that can be of differing types:

```c
typedef struct 
{
string name; 
string phone number;
}
person;
int main(void) 
{
person people[n];
people[0].name = “Carter”;
people[0].number = “4126736272”;
```

Selection sort = Theta (n^2) → General expression

![[Untitledalg.png]]
Recursion = using the same function within itself to reduce redundancy of code often denoted by (n!) = fact(n) (as ! is used to express an inversion). You need to implement a base case to break the loop of recursion, otherwise it will repeat forever. It will call itself in a slightly altered way. e.g. n==1 (fact(1) =1)

Merge sort is a general, efficient way to sort an array of numerical values (Much more efficient than bubble sort and selection sort (ew)) it is denoted by n log n (more efficient than bubble and selection sort both denoted by O(n^2))

![[huh.png]]

Linear search = look for x value from left to right (if first is not desired value, then move to next value) If value is not found, return 1 or any number that isn’t 0

Binary search = Sort data, then reduce the search area by half each time, trying to find the target number (repeat until sub array size is 0) If not = to the median of data see if its in the lower or upper half. Repeat this process until value is found. If not found, sub array is still size zero”

Bubble sort = Move higher values to the end of an array and the smaller values to the beginning of the array

= set swap counter == a non-0 value, repeat until swap counter is 0 (making no more swaps) Reset swap counter to 0, look at each adjacent pair (if two elements are not in order, swap them and add 1 to the swap counter) MOVING BIGGEST TO THE RIGHT. Because it works from left to right, it is slower than selection sort. 


## LECTURE 4: MEMORY
HEX (I’m not relearning this) an x between two values treats the data as a hexadecimal value. = memory addresses

A pointer value stores the location of a byte value. The address is denoted by a single ‘&’ to store the address of that variable, use an asterisk before the variable (int *p = &n) By utilizing this you can sometimes access pieces of memory outside the program, i.e. hack >:))

The Pointer in C, is **a variable that stores address of another variable**. A pointer can also be used to refer to another pointer function. A pointer can be incremented/decremented, i.e., to point to the next/ previous memory location. The purpose of pointer is to save memory space and achieve faster execution time.

A string is really a pointer to the address of the first character of a string, trusting that the last value will be \0, the computer knows when the string starts and ends

Copies of variables don’t store the same location of the variable that they are referencing.

Often values in a string are next to one another thus you can use pointer arithmetic to determine their location. E.x. str s=“hi”, $*$s=h, *(s+1)=i . This is why when you compare two strings with ‘== ,' you get an error. By using pointer values, you can more accurately compare two addresses or strings.

Additionally when you assign variables to have a value and then copy that variable, they end up referencing the same address. Thus by modifying the value, you edit both the original variable and copied variable.

Malloc asks for more memory to use, allowing memory to be designated in a dynamic fashion. Malloc returns 4 bits data, and array of total four (0 indexed)

Free allows you to deallocate/release memory block which have previously been allocated by calloc(), malloc() or realloc() functions

To check if a pointer is valid or not use “pointer variable == NULL”

### Summary of pointer values:
Pointers provide an alternative way to pass data between functions. Previously only able to pass copies of values, pointers allow you to reference an address that a data value is at. By editing the data stored at a specific address, you can manipulate. Storage lives on a HHD or a SSD = ROM, Ram is where data can be manipulated, having a storage of 512MB-4GB of memory (in arrays of 8-bit wide bytes) = volatile data

To extract the address of an already existing variable, use the ‘&’ operator. E.g. y=&x (where x stores the int 45 and &x = the address of x) y is now has the value of 45 and executing operations with y now on, manipulates the x value globally. If arr is an array of doubles, then &arr[i] is a pointer to the double who has the i-th address in the element arr. Thus arrays are really just pointers. 

![[oioih.png]]

If you don't set your pointers to null, then you may be tampering with data from other programs. (If not something meaningful) To create multiple pointers on the same line follow this format (int *px, *py, *pz;)

Dynamic memory allocation can be utilized thanks to pointers getting access to a block of dynamically allocated memory at runtime. This pool of memory is HEAP memory. (Prior to this point only stack memory has been used) Malloc(memory allocator)(size of (int)) will give you a pointer that allows you to utilize memory in the heap. If there is no more memory, it will return a null pointer. (using this memory will return a segmentation fault) Once you’re done using the data, you must free the memory, otherwise your program will crash due to a memory leak. To do this use free()

Call stacks: When you call a function, the system sets aside memory for that function to do its necessary work i.e. stack frames or function frames. Additionally more than one function’s stack frame may exist in memory at a given time. If main() calls move(), which then calls direction(), all three of these functions have open frames. The active frame is at the top of the stack where it is easiest to access.

![[ijoijp.png]]

Once the base case has been completed, (fact(1)), it then moves on to complete the next executable function (fact (2)) until all have been completed. 

Now you can store values of other variables to have the same address of another variable, and as well as manipulate the value.

### File Pointers
$[$int = 4 bytes$][$char = 1 byte$][$lfoat = 4 bytes$][$double = 8 bytes$][$long long= 8 bytes$][$strings=char * = 4 or 8 as they reference the address of the first character of a string and \0$]$

Segmentation faults are a result of using garbage pointees. If you don’t dedicate space for values to be stored, and manually try to give a value it will end up taking a random piece of storage, becoming a garbage value.

int* x;
x = malloc (sizeof(int));
*x = 42 (directly allocates a value into specified piece of storage)

tmp

File pointers:
In order to store persistent data on a computer, you must introduce a FILE pointer. Common file pointers include, fopen(), fclose(), fgetc(), fputc(), fread(), fwrite()

fopen() opens a file and returns a file pointer to it (always check the return value to ensure the return value is not NULL) written as: (FILE* ptr = fopen(<filename>, <operation>) An example of an operation is ‘r’ meaning read the file, w = write(overwrite/new) and a = append (edit/write)

fclose(<file pointer>); closes the file and is the co-operator of fopen()

fgetc() reads and returns the next character from the file pointed to. Can only be used when fopen() is read = r. Written as (char ch = fgetc(<file pointer>);)

EOF means end of file. (Looping fgetc(ptr) and then printing each character, until the EOF, will display the contents of the file in text

fputc() writes or appends a specified character to the pointed to file. (fopen() must have undergone the operation w or a in order for fputc() to function) It is written as fputc(”character”, “location” (e.g ptr2)); This now allows you to copy to files.

fread() Reads <qty> units of <size> from the file pointed to and stores them in memory in a buffer (usually an array and malloc can be used) <buffer> File must be opened and read before operating fread(). Written as:

int arr[qty]

fread(<buffer>, <size>, <qty>, <file pointer>);

fwrite() Writes whatever file has been pointed to (that had been operated by a or w, and follows the same formating of fread(); from buffer to file instead of vice versa

Additional functions

fgets() Reads a full string from a file. fputs() Writes a full string to a file.

fprintf() Writes a formatted string to a file. fseek() Allows you rewind or fast-forward within a file.

ftell() Tells you at what (byte) position you are at within a file. feof() Tells you whether you've read to the end of a file.

ferror() Indicates whether an error has occurred in working with a file.


## LECTURE 5: DATA STRUCTURES

Qualities of arrays:

- Insertion is bad - lots of shifting to fit an element in the middle
- Deletion is bad - lots of shifting to remove an element
- Lookup is great - index allows for random access at constant time
- Relatively easy to sort
- Relatively small size-wise
- Stuck with a fixed size, no flexibility

Singly Linked lists are made of nodes. A node contains the variable and a pointer to the next value in that list,. The variable can be of multiple types containing more than 1 piece of data. It can be thought of as a chain. There is no index allocated to these lists.

```c
typedef struct sslist
{
VALUE val; 
struct sslist* next;
}
sslnode;
//Temporary name of sslist as it is refering to itself 
```

Creating a new node into the linked list: sslnode* insert(sslnode*head, VALUE val); This inserts a value to the beginning of a list (It will return a pointer to the new head of the list. Always set a link the new element before stating what the head is. This minimized the chance at orphaning the list.

Pseudo code:

1. Dynamically allocate space for a new sllnode
2. Check to ensure there is memory (pointer != NULL)
3. Populate and insert the node at the beginning of the list
4. Return a pointer to the new head of the linked list

Deleting the entire linked list: Void destroy(sslnode* head) Remove every other element in a list and then the first value. This is typically done with recursion. Base case= Null pointer

Linear search: bool find(sslnode* head, VALUE val);

Doubly linked lists (dll) are similar to singly linked lists, only that they contain an extra pointer to the previous value in the list. This allows you to more easily delete nodes (by connecting two surrounding nodes and orphan the unwanted value). This is done with the same steps as linked lists except between the 3rd and 4th step, you must fix a PREV pointer of the old head of the linked list to allow for insertion of new values.

Deleting a node: void delete(dllnode* target); *There are extra steps for deleting the first and last element of a list.

Linked lists always take constant time to insert data at the expense of randomly accessing values (linear time)

Qualities of linked lists:

- Insertion is easy - track onto front
- Deletion is easy - (double list) once you find the first element
- Lookup is bad - relies on linear search
- Relatively difficult to sort
- Relatively small, although not as small as arrays


Hash tables have a theta efficacy that approaches a constant as the data itself indicates its location in the data structure. The trade off being an inability to sort data.
The elements of a Hash table include a has function that returns a hash code, a non-negative value and an array compatible with sorting the desired datatype

![[hash-table.png]]

A hash function should incorporate all elements of value in its function, as well as only the data’s information. It should also output the same value every time. It should also output data uniformly as well as out put very different hash codes for very different pieces of data. *Use hash functions made by other people to avoid collisions/errors.

Collisions occurs when a hash function returns t the same hash code for two different pieces of data. A solution to this is utilizing linear probing (adding 1 to the hash code for example). The downside to using this is that it doubles the chance of future collisions. A buildup a hash values that don’t match the placement of their original value, leads to clustering.

Chaining eliminates clustering by replacing the storage of data with the storing of linked lists. If a new piece of data collides with a hash code it just adds onto the linked list of values that have the same hash code.

Qualities of a hash table:

- Insertion is a two step process - hash then add
- Deletion is easy - just finding the element
- Lookup is on average better than with linked lists because you have the benefit of a real-world constant factor (although linear) 1/n
- Not an ideal data structure if sorting is the goal -just use an array
- Varying size although generally larger than linked lists but smaller than tries

### Tries 

Tries guarantee a unique key and with a value that could be a Boolean that tells you whether it exists in the structure or not. Tries are linked lists can be thought off as trees that branch off at differing elements:

***Set a variable equal to the root or any other important pointer to avoid manipulating that variable

```c
typedef struct _trie
{
char string[x];
struct _trie* paths[y];
}
trie;
```

Where x is at the location of where its path ends and where y = to the amount of paths created when a new branch is made. Often = the number of ASCII digits.

Searching a trie looks for the end of a path (NULL pointer) and if the data found matches what was searched for, it returns true.

This data structure comes at the expense of storage for time (constant theta).

*Dictionaries are an application of tries
![[trie.png]]

Qualities of tries:

- Insertion is complex although it gets easier as you go
- Deletion is easy, just free node/orphan node
- Lookup is fast although not as fast as an array
- Already sorted as it is built into the structure
- Rapidly becomes huge, even when very little data is present. Memory heavy

### Memory Allocation Commands 
malloc() = memory allocates a size of byte memory, returning a pointer to the first byte. If there is an error, it will return NULL. Follow this format: (type*) malloc(sizeof(type)); where type refers to any variable type, e.x. int, char etc.

free() = deallocates memory

calloc() = similarly to malloc, calloc allocate memory but the difference is that it initializes all bytes in the allocation block to zero, because its uses to reserve space for dynamic arrays. Formatted like this (type*) calloc(num,size); where num specifies the size in bytes of one element to the secont argument (size). If the partitioning is successful, the address is returned. If not NULL is returned. *calloc() is slower than malloc because it clears all the memory before usage.

calloc() is basically malloc() + memset()

realloc() is used to reallocate the memory space which has already been initialized. It increases or reduces the allotted space at a later stage in the program. Format: sp=realloc(sp,size); where sp is the pointer variable, and size is the number of bytes newly allotted.

[https://webeduclick.com/malloc-vs-calloc-vs-realloc/](https://webeduclick.com/malloc-vs-calloc-vs-realloc/)

[](https://jraleman.medium.com/c-programming-language-functions-malloc-calloc-realloc-and-free-61cfc3e45da7#:~:text=Also%2C%20take%20note%20that%20calloc,memory%20block%20on%20the%20heap)[https://jraleman.medium.com/c-programming-language-functions-malloc-calloc-realloc-and-free-61cfc3e45da7#:~:text=Also%2C](https://jraleman.medium.com/c-programming-language-functions-malloc-calloc-realloc-and-free-61cfc3e45da7#:~:text=Also%2C) take note that calloc,memory block on the heap.

### Arrows in C 
`(pointer_name)->(variable_name)`

`foo->bar` is equivalent to `(*foo).bar`, i.e. it gets the member called `bar`from the struct that `foo`points to. The operator ‘.’ is used to access the child object of…
#### Bucket sort: 
![[what-is-bucket-sort-algorithm.webp]]

### Priority
FIFO = First in first out system/priority hierarchy
LIFO = Last in first out system/priority hierarchy
Queues = a FIFO system
Enqueue = add (an item of data awaiting processing) to a queue of such items.
Dequeue = a double ended que, where both the first and last items of a list take the highest priority and the middle takes the least.
Abstract data structures/type (ADTs) is a data type that is not defined by its concrete data but its behavior. E.g. Arrays, Lists, table, tries, trees, vectors etc. Real life example = telephone number book

## LECTURE 6: PYTHON

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

All of the data types in C are also present in python although python has some new types (If not they are represented in a more efficient manner. (bools, floats (overflow possible), ints (overflow impossible) and strings(aka str) etc.) New datatypes include:

- range =
- list =
- tuple =
- dict =
- set =
- *Str = Strings in Python are immutable as well as an object. Whereas in C strings are an array of characters/linked list. _You cannot change/append a string in Python where as you (traditionally) could in C_

…

To include libraries in Python, import (library file). If you want a specific function, use the following syntax from (library) import (function name), (function name), …

Python compiles your code for you.

Python is an object oriented language meaning that it is centered around the organization of data rather than functions and logic (an example of a function/logic based language would be C). An object is a collection of data (variables) and methods (functions) that act on that data. Similarly a class is a blueprint for that object/prototype/template. A module is an object is an object with random attributes so that it can be referenced later. Modules can include runnable code as well as (primarily) define definitions, classes, and variables.

“Python's property() is **the Pythonic way to avoid formal getter and setter methods in your code**. This function allows you to turn class attributes into properties or managed attributes. Since property() is a built-in function, you can use it without importing anything.”

Because you don’t assign variable types in Python you must declare contingencies for which the user inputs unexpected data. (E.g. you cannot divide a string). The try except function prompts the user for data and when it receives malicious data it outputs a user ‘error’)

Truncate() resizes the file to the given number of bytes. If not specified, the current position will be used.

Trunc() truncates the value of its argument to a whole number (truncate = cut off)

In Python if the value of an object cannot be changed over time, it it immutable

Constructors are generally used for instantiating an object: def_int_(self): (Newline+ indent #body of the constructor)

Generally in Python there are no pointers, and no need to define global variables.

Positional arguments in Python are variables, objects or values passed into a function or method as an input. They need to included in the proper position in order to be run correctly Whereas named arguments use values as ‘codes’ that produce different outputs

‘end’ within a print function removes the automatically placed new line and joins together two different print functions

Command line arguments in Python are input parameters passed to the script when executing them. Argv is a list in python that contains all the command line arguments passed to the script.

*Interpolation is a RNG between two points

In Python, if you decide to open a file you must close it but if you want to open it once, you can use the following format (and not have to close the file): with open … as file

```python
Defining main (Although unnecessary) Follows the following format: (at the end of the file)
if _name_ ==”_main_”: 

         main()
```

## LECTURE 7: SQL

Manipulating data in Python E.x.=favorite show (data from google survey)

```python
#Data processing 
#google forms (E.x.= favourite show) -> (convert to) excel -> csv file -> python
import csv

with open("favorites.csv", "r") as file:
    reader = csv.reader(file)
    next(reader)
#next skips the first row of the imported data
    for row in reader:
        print(row[1])
#prints out the first row (E.x.= favourite show title) 
```

```python
import csv
titles = []

with open("favorites.csv", "r") as file:
    reader = csv.DictReader(file)
#DictReader creates a dictionary from each row, allowing for access to each row by name
#DictReader uses the first row as the column names 
    for row in reader:
				title = row["title"].strip().upper() 
#.strip().upper() makes all titles upper case = canonicalized/standardized 
        if not row ["title"] in titles: 
						titles.append(row["title"])

for title in titles:
print(title) 
```

The most common way to save large amounts of information digitally is through the usage of databases. Similarly to programs like excel, databases are organized by a set of rows and columns.

SQL (the Structured Query Language) is the most powerful database program. Its purpose if to query a database. MySQL is one open-source platform on which you can establish the type of relational database that SQL is best at working at. SQLite is a less storage heavy version. Several installations of SQL come with a GUI(Graphical user interface) tool called phpMyAdmin which can be used to execute queries in a more user friendly way. It is most commonly used to create tables and databases as the syntax for making them is complicated. (You will be prompted to specify the columns of the table, then the majority of the queries executed will be on the rows )

storing in files/folders using python

Data types in SQL:

[INT][SMALLINT][TINYINT][MEDIUMINT][BIGINT][DECIMAL][FLOAT][BIT][DATE][TIME]DATETIME][TIMESTAMP][CHAR = one character = fixed 1 string][VARCHAR][BINARY][BLOB][TEXT][ENUM][GEOMETRY = mapping data][LINESTRING = mapping data]…

Primary keys enable rows of a table to be uniquely identified, (basically an index). You should have these values automatically increment as new information is being added (and be an int).

Joint primary keys are two columns that are always guaranteed to be unique

*SQL has very limited vocabulary

- SELECT extracts information from a table Use ’*’ to select all the columns (after <columns>)
- SELECT (JOIN) joins information across two different tables
- INSERT adds new information to the table
- UPDATE modifies information in a table

→ Other operations include: [AVG][COUNT][COUNT][DISTINCT][LOWER][MAX][MIN][UPPER][WHERE][LIKE][ORDER BY][LIKE][GROUP BY]

```sql
//**SELECT (JOIN)**
SELECT 
<columns>
FROM
<table1>
JOIN
<table2>
ON
<predicate>
```

```sql
//SELECT
SELECT <columns>
FROM 
<table>
WHERE <predicate>
ORDER BY 
<column>

```

```sql
//INSERT
INSERT INTO 
<table> 
(<columns>) 
VALUES 
(<values>)

```

```sql
//**UPDATE** 
UPDATE 
<table>
SET 
<column> = <value> 
WHERE
<predicate>
```

```sql
//DELETE 
DELETE FROM
<table>
WHERE
<predicate>

```

#### SQL Operations 

key =lambda
. = any character
.* = 0 or more characters
.+ = 1 or more characters
? = optional
^ = start of input
$ = end of input

relational database
create table table(column type, …);
.mode csv
.import
b tree
sequel attacks
?
rare conditions
atomic
interacting with databases at the same time as another user

## LECTURE 7.5: CYBERSECURITY
Passwords

Brute force attacks → Trying every combination to crack a code (4 digit password = least secure → multicharacter 8+ digit password) ‘Try again later’ is a response

Password managers generate passwords, and provide a key to access all of your passwords stored on various different sites.

Two factor identification is about having one digital-password and some sort of physical verification

Encryption scrambles messages using a key. → http(s):// (s) = secure/encrypted (may not be end to end)

Incognito mode: Doesn’t truly make you ‘invisible’ as websites, sever holders and internet providers can access what you’re viewing. (MORE)

End to end encryption:
![[E2EE.png]]

## LECTURE 8: HTML, CSS, JavaScript

Web-programming

The internet is a connection of networks physically connected through cables and wires. A router being a node in that network. Hardware knowing what router information it has.

TCP (Transmitting control protocol) Is the fragmentation splits up a file’s information (in order to reassemble) and if there is any information missing it will notice it. It also guarantees delivery. Marking the source address and TCP specifies what kind of service it is sending. Port 80= Website, Port 443 = Encrypted Website, Port 25 = SMTP = email, Port 53 = DNS

IP makes the sources address and recipient address. IPs #.#.#.# = 32bit, now 128bit → IPv6 = 8 clusters of HEX Omitting of 126 bit IP addresses with large chunks of zeroes can be written in the following format. 2001:4567:9807:0:0:0:0:9876 = 2001:4567:9807::9876

IP’s (Internet Protocol) public router address is connected to other routers locally. The central point of their connection is connected to a larger framework that connects networks on a global scale. It has multiple path in case traffic on a specific path is too jammed

DHCP (Dynamic host configuration protocol) assigns IP addresses

Domain name system (DNS) connects IP addresses to (Fully qualified) domain names. Large DNS servers (like Google’s) collect smaller sets of DNS information and pool them together, updating them frequently.

Access points: The IP address is assigned to a router, whose job is to act as a traffic cop that allows data requests from all of the devices on your local network (home/business etc.) to be processed through the same IP address

HTTP Standardizes how the web (built on top of the internet) interacts with the user. It is an application layer protocol (other examples include: FTP, SMTO, DDS, RDP, XMPP etc.) which specifically dictates the format by which clients request web pages from a server and the format via which servers return information to clients.

http(s)://www.example.com/folder/file/html www.=subdomain .com=commercial http(s)


```html
//GET: Requests information from the
server and the client gets response
GET/HTTP/1.1
Host: www.example.com
...

//Response 
HTTP/1.1 200 OK 
Content-Type: text/html
... 
```

![[internet-diagram.gif]]


```html
Seeing these messages using the curl function 
200 0K [success]
301 Moved Permanently [redirection] (safetyschool.org) (harvardsucks.org) 
302 Found [redirection temporarily]
304 Not Modified 
307 Temporary Redirect 
401 Unauthorized [not logged in]
403 Forbidden [not intended for clients to access]
404 Not found [doesn't exist on the server]
418 I'm a Teapot (<https://www.google.com/teapot>) 
* 500 Internal Server Error [server end error] 
503 Service Unavailable [timeout]
... 
```

![[oihoihoi.png]]

HTML (Hypertext Markup Language) is a language but not a programming language as it lacks variables, logic, function etc. It is a markup language, using angle bracket enclosed tags to semantically define the structure of a web page, causing the plain text inside of sets of tags to be interpreted by web browsers in different ways.

```html
//Example of 'Hello world' on a website
<html>
//Indicates that the language being used
	<head> 
//What shows in the tab of your browser
		<title> 
//Displayed text 
			Hello, world 
		</title> 
//Closes the operation (done automatically) 
	</head> 
	<body> 
//content of the page 
		World hello 
	</body>
</html> 

==
<html><head><title>Hello, world</title></head><body>World, hello</body></html>
//Removed white space

```

```html
//Common HTML tags 
<b>, </b> //Where it bolds the surrounded text 
<i>, </i> //Text is in itallics 
<u>, </u> //Text is underlined 
<p>, </p> //Text is rendered as a paragraph 
<hX>, </hX> //Where x is = to level section header (size of header) 
<ul>, </ul> //Demarcate an unordered, bulleted list 
<ol>, </ol> //Demarcate the beginning and end of an ordered (numbered) list
<li>, </li> //Demarcate list items with an ordered or unordered list 
<table>, </table> //Demarcate the beginning and end of a table definition 
<tr>, </tr> //Demarcate the begining and end of a row within a table
<td>, </td> //Demarcate the begining and end of a column within a row within a table
<form>, </form> //Demarcate the begining and end of an HTML form (
<div>, </div> //Demarcate the begining and end of an arbitrary HTML division
<a href=X>, </a> //Creates a hyperlink to a webpage X, with tw=ext being refered to as linked text
<!DOCTYPE html> //Specific to HTML5, lets browser know that's the standard you're using 
<!--,--> //Demarcates the begining and end of a comment <!--,(comments)-->  
<img scr=X.../> // Displays an image located at X (has additional attributes, such as specifying width/height) 
<input nuam=X type=Y/> // (Self closing tags) Define a field withing an HTML form. X is a unique ID for theat field, Y is what data type it accepts 
```

CSS (Cascading Style Sheets) is also a language used to construct websites. While HTML is used to make the website functional, CSS is used for the aesthetic aspects of a website. A common way to include CSS information into a HTML file is through linking

```css
/*Example of property usage:*/
body'
{
background-color: blue; 
} 
```

```css
//Common CSS porperties
border: style color width
backgroun-color: [keyword e.g.blue|Hex code]
color: [keyword e.g.blue|Hex code] -> ususally applies to text
font-size: [absolute size|relative size]
font-family: [font name|generic name]
text-align: [left|right|center|justify]
```

```css
//ID attributes, an ID selector will apply to an HTML tag with a unique identiifier'
#unique 
{
	border: 4px dotted blue; 
	text-align: right; 
} 
```

```css
//Classes are selectors that will apply only to those HTML tags that have been given identical class attributes'. 
.students 
{
	background-color: yellow;
	opacity: 0.7;
}
```

### JAVASCRIPT

JavaScript is a language built off of C that is run on the client’s side. Just like CSS with<style> tags, you can directly write your JavaScript between <scrip> tags. You can also write JavaScript in separate files and link them in by using the scr attribute of the <script> tag . JavaScript can behave like an object oriented language, where an object is similar to a structure in C. Where elements of the structure are called fields, members or properties. There are also methods which operate like functions that only operate on the object it is manipulating. [object.function();]

*Getbootstrap is a library that allows for easy formatting in HTML, CSS and JavaScript

Variables in JavaScript are similar to Python, the only difference is a need to distinct the variable with the var keyword.

Loops and If statements are identical in JavaScript to C

Additional loops in JavaScript:

```jsx
//Redux loop = itterate an operation across an array of data
for //(var key in object) 
{
	//use object[key] in here 
}
//or 
for //(var key of object) 
{
	// use key in here
}
```

```jsx
//Mapping methods onto objects operates across the entire array
var nums = [1,2,3,4,5];
nums = nums.map(function(num) {
	return num * 2; 
});
$2,4,6,8,10
```

All functions are introduced with the function keyword. JavaScript functions, particularly those bound specifically HTML elements can be anonymous (you don’t have to assign a name)

Array declaration: vars nums = [1,2,3]; *you can also have different variable types, vars mixed = [true,’two’, 3]

Events are a responce to user interaction with a webpage

[https://www.example.com/path?key=value](https://www.example.com/path?key=value)

Common events that can be listened for: [blur][change][click][drag][focus][keyup][load][mousedown][mouseover][mouseup][submit][touchmove][unload]

DOC (Document Object Model) is an object inn JavaScript that nests all of the objects and data within a website into one object. Its structure is similar to that of tries in C.

```jsx
//Common DOM properties
innerHTML //Holds the HTML inside a set of HTML tags 
nodeName // The name of an HTML element or element's attribute 
id // The 'id' attribute of an HTML element 
parentNode // A reference to the node one level up in the DOM 
childNode //An array of references to the nodes one level down in the DOM 
attributes //An array of attributes of an HTML element 
style //An object encapsulating the CSS/HTML styling of an element  

//Common DOM Methods
getElementById(id) // Gets the elemenet with a given ID below this point in the DOM //'Id' in method is case sensitive 
getElementsByTagName(tag) // Gets all elements with the given tag below this point in the DOM
appendChild(node) //Add the given node to the DOM below this point
removeChild(node) //inverse of appendChild(node) 
```

Because the names of the objects can be quite long, the library, ‘jQuery’ is added. One thing it does is it simplifies DOM manipulations

[https://api.jquery.com](https://api.jquery.com)

```jsx
document.getElementById('colorDiv').style.backgroundColor = 'green' 
//Using the jQuery library it can also be written as
$('#colorDiv).css('background-color','green');
```

## LECTURE 9 :FLASK

### FLASK

Web frameworks make the process of typing code manually much easier. Popular frameworks include Django, Pyramid, Jinja and Flask. (Basically a library). HTML’s major fault is that it is static. By incorporating Python, you can make web pages more dynamic.

```python
#Displaying time example
from flask import Flask 
from datetime import datetime 
from pytz import timezone
#importing function Flask and module
app = Flask(_name_) 
#from here define application behaviours 
@app.route("/") 
def time():
	now = datetime.now(timezone('America/New_York'))
	return "The current date and time in Cambridge is {}".format(now) 
```

The way that Python is implemented into HTML is through the usage of decorators. A decorator is a function that takes in another function as a parameter and then returns a function. In Flask they are used to associate a particular function with a particular URL.

```python
#Running a Flask application within CS50 IDE 
export FLASK_APP=application.py 
	export FLASK_DEBUG=1
		flask run 
```

```python
#Passinng data via URLs is akin to using HTTP GET 
@app.route("/show/<number>")
def show(number):
	return "You passed in {}".format(number) 
```

```python
#Passing data via HTML forms as with HTTP POST (must indecate the acception of POST) 
@app.route("/login",methods=['GET','POST'])
def login()
	if not request.form.get("username") 
		return apology("must provide username")
```

```python
url_for()
redirect()
session()
render_template()
```

→ Flask Guide: [](https://flask.pocoo.org/docs/0.12/quickstart/)[https://flask.pocoo.org/docs/0.12/quickstart](https://flask.pocoo.org/docs/0.12/quickstart)

→ Jinja Guide: [https://jinja.pocoo.org](https://jinja.pocoo.org)

### AJAX

AJAX (formerly known as Asynchronous JavaScript and XML(JSON)) Allows us to dynamically update a webpage. For example the scores of a sports game are updated using AJAX

XMLHttpRequests allow a client to ask for an asynchronous request for more information. Syntax is as follows: var xhttp = new XMLHttpRequest();. After obtaining the new object, you need to define its onreadystatechange behavior. This is a function (typically an anon function) that will be called when the asynchronous HTTP request has completed, and thus typically defines what is expected to change on your site. They have two additional properties that are used to detect when the page is finished loading.

- The readyState property will change from state=0 (request not yet initialized) to 1,2,3 and 4(request finished, response ready); Returning 200 (OK)

Then ensure asynchronous request using open() method to define the request and the send() method to actually send it. → There is a slightly different way to do this in jQuery

```python
function ajax_request(argument)
{
	var aj = new XMLHttpRequest();
	aj.onreadystatechange = function() {
		if (aj.readyState == 4 && aj.status == 200) 
	#do something to the page here
	};
	aj.open("GET",/*url*/,true);
	aj.send();
}
```

This can be done in jQuery: [https://api.jquery.com/jquery.ajax/](https://api.jquery.com/jquery.ajax/)

vsco

css files

[](https://www.example.com/route)[https://www.example.com/](https://www.example.com/)route/?key=value

flask framework in python

[app.py](http://app.py)

requirements.txt

static/

templates/

decorator

Advantages to using flask

URLs

templates

input tag

form tag

key value pair

jinja

privacy + inspect

post

confirm form resubmission

MVC

select menu

cross site request forgery

OS.environ

band

sending emails through python

cookies

sessions

shopping carts

post

fetch

JSON

## LECTURE 10: CONCLUSION

Computational thinking

correctness, design, style

abstraction

precision

[https://docs.microsoft.com/en-us/windows/wsl/about](https://docs.microsoft.com/en-us/windows/wsl/about)

Learn GIT → Git hub

Get visual studio code

Host a website (portfolio)

![[iuhigu.png]]![[gtiuuiiuhiui.png]]