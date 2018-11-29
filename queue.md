# Queue

A queue is a linear data structure but it is not a contiguous block of memory. It can be thought of as an ordered collection of items. It is a FIFO data structure meaning its nature is first in first out. This can be thought of as "first come first served."

# In Memory

In memory, a queue looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

A queue supports the following operations:

* **dequeue**: Dequeueing the first item from the queue. This operation has a complexity of O(1) because in the implementation we maintain a pointer to the first variable in the array or linked list (however we choose to implement it) to allow for constant time.
* **enqueue**: Enqueueing an item to the end of the queue. The complexity of this operation is O(1) because we only ever enqueue to the end of the list. If we implement the queue using an array this operation is O(1) because inserting in arrays in O(1). If we implement the queue as a linked list the complexity to enqueue would still be O(1) because we would maintain a pointer to the end of the list.
# Use Cases

A linked list is useful when we need to do a lot of insertions or deletions because they are constant time operations.

A linked list is not as useful when we need to do a lot of searching or checking to see if an element is in the linked list.

# Example

```
myLinkedList = Linkedlist() #instantiates a Linked List

myLinkedList.insert(prev_node, 12) #inserts a node with value 12 after the "prev_node"
myLinkedList.deleteNode(deletee) #deletes deletee node
myLinkedList.search(22) #checks to see if node with value 22 exsists
```

(c) 2018 Chevelle Boyer. All rights reserved.