## Ordered list Search

When searching an ordered list sequntially , it is not necessary to search to the end <br/>
of the list to determine if the target is in the list or not . We can stop when the target becomes less<br/>
than or equal to the element in the list.

we can use the sentinel concept here too, when the target is greater than the last element then the last <br/>
element become the sentinel allowing us to eleminate the test for the end of the list.

```javascript
list - array
last - index of last element
target - data to be stored
locn - address of index in calling the algorithm

1. if ( target < = list[last])
    1. looker = 1
    2. loop ( target > list[looker])
        1. looker = looker + 1
2. else
    1. looker = last
3. if ( target == list[looker])
    1. found = true
4. else
    1. found = false
5. locn = looker
6. return found
```
