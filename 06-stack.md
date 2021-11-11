# Stack

Stack is a last in first out LIFO data structure that can be implemented using the list data type. Stack is a linear data structure in which the alst element added is the first element to be removed.

Inserting an element in the stack is known as pushing which can be done using the `append()` method and removing an element is known as popping which can be done using the `pop()` method.

# Complexity

The time complexity of the stack operations is `O(1)` as they are constant time operations.

The complxity of searching an element in the stack is `O(n)` as it is linear time operation.

# Use Cases for Stack

- Function calling in any programming language is managed using the stack data structure.
- The stack is used to manage the function call in the recursive function.
- The undo functionality in text editors is implemented using the stack data structure.

# Implementation

```python
def foo() :
    arr = [1,2,3,4]
    stack = []
    print(f"Before : {stack}")
    for data in arr :
        stack.append(data)
    print(f"After : {stack}")
    print(f"Popped : {stack.pop()}")
    print(f"After : {stack}")

if __name__ == '__main__' :
    foo()
```

More efficient way to implement the stack is using the the deque from the collections module. This is a double ended queue which can be used to implement the stack. Deque uses the linked list data structure.

```python
from collections import deque

def foo() :
    arr = [1,2,3,4]
    stack = deque()
    print(f"Before : {stack}")
    for data in arr :
        stack.append(data)
    print(f"After : {stack}")
    print(f"Popped : {stack.pop()}")
    print(f"After : {stack}")

if __name__ == '__main__' :
    foo()
```
