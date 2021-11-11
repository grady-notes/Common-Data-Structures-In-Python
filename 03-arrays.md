# Arrays

Arrays are the most common data structure in any programming. They are used to store multiple values in a single variable. They store similar data types in consecutive memory locations. Arrays can be iterated over and their elements can be accessed by their index.

## Representation of array in general format.

```
arr = [100,200,300]
```

<style>
tr, th {
    border: 1px solid #ccc;
}
</style>
<table>
  <tr>
    <th>Memory Location</th>
    <th>Element</th>
  </tr>
  <tr>
    <th>0x00500</th>
    <th>100</th>
  </tr>
  <tr>
    <th>0x00504</th>
    <th>200</th>
  </tr>
  <tr>
    <th>0x00508</th>
    <th>300</th>
  </tr>
<table>

Notice that we are skipping 4 bytes between each element. This is because we are storing integers and the size of the integer data type is 4 bytes.

## Iteration of an array by index

```
arr[0] = 100
arr[1] = 200
arr[3] = 200
```

If you want to access an element from the array, you can use the index.

For example,

```
arr = [100,200,300]
print(arr[2])
```

This will print 300.

# Complexity of an Array

Complexity of looking up an element in an array is O(1). This will always be the same since, the array is stored in consecutive memory locations and it is a constant time operation.

Complexity of looking up an element by its value will always be in in the order of O(n). This will be the case if the array is sorted.

Complexity of iterating over an array and traversing through it is O(n)

Complexity of inserting an element in an array at any given specific index will be O(n). This complexity remains the same for deleting an element as well.

# Types of Arrays

Arrays are generally of two types, one is fixed size and the other is of varying size.

The fixed size array is called as the static array and is always initialized with a fixed size value and does not allow tranversion or insertion/deletion of elements beyond the fixed size.

The varying size array is called as the dynamic arrays and can grow as much as the input of the array grows. They do not have a fixed size or limit. This is the case of the Python list which can be operated as long as the elements exist.
