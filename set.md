# Set

A set is an unordered collection of data objects similar to dictionaries but with only keys. Sets do not allow duplicates. Because of these behaviors a set guarentees everything is unique.

# In Memory

In memory, a set looks like this:

![Image of Array in Memory](images/array_memory.png)

\[description of diagram\]

# Operations

A set supports the following operations:

* **containsKey**: ContainsKey checks to see if a key is in a set. The complexity is O(1).
* **add**: This operation will add an element into the set. Its complexity is O(1) because like a dictionary it is also implemented using a hash table which allows for constant time operations.
* **remove**: Remove will remove a key from the set. The complexity is also O(1).

A set is useful when we have a lot of data that has no real order. An example of a set would be ingridients for a recipe. Often a recipe will call for butter twice, or 2 egg yolks and seperatly call for 2 egg whites. This might be because we need to use butter in the pie, and the other butter is meant for the pie crust. When we go to the store to shop for the ingridients we don't look at the list and buy 2 tablespoons of butter, then other ingridients, then go grab another 3 tablespoons of butter when we read it again. We just care that we need the butter once. So we could put all the ingridients into a set and this would efficiently help us shop.

# Example

```
mySet = {12, TRUE, 'cat', 77, 0} #Creates a set with values 12, TRUE 'cat', 77, 0

'dog' in mySet #returns false because 'dog' is not a key in mySet
mySet.add('dog') #adds 'dog' to mySet
mySet.remove('cat') #removes 'cat' from mySet
```

(c) 2018 Chevelle Boyer. All rights reserved.