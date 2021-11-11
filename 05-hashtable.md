# Hashtable

Hashtable is an underlying data structure that stores data in key-value pairs. It is similar to a dictionary, but it is not a dictionary. The keys are unique and unordered. The values can be any type of data. The dictionary uses the hash function to determine where the data is stored.

Hash functions are used to convert a string into a number. The hash function is used to determine where the data is stored.

# Complexity

The Big O notation for the hash function is O(1). This is because the hash function is a constant time operation.

# Implementation of Hashtable

```python
def foo() :
    # Hashtable Class
    class Hashtable :
        def __init__ (self, max) :
            self.max = max
            self.arr = [None for i in range(max)]
        def get_hash(self, key) :
            hash = 0
            for char in key :
                hash += ord(char)
            return hash % self.max
        # Adding an item to the Hashtable
        def add(self, key, value) :
            hash = self.get_hash(key)
            self.arr[hash] = value
    # 30 is the maximum style of the hastable
    h = Hashtable(30)
    arr = ['january 1', 'february 2', 'march 3', 'april 4']
    for item in arr :
        print(f"Index of {item} in Hashtable : {h.get_hash(item)}")
    h.add('may 5', 20)
    print(f"Index of may 5 in Hashtable : {h.get_hash('may 5')}")

if __name__ == '__main__' :
    foo()
```

[Previous : Linked List](./04-linked-list.md) | [Next : Stack](./06-stack.md)
