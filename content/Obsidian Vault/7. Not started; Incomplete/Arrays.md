2024-07-3119:19
Status: #CS50 #NES #Incomplete 
## Overview 

## Compiling
$ clang = directly compiles code, allows for code to act in specific ways when converted to machine code (E.x `$clang-o hello hello.c, -o = output)`

`a.out` = assembly output

Compiling
- Preprocessing (#telling the compiler to find/trust that the prototypes used are real and should not output an error) Copying and pasting the #…’s actual code in place of #… so that the program can actually run.
- Compiling = converting code into assembly language (basic instructions)
- Assembly = converting assembly language to binary
- Linking = stiches all libraries and code together e.g. (The binary of your code, library A, library B are all now linked together)

### Debugging
By using printf(), you can see the values assigned to strings and take a closer look into what might be causing an issue

There are also debugger commands that tell you what’s happening within your code one step at a time. (they modify only compiled code). To note it can tell you the value of a variable.

Step over = stepping over a line, step into = stepping into a function

Int manipulated by int will output an int. An int manipulated by a float will output a float

Arrays store multiple variables of the same kind of variable in different locations denoted by their location in “$[]$” E.x. bool battleship$[10][10]$ (Having two indexes allows for grid like storage) Arrays ARE passed by reference i.e. they are global regardless of if they’re in a function or not.

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

 think now it would be clear. Good Luck.

Exit status reasons to quit code through CLI, (having main return a non-zero value e.g. 1) e.g. ERROR 404

Functions (procedures, methods, subroutines) are black boxes with a set of 0+ inputs and 1 output

e.g. a=3, b=6, c=7, add(a, b, c) → 16

Functions allow programmers to write less code and to organize/simplify their code. It also allows for smoother debugging and reusability

Function declarations are established so that the computer knows what the program is saying. (Establishing a ‘shortcut’)

They are all structed like this:

Return-type`[the kind of output] name[meaningful name of function](argument-list)[comma separated inputs to your function, each of which have a time and name]`; Then using {}, add what the function does

```c
E.x. int add_two_ints(int a, int b); 
{
int sum = a + b
return sum;
}
```

Functions can have void input or output in which they output or take in no arguments

## Variable scope
If a variable is within a function is is a local variable and cannot be referenced in future lines of code, where global variables can.

When referencing a global variable, you are making ‘copies’ of when used in functions. To manipulate the variable you must be overwritten to be changed

argc = count the amount of strings, argv = store an array of string values
# Source(s)