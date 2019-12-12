# midsquare method

In midsquare hashing, the key is squared abd the address selected from the middle of the squared number.<br/>
the limitation of this method is the key size.<br/>
given a key size of 6 digit , the product will be of 12 digit<br/>
so to counter this problem , we midsquare the key and select a portion from it say middle 3 digit.


example
```js
key = 9452

so , 9492 * 9452 = 89340304 

address is 3403
```

there are two folding methods<br/>
* fold shift -<br/>
key value is divided into equal parts , added and if the resulted value is greater than 999 , we discard the leading digit.


example
```js
key = 123456789

    123 456 789

    123
    456
  + 789
  -----
   1368

address is 368
```


* fold boundary -<br/>
key value is divided into equal parts , then individual parts are rotated and added, if the resulted value is greater than 999 , we discard the leading digit.


example
```js
key = 123456789

    321 654 987

    321
    654
  + 987
  -----
   1764

address is 764
```
