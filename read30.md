# HashTables : 

* *Hash* : is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array

* Hashing is implemented in two steps:

1. An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
2. The element is stored in the hash table where it can be quickly retrieved using hashed key.

`hash = hashfunc(key)
index = hash % array_size`
* *Hash function* : is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size,

* *Buckets* : is what is contained in each index of the array of the hashtable.

* *Collisions* :  is what happens when more than one key gets hashed to the same location of the hashtable.

#### HashTable: are a data structure that utilize key value pairs.

 ###### if two keys resolve to the same index in the array then their key/value pairs can be stored as a node in a linked list.

 ###### Each index in the array is called a`bucket` because it can store multiple key/value pairs.










