# Tuple

A tuple is a linear data structure similar to an array. One of the differences between them is that a tuple is immutable and therefore can't be changed. The elements in a tuple are just references to strings which is why they cannot be changed/modified. You can, however, modify the object it points to.

# In Memory

In memory, a tuple looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

A tuple supports the following operations:

* **access/search**: Accessing or searching for an element in the tuple has a complexity of O(1). This is because just like with an array the tuple variable points to the memory base address. From there we can do one calculation, base address + index, to access any element. This is the only operation supported by a tuple because it is immutable. Since it cannot be changed we cannot insert or delete elements.

A deque is useful in  many situations. An example would be a DutchBros. coffee stand with two drive up windows. Generally, cars will line up at one window. If this line gets too long, however, cars can enter (enqueue) from the other window going the opposite direction. If both sides have long lines and one side starts to get shorter, the last car in one line can move to the end of the shorter line. Cars can not move from one line to the other if they are in the middle (without causing a huge traffic jam).

A deque is not as useful when we want our data processed in the order it was recieved with no exceptions. This would require a queue.

# Example

```
myDeque = Deque() #instantiates an empty deque

myDeque.enqueueFront(7) #enqueues 7 to the front of the deque
myDeque.enqueueRear(13) #enqueues 13 to the rear of the deque
myDeque.enqueueFront(22) #enqueues 22 to the front of the deque
myDeque.dequeueFront() #dequeues 22 from the deque
myDeque.dequeueRear() #dequeues 13 from the deque
```

(c) 2018 Chevelle Boyer. All rights reserved.