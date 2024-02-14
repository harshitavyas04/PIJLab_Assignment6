# PIJLab_Assignment6
In this code, we have two different implementations of a stack data structure: Fixed_STK and Growable_STK. Both implementations follow the Interface_STK interface, which defines the methods that a stack should have: push, pop, displayStack, isOverflow, and isUnderflow.

The Fixed_STK implementation uses a fixed-size array to store the elements of the stack. It has the following methods:

push: This method takes an integer as an argument and adds it to the top of the stack. If the stack is full (i.e., the top index is equal to the last index of the array), it throws an error message and terminates the program.
pop: This method removes the element at the top of the stack and returns it. If the stack is empty (i.e., the top index is -1), it throws an error message and terminates the program.
displayStack: This method prints the elements of the stack. If the stack is empty, it prints a message and terminates the program.
isOverflow: This method checks if the stack is full. It returns true if the top index is equal to the last index of the array, and false otherwise.
isUnderflow: This method checks if the stack is empty. It returns true if the top index is -1, and false otherwise.
The Growable_STK implementation uses an ArrayList to store the elements of the stack. It has the same methods as the Fixed_STK implementation, with the following differences:

push: This method takes an integer as an argument and adds it to the top of the stack. If the stack is full (i.e., the ArrayList is at its maximum capacity), it automatically increases its capacity.
pop: This method removes the element at the top of the stack and returns it. If the stack is empty, it throws an error message and terminates the program.
displayStack: This method prints the elements of the stack. If the stack is empty, it prints a message and terminates the program.
isOverflow: This method always returns false, because an ArrayList can grow indefinitely.
isUnderflow: This method checks if the stack is empty. It returns true if the ArrayList is empty, and false otherwise.
In the main method of the StackDemo class, we create instances of both implementations and use them to demonstrate their functionality. We push some elements onto the stacks, display the elements, pop an element, and then display the remaining elements.
