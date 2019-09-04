## Probability search


It is one of the most useful variation of searching algorithm.<br/>
The array is ordered with the most probable seach element at the beginning probability<br/> of the array and the least probable at the end.<br/>

to ensure that the probability ordering is correct over time,in each search we exchange the located element<br/>
with element immediately before it in the array.


```javascript
list - array
last - index of last element
target - data to be stored
locn - address of index in calling the algorithm


1. looker = 1
2. loop ( looker < last && target !== list[looker])
    1. looker = looker + 1
3. if ( target == list[looker])
    1. found = true
    2. if (looker > 1)
        1. temp = list[looker - 1]
        2. list[looker - 1 ] = list[looker]
        3. list[looker] = temp
        4. looker = looker - 1
4. else
    1. found = false
5. locn = looker
6. return found

```
