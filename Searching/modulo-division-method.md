# Modulo-division method

In this method we will divide the key by the array size and use the remainder as plus one for the address.

```
    address = key MODULUS listSize + 1
```

A list with prime number will produce fewer collisions than other list sizes.

Example : if we want to provide data space for upto 300 employees, we will find the first prime number <br/> greater than 300 which is 307.<br/>
we therefore choose 307 as our array list <br/>

```
employee id = 121267

121267 / 307 = 395 with remainder of 2
hash(121267) = 3

```