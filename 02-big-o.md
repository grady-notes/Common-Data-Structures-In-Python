# Big O Notation

Big O notation is a mathematical notation for describing the growth of a function. In simpler terms, Big O notation is a way to describe the growth of a function as the number of operations it takes to compute a value.

For an array, the time taken to run any operation on the array is linearly proportional to the size of the array.

Any linear function can be expressed as a polynomial function of the form:

```
time = a * size(array) + b
```

# Time complexity.

The mathematical representation of the time required for the program to complete a task is called the Big O notation.

```python
def foo() :
    def sqaured (arr) :
        squared_n = []
        for i in arr :
            squared_n.append(i ** 2)
        return squared_n
    arr = [1,2,3,4,5]
    print(sqaured(arr))
if __name__ == "__main__" :
    foo()
```

An example of a program whose time complexity is constant is shown below: O(1) is the Big O notation for this function.

```python
def foo() :
    def find_first_pe(prices, eps, index) :
        pe = prices[index] / eps[index]
        return pe
    print(
        find_first_pe(
            [1,2,3,4,5],
            [0.1,0.2,0.3,0.4,0.5],
        3))
if __name__ == "__main__" :
    foo()
```

An example whose time complexity is square is shown below: O(n^2) is the Big O notation for this function.

```python
def foo() :
    arr = [3,6,2,4,3,6,8,9]
    duplicate = None
    for i in range(len(arr)) :
        for j in range(i+1, len(arr)) :
            if arr[i] == arr[j] :
                duplicate = arr[i]
                break
        for i in range(len(arr)) :
            if arr[i] == duplicate :
                print(arr[i])
if __name__ == "__main__" :
    foo()
```

There are some rules to follow when writing Big O notation:

Considering

```
time = a * size(array) + b
```

- The Big O notation should be a single letter.
- Consider only the fastest growing function. Hence `time = a * size(array)`
- Drop all the constants. Hence, `time = size(array)`

An example of a program whose time complexity is proportional to the size of the array is the n(th) function. O(n) is the Big O notation for this function.

The reason we apply these rules is because we want to write a program that is efficient. Big O notation applies to worst cases of a program where the value of the function grows in very large numbers. Due to this other values become irrelevant.

# Space complexity.

Previously we saw the time complexity of the n(th) function. Now we shall see the space complexity of the n(th) function.

Let us take an example of a simple binary search operation and understand the space complexity of the n(th) function.

We know that for a complete binary search operation, it would take n/2<sup>k</sup> iterations.

Hence,

<pre style='font-family: sans-serif; letter-spacing: 1px'>
1 = n/2<sup>k</sup>
</pre>

Applying logx to the above equation, we get:

<pre style='font-family:sans-serif; letter-spacing: 1px'>
log<sub>2</sub>(n) = log<sub>2</sub>2<sup>k</sup>
log<sub>2</sub>(n) = (k)log<sub>2</sub>2
log<sub>2</sub>(n) = k
</pre>

Hence we get,

<pre style='font-family:sans-serif; letter-spacing: 1px'>
k = log<sub>2</sub>n
</pre>

Therefore we get log<sub>2</sub>n iterations for a complete binary search operation.

Therefore the space complexity of the n(th) function is :<pre style='font-family:sans-serif; letter-spacing: 1px'>O(log<sub>2</sub>n)</pre>
