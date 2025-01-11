###### 2025-01-1016:25
###### Status: #Incomplete 
###### Tags: [[Computer Science]] [[Object Oriented Programming]]
###### Source(s): 
https://www.youtube.com/watch?v=xk4_1vDrzzo
## Overview/setup 
Java is a high level language and is the 3rd most popular programming language. Source code (what is written be developers) is complied to byte code (an intermediate, cross-platform, portable version of the code) that can then be translated by a JVM to run on a local machine. This is done to cater to the operating system - compilation on a Mac system will differ from Windows. 

![[Pasted image 20250110150755.png]]

A JVM is a "translator" of byte code to machine code. It is included in a JDK (Java Developer's Kit). A JDK also contains a JRE (Java Runtime Environment) which is a collection of libraries and toolkits. The JVM (Java Virtual Machine) is in the JRE and it is used to run programs.   

![[Pasted image 20250110151318.png]]
*The Oracle SE JDK is the most common JDK*

An IDE is also needed (Integrated Developer Environment) → Eclipse and IntelliJ are the most popular. 

To create a Java Explorer in Eclipse follow: https://www.youtube.com/watch?v=xk4_1vDrzzo 7:00
## Fundamental Methods
### Main 
Every program will contain some sort of `main` method to run. It should look like this: 
```java 
public class Main {
	public static void main(String[] args) {
		// code goes here
	}
}
```

### Print 
To print text to the terminal, use the method, `System.out.print();`. 
```java 
public class Main {
	public static void main(String[] args) {
		System.out.print("I love pizza");
	}
}
```
> *Terminal output:* 
> `I love pizza`

The cursor does not move down the next line, so if the following runs,
```java 
public class Main {
	public static void main(String[] args) {
		System.out.print("I love pizza.");
		System.out.print("It's really good!"); 
	}
}
```
> *Terminal output:* 
> `I love pizza.It's really good!`

To make a new line after a print statement, use `.println` (print line) instead of `.print`
```java 
public class Main {
	public static void main(String[] args) {
		System.out.println("I love pizza.");
		System.out.println("It's really good!"); 
	}
}
```
> *Terminal output:* 
> `I love pizza.`
> `It's really good! 

An escape sequence character, "\" is used to perform special operations within print statements. So another way to make another new line in a print statement is to use `\n` where the new line is intended to be. 

```java 
public class Main {
	public static void main(String[] args) {
		System.out.println("I love pizza.\n It's really good!"); 
	}
}
```
> *Terminal output:*
> `I love pizza.`
> `It's really good! 

Some other escape sequences are: `\t` adds a tab, `\"` adds a double quote, `\\` adds `\` 
##### Concatenating Expressions 
To add expressions together (often a variable and a string literal), use `+` to combine the expression: 
```java
public class Main {
	public static void main(String[] args){
	
		int x = 123; //initialization 
		System.out.println("My number is:" + x); 
	}
}
```
> *Terminal Output*
> `My number is: 123` 

#### Tips and Tricks: 
- For Eclipse, `System.out.println();` = `sysout + Ctrl + Space`
- For IntelliJ, `System.out.println();` = `sysout + Tab`
- Find-replace command is very useful for changing the behavior of code. 
-  In most cases whitespace (spaces, tabs, new lines) in source code (not print statements, nor keywords), do not affect the program's behavior: `System.out.print();`= `System.out.          print();`. 

### Comments
To comment code, write two forward slashes, `//` preceding the line of code that is to be commented out. To comment out multiple lines, use `/*` and `*/` to wrap a comment over multiple lines. *Eclipse will automatically add `*` at the beginning of the commented line not at the ends of the comment. However, the `*` is not necessary.* 

```java 
public class Main {
	public static void main(String[] args) {
		// System.out.println("I love pizza.\n It's really good!");
		
		/*  System.out.println("I love pizza.");
		*	System.out.println("It's really good!");  
		*/
		
		/*  System.out.println("I love pizza.");
		 	System.out.println("It's really good!");  
		*/
	}
}
```
> *Terminal output:*
> ` ` 
## Variables 
### Definition 
#### Primitive Data Types
There are 8 primitive (built into Java): 

![[Pasted image 20250110162145.png]]
*The convention for float values is to end the value with 'f'
The convention for char values is to wrap the value with single quotation marks 
The convention for String values is to wrap the value with double quotation marks
The convention for Long values is to end the value with 'L'*
#### Primitive vs. Reference Data Types
![[Pasted image 20250110163152.png]]
#### Declaration of Variables
- To declare a variable, state the type e.g. `int` and the variable name, say `x`. 
	- `int x;`
- To assign a variable to a value, ensure the value is of a valid type and 'equate' them with and equal sign. This requires the variable to first be declared (defined). 
	- `x = 123;`
- To initialize a variable combine the declaration and assignment of the variable into one step. 
	- `int x = 123;` 
### User input 


### Manipulation 
#### Swapping Variables 
Think of variables as cups of different liquids. In order to swap the fluid, you need to transfer one of the liquids to a temporary cup, then transfer.
- `x` $\to$  `temp`, then  `y` $\to$ `x`, then `temp`$\to$ `y`. 

```java
public class Main {
	public static void main(String[] args){

		String x = "water"; 
		String y = "Kool-Aid"; 
		String temp; 

		temp = x; 
		x = y; 
		y = temp; 
	}
}
```