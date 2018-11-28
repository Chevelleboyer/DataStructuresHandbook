# Array

An array is \[a linear data structure that takes up a contiguos block of memory.\].

# In Memory

In memory, an array looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

An array supports the following operations:

* **index/retrieval/access**: Obtain a value stored in the structure at a specific indexed position in the array.
  * O(1), constant time. An array variable points to the first memory address (base address) in an array. We also know the data type of the elements in the array, and therefore the size of each element. Given the index of an element we wish to read, we can calculate the address of that element in just one calculation: base address + sizeof(datatype) * index. Since we can calculate this in one step for all values in the array, this is an O(1) constant time operation.
* **delete**: This operation will delete an element in the array. The complexitiy of this operation is O(n) because after deleting an item you must shift all the other elements over to fill the empty space.
* **insert**: Inserting a value into the middle of an array. The complexity of this operation is O(n) n being the size of the array. This is because in order to insert a value into an array you must shift every element after the insertee over.
# Use Cases

An array is useful \[when\] \[why\].

It is not as good as \[what] \[why].

# Example

```
sample code showing creation, and exercising all of the operations
or
a program that doesn't use the structure, and then a version that does
```

(c) 2018 YOUR NAME. All rights reserved.
