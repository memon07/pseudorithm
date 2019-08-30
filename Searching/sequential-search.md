## sequential search

It is used whenever the list is not ordered. It is used only for small lists.

In sequential search we start searching for the target at the beginning of the list and continue until we find the target <br/> or we are sure that it is not in the list.

In sequential search you need to tell the calling algorithm two things:<br/>
1.did it find the data it was looking for ?<br/>
2.if its found , what is the index of the element ?<br/>


Algorithm requires 5 parameters :<br/>
1.the list.<br/>
2.index of the last element in the list.<br/>
3.the target.<br/>
4.the address where the found element's index location is to be stored.<br/>
5.address where boolean found or not found will be stored.<br/>



```javascript
list - array
last - index of last element
target - data to be stored
locn - address of index in calling the algorithm


1. looker = 1
2. loop (looker < last AND target !== list[looker] )
    1. looker = looker + 1
3. locn = looker
4. if ( target == list[looker])
    1. found true
5. else
    1. found = false
6. return found
```
