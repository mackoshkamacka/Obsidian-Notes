2024-11-0113:29
Status: #CPSC110 
Tags: 

Abstraction is a crucial technique for managing complexity in programs. One aspect of this is that it can make programs smaller if the abstract functions are used by many other functions in the system. Another aspect is that it helps separate knowledge domains more clearly in code. All the work you've done understanding templates is about to give you a nice surprise.

Instead of writing several functions that all do generally the same thing, abstraction can be used to generalize them. Similar to putting operations as a parameter into functions. Take listing all elements of an array, adding all node indexes, appending letters of a string. The general recursive structure is the same, but only the operation and data type changes. 

