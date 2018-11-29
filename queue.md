# Queue

A queue is a linear data structure but it is not a contiguous block of memory. It can be thought of as an ordered collection of items. It is a FIFO data structure meaning its nature is first in first out. This can be thought of as "first come first served."

# In Memory

In memory, a queue looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

A queue supports the following operations:

* **dequeue**: Dequeueing the first item from the queue. This operation has a complexity of O(1) because all we have to do to delete a node is make the node before the deletee point to the node after the deletee as it's next. There is no iteration involved. If we have to search for the item we wish to delete, then this is actually executed in O(n) because searching is O(n). The actual deletion itself is O(1).
* **insert**: Inserting a node into the linked list. The complexity is O(1) as well because we just have to swap the next pointers around accordingly. For example, we just make the insertee's next point to the node we want to come after it. We then make the node before the insertee's next point to the insertee. As with deletion, this would only be an O(1) complexity if we had a handle on where things were. If we don't have a handle where items are we have to search for the space we want to insert and as mentioned above, searching is an O(n) operation.

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