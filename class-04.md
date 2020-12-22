# Classes, Objects and understanding recursion(recursion())

Objects are containers for variables and functions, not unlike a toolbox or chest of drawers. Recursion is the process of chipping away at a problem until a solution is reached often by repeating a single step until a pre-determined condition is satisfied.

## Classes and objects
Classes give objects their shared variables and functions. If we use a toolbox example, different drawers hold different types of tools. A crude anology might be; if the drawer is the class and the tools are the objects and they are seperated by what they are used for than the leather tools drawer is the class and the tools inside are the objects all sharing certain characteristics that make them ideal for working with leather.

each instance of an object from a class will have all the same variables and functions but the values assigned to them can be different for each instance of the class. variables of an object can be accessed using dot `.` notation. like so: `my_object.object_variable_name`

Functions of a Class can be accessed by their objects using the similar notation but making sure to add the parens `()` at the end and passing in any of the required arguments. `my_object.object_function(arguments)`

all functions declared within a class must contain "self" as a parameter. very similiar to the implied "this" of javascript constructor functions. 

### Recursive thinking

- set base case, this is the condition that breaks the loop allows the functions to clear from the stack
- because each call of the function is dependent on information from the first call you must remember to preserve the state of the current calculation and pass it through to the next call of the function. 
- 



[Return to Main index of Notes](./README.md)