2024-07-3119:08
Status: 
Tags: 
## Structure
Command line interface (CLI)→ Linux +vs. GUI
(IDEs = Text editors → Use Visual Studio Code )
(Source code → Compiler → Machine code)
A terminal window allows you to run commands on code you create ($)

Header files = a menu of functions for example # include <stdio.h> and  <#include cs50.h> = are extensions to C
## Data Types
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

## Source
```c
printf("hello world") = // Side affect = visual output
Return values = // Output of the function or program
string answer  = // get_string("What's your name? ");
string/int = //specifies what variable is, answer = variable, get_string()= function, "x" = displayed text
(=) = //assignment operator
$\n$ = //writes a new line
printf("hello, %s\n", answer);
= // %s put a string placeholder
= // %i put a integer placeholder

// To start a program use
int main(void)
{
... put all main code in here
}
```
## If Else Conditionals 
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

## Loops 
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
``````
## Arrows 
`(pointer_name)->(variable_name)`

`foo->bar` is equivalent to `(*foo).bar`, i.e. it gets the member called `bar`from the struct that `foo`points to. The operator ‘.’ is used to access the child object of…

# Source(s)