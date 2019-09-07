## Hashed list Search

It is a search in which a key through an alorithmic function determinses the location of the list.<br/>
If we are using an array ,we use a hashing algorthim to transform the key into the index that contains the data we need to locate.<br/>

The population of the keys for a hashed list is greater than the storage area used to store the data.<br/>

because there are many keys for each index location in the array,there are chances that one element will hash to the same location in the array<br/>

Set of keys hash to the same location is called as synonyms.<br/>if the list have two or more synonyms then we <br/>will have collisions.A collision is an event that occurs when a hasing algorithm produces an address for an insertion key <br/>and that address is already occupied.

The address produced by the hashing algorithm is known as home address.

memory which contains all of the home address is called as prime area.