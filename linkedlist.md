# Linked List

A linked list is a linear data structure but it is NOT a contiguous block of memory. We must always know where the first, or head, node is, as well as teaching the last node that it is the last by telling it there is no next. We are still able to navigate a linked list even though it is not sequential by only knowing each node's next. There is also a doubly linked list where each node points to the one after it and before it.

# In Memory

In memory, a linked list looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

A linked list supports the following operations:

* **search**: Searching for an element in the linked list. The complexity of this operation is O(n). In order to see if an item is in the list, we have to check every node. This is becasue the only information each node has is it's next node. Therefore we must traverse through the entire list until we find the element we are looking for (or don't) making it O(n).
* **delete**: Deleting a node from the linked list. This operation has a complexity of O(1) because all we have to do to delete a node is make the node before the deletee point to the node after the deletee as it's next. There is no iteration involved.
* **insert**: Inserting a node into the linked list. The complexity is O(1) as well because we just have to swap the next pointers around accordingly. For example, we just make the insertee's next point to the node we want to come after it. We then make the node before the insertee's next point to the insertee.

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