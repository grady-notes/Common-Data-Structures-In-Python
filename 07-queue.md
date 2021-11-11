# Queue

Queue is a data structure that stores a collection of items in a linear order, allowing only access to the **front** of the collection. It is a first in first out (FIFO) data structure. The first element to be added to the queue is the first one to be removed.

# Complexity

The complexity of the operations is O(1) as the operations are performed in constant time.

# Implementation

In a queue, we always insert data at the 0 index and remove data from the end of the queue.

```python
def foo() :
    arr = [1,2,3,4]
    stack = []
    print(f"Before : {stack}")
    for data in arr :
        stack.insert(0, data)
    print(f"After : {stack}")
    print(f"Popped : {stack.pop()}")
    print(f"After : {stack}")

if __name__ == '__main__' :
    foo()
```

More efficient implementation of the queue using a deque.

```python
from collections import deque

def foo() :
    arr = [1,2,3,4]
    stack = deque()
    print(f"Before : {stack}")
    for data in arr :
        stack.insert(0, data)
    print(f"After : {stack}")
    print(f"Popped : {stack.pop()}")
    print(f"After : {stack}")

if __name__ == '__main__' :
    foo()
```
