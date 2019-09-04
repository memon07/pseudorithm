## Binary Search

Binary search are basically used whenever the list starts to become large.<br/>
The binary search starts by testing the data in the element at the middle of the array.<br/>
this determines if the target is in the fist half or the second half of the list.we repeat the process <br/>
until we find the target or we come to conclusion that the target is not in the list.

middle :
```
(fist element index + last element index ) / 2
```

```javascript
list - array
last - index of last element
target - data to be stored
locn - address of index in calling the algorithm

1. first = 1
2. last = end
3. loop (first <= last)
    1. mid = (first + last) / 2
    2. if ( target > list[mid])
        `look in upper half`
        1. first = mid + 1
    3. else if (target < list[mid] )
        `look in lower half`
        1. last = mid - 1
    4. else 
        `found equal : force exit`
        1. first = last + 1
4. locn = mid
5. if (target == list[mid])
    1. found = true
6. else
    1. found = false
7. return found
```
