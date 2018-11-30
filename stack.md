# Stack

A stack is a linear, and a LIFO (last in first out), data structure.

# In Memory

In memory, a stack looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

A stack supports the following operations:

* **push**: Pushes an element onto the top of the stack. This operation is O(1) because we maintain a stack pointer that keeps track of where the top of the stack is at all times.
* **pop**: This operation will pop (which is like a deletion) the top item off of the stack. It is important to note that popping does not return the value of the element popped.
* **peek**: Peek allows us to view the value of the top item on the stack. It is an O(1) operation because of the stack pointer which always points to the top item.

# Use Cases

A stack is useful when we want something in reverse order due to the nature of LIFO. For example when the use of backtracking is required.

A stack is not as useful when we need to access/insert/delte items in the middle of our data, or when we need to alter data already stored.

# Example

```
pancake = Stack() #instantiates an empty stack

pancake.push(blueberry) #pushes a blueberry pancake object onto the top of the stack
pancake.push(bananaCream) #pushes a bananaCream pancake object onto top of stack
pancake.push(chocolateChip) #pushes a chocolateChip pancake object onto top of stack
pancake.pop() #removes chocolateChip pancake object from top of stack
```

(c) 2018 Chevelle Boyer. All rights reserved.
