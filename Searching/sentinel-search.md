## Sentinel Search

In sentinel search , you add an extra element at the end of the list.The target is added in the sentinel entry.<br/>
This eleminates the need of checking whether the element is present in the array or not.

```javascript
list - list must contain a sentinel at the end of the array.
last - index of the last element
target - data to be located
locn - addresss of index in calling algorithm

1. list[last + 1] = target
2. looker = 1
3. loop (target !== list[looker])
    1. looker = looker + 1
4. if ( looker  <= last)
    1. found = true
    2. locn = looker
5. else
    1. found = false
    2. locn = last
6. return found
```
