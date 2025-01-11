2025-01-1015:40
Status: #CPSC210
Tags: [[Java]] [[Object Oriented Programming]] 
###  Basics 3 

#### Classes 
- A class holds operations and data related to one concept:
- Take a dog for instance. Data = age, breed, DNA etc. operations = bark, wag tail etc. 
- Classes are a static structure that allows for description of a concept in one place. This allows for creating instances based on the "template" a class provides. 
- Constructors are how new instances (objects, reference variables) are defined - they come with a template: 
	- `new Dog(...)`
- Constructors usually come right after the declaration of constants and field, and have the same name as the class they're located in. 

#### Anatomy of a Class 
- A **class** contains: **imports**, a **declaration** (its name), and body (its **definition**).
- A **class definition** contains **constant declarations**, **field declarations**, and **method declarations** (including constructors).
- A **class name** summarizes its contents to make it clear what concept it is encapsulating. Everything inside the class is centrally related to that class, and ties back to that name. 
- All names must reflect their purpose.  
- Fields can be declared to be of types defined in the project (Types are Classes and more, as we will see).
- **Constructors** are named exactly the same thing as the class, and there can be more than one of them, as long as they have different parameter lists.
- The keyword **Static** means that a field or method stays within the class and doesn't get instantiated with the object.

#### Variables
- Java has two kinds of types that can be used to declare variables: primitives (int, boolean, ...) and objects
- when primitive values are declared, they get a spot in memory that holds their value. 
- when objects are declared and instantiated, they get a spot in memory that holds a reference to an instance of their type.
- `a = b` assigns whatever value is in **b**, into **a**'s memory slot. If that value is of a primitive type, it copies the value right in. If **b**'s value is an object reference, that object reference is copied, which means that **a** and **b** would refer to the same object.
- ArrayLists hold a sequence of object references to whichever type the ArrayList is declared to hold.  `ArrayList<Dog>` holds a series of references to Dog instances. (Note that adding the same object to the array multiple times puts the same object reference in multiple spots in the array, all pointing to the same instance!)
- An object is active if it has been instantiated. If we are counting active objects, we count how many objects have been instantiated.
- A variable is active if it is referring to an active object. There can be multiple variables referring to the same object. 
- A primitive value is active if it has been declared at all.

#### Styling convention for classes in CPSC 210
![[Pasted image 20250109183958.png]]

#### Debugging 
- **Hypothesis driven debugging**: making careful educated guesses, with plans for how to validate or invalidate them.
- **Breakpoints** let you stop execution of your code at a specific point. Set a breakpoint by clicking on the left next to the line of code (in the grey area).  Then **step over** or **step into** methods, watching the values of variables in scope as you go.
- Choose the "**debug**" icon instead of the "run" icon to execute your code in debugging mode.
- If it looks like a value isn't being set there are a few common possibilities: step through to ensure it's being displayed or returned correctly, and step through to where the value should be set, and make sure it's being set properly.
- If you are getting output you weren't expecting, try placing a breakpoint at the code responsible for the output -- then you will be able to check the state of all the variables to see the context of that code -- maybe some of the variables aren't being set properly!
#### Primitive Types
![[Pasted image 20250110100820.png]]


Addresses have 4 bytes 
An initiated object (in a variable p), only contains the address to the object in memory 

```java 
Tank myTank; // Constructor to create an object
myTank = new Tank(100); // Assaigning address to myTank
myTank.faceLeft(); // Method on myTank to change the direction 
myTank.move(); // Method on myTank to move the x position by one step.

```

static = all objects share the same field.