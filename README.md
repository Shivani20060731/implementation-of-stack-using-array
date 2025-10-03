# implementation-of-stack-using-array
Implementation of Stack using Array in C++

Aim

To study and implement a Stack data structure in C++ using arrays, demonstrating its fundamental operations: Push, Pop, Peek, and Display.


Software Required

Online C++ Compiler


Theory

Concept of Stack

A stack is a linear data structure that works on the LIFO (Last In, First Out) principle. This means that the element inserted last will be removed first.

Examples from daily life:

A stack of plates, where the plate placed last is picked first.

Undo/Redo operations in text editors.

Function call management in compilers.


Stack Operations

1. Push (Insertion): Adds a new element at the top of the stack.

If the stack is full, it causes Stack Overflow.



2. Pop (Deletion): Removes and returns the topmost element of the stack.

If the stack is empty, it causes Stack Underflow.



3. Peek (Top): Returns the top element without removing it.


4. Display: Prints all elements of the stack from bottom to top.



Implementation Using Array

The stack is implemented using a static array of size MAX_SIZE = 5.

A variable topIndex keeps track of the current top of the stack.

Initially, topIndex = -1 indicates an empty stack.

Each successful push increments topIndex, while each pop decrements it.



Advantages of Array-based Stack

Simple and easy to implement.

Fast access using index values.


Limitations

Fixed Size: Cannot grow beyond the defined array size.

Wasted Space: If stack is underutilized, memory is wasted.


For real-world applications, dynamic stacks using linked lists are often preferred.


Algorithm

Stepwise Algorithm for Stack using Array

1. Start


2. Initialize topIndex = -1 and declare stackArray[MAX_SIZE].


3. Push(x):

If topIndex == MAX_SIZE - 1 → print "STACK OVERFLOW".

Else, increment topIndex and set stackArray[topIndex] = x.



4. Pop():

If topIndex == -1 → print "STACK UNDERFLOW".

Else, return stackArray[topIndex] and decrement topIndex.



5. Peek():

If topIndex == -1 → print "STACK UNDERFLOW".

Else, return stackArray[topIndex].



6. Display():

If topIndex == -1 → print "STACK is empty".

Else, print elements from stackArray[0] to stackArray[topIndex].



7. In main():

Perform push operations to insert elements.

Perform a pop to delete the top element.

Use peek to view the current top element.

Use display to print the remaining stack contents.

8. Stop


Conclusion

The array-based stack implementation successfully demonstrates the fundamental operations of the LIFO (Last In, First Out) data structure.

Key Learnings:

Push, Pop, Peek, and Display operations were implemented using array indexing.

Overflow and underflow conditions were properly handled to prevent runtime errors.
