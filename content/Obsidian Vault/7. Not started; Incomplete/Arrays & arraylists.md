An array can be thought of as a flight of stairs where each "step" is another index. In memory, each value is stored contiguously such that there are consistent steps that connect each element. In other words it is a list with similar values. It can be used to store anything from usernames to passwords to high scores and prices. However, in most programming languages they must be of the same type. (Integer, string, float …)

When defining an array you can populate it at declaration or simply set the size and do so later. Syntax depends on the language

Every item within a list is referred to as an element, where the collective of the elements are what make up the array. Where an array always has a name (reference and interaction), a type and a size (often fixed).

Parallel arrays contain the same number of elements and have an index value that corresponds with the other arrays information. E.g. `name[2] = phone_number[2]`. The information in different arrays are meant to talk about the same entity. (these have few use cases)

![[Getting-Started-with-Array-Data-Structure.webp]]

An array is 0 indexed, meaning the first element in an array has an index of 0
You can use a variable to reference a specific element in an array `array[i] = 3`

![[Memory-Representation-of-Array-(1)-1024.webp]]

Two-dimensional arrays are useful for creating a grid, where two indexes are required, `array[column][row]`.

- Accessing elements = O(1) 
	Through usage of indexes, and definite size. In memory, size is allocated for the array, and its stored near each other; allowing for operations to be preformed, the computer can add the index of the accessed value to access the data at a constant rate
	
* Searching for an element = O(n) 
	Arrays are often not sorted and thus linear search has to be preformed, worst case scenario
* Insertion and deletion of an element O(n)
	Shifting every element to the right once and placing the new value at index = 0 Setting array[i] = `array[i+1]` will also take O(n) amount of steps

In C, arrays have a fixed size = the size cannot be altered. For alterable "arrays" see [[Vectors (DS)]] 

Pros
- Good for storing similar contiguous data
- Used for smaller tasks
- O(1) Accessing

Cons
- Size of array is fixed
- Insertion and deletion are not efficient
- Can waste storage if elements in an array are null