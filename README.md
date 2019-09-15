## Searching 

Searching is the most common and time consuming technique.

* [Linear search](Searching/linear-list-search.md)<br/>
    There are two basic searches for array , the sequential search and the binary search.

    * [Sequential search](Searching/sequential-search.md)
        There are 3 types of sequential search:
        * [The sentinel search](Searching/sentinel-search.md)
        * [The probability search](Searching/probability-search.md)
        * [The ordered list search](Searching/ordered-list-search.md)
    * [Binary search](Searching/binary-search.md)
    * [Hashed list search](Searching/hashed-list-search.md)
        * [direct hashing](Searching/direct-hashing.md)
        * [subtraction method](Searching/subtraction-method.md)

Measuring algorithm's efficiency
## Big-O Notation

If we want to measure the efficiency between two algorithms in which one has 25 iterations and other has 45 iterations, we won't be able to differentiate as both will be executed fast.

But if one iterates 10 times and the other 1000 times then we have to create some measurements to check the eficiency.

> text book definition :
 The number of statements executed in the function for n elements of data is a function of the number of elements, expressed as f(n).
 We don't need to determine the complete measure of effeciency,only the factor that determines the magnitude.this factor is big-O.
 
 The Big-O notation can be derived from f(n) using the below steps:
 1. In each term set the coefficient of the term to one.
 2. Keep the largest term in the function and discard the others.
  
  
 Terms ranked from highest to lowest :
### logn .. n ..  nlogn .. n^2 .. n^3  ............ n^k  .. 2^n .. n!



There are 7 categories defined for alogrith efficiency.below is the table displaying the 7 categories.



| Efficiency | Big-O | Iterations | Est Time |
| ------------- |:-------------:| :-----:| ----: |
| Logarithmic | O(log n) | 14 | microseconds |
| linear | O(n) | 10,000 | .1 seconds |
| linear logarithmic | O(n(log n)) | 140,000 | 2 seconds |
| quadratic | O(n^2) | 10,000^2 | 15-20 min. |
| polynomial | O(n^k) | 10,000^k | hours |
| exponential | O(c^n) | 2^10,000 | intractable |
| factorial | O(n!) | 10,000! | intractable |




![big O range](./images/bigochart.jpeg "Big O range")


```
 based on Data Structures - A Pseudocode approach with C 
 ```
