# Hash Tables

A hash table (hash map) is a data structure that implements an associative array abstract data type, a structure that can map keys to values. A hash table uses a hash function to compute an index, also called a hash code, into an array of buckets or slots, from which the desired value can be found. During lookup, the key is hashed and the resulting hash indicates where the corresponding value is stored.

![](https://hughewilliams.files.wordpress.com/2012/09/450px-hash_table_5_0_1_1_1_1_1_ll-svg.png?w=584)


- Hash table operations are performed in two steps:
    - A key is converted into an integer index by using a hash function.
    - This index decides the where the key-value pair record belongs.

- Note: Although hash tables provide fast insertion, deletion, and retrieval, they perform poorly for operations that involve searching, such as finding the minimum and maximum values in a data set. For these operations, other data structures such as the binary search tree are more appropriate.

- Hashing is a technique to convert a range of key values into a range of indexes of an array.

- Collision-Resolution
Even with an efficient hash function, it is possible for two keys to hash (the result of the hash function) to the same value. This is called a collision, and we need a strategy for handling collisions when they occur.

- A hash function is any function that can be used to map a data set of an arbitrary size to a data set of a fixed size, which falls into the hash table. The values returned by a hash function are called hash values, hash codes, hash sums, or simply hashes.

    - Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
    - Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
    - Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

- Hashing is a technique that is used to uniquely identify a specific object from a group of similar objects.

###  Methods
- put(key, value): Adds a new key-value pair to the hash table.

- get(key): Gets the value associated with a key.

- remove(key): Removes the key-value pair from the table.

- forEach(): Allows iterating over all key-value pairs.

- static join(): A static method to join 2 hash tables in a new one.

### Resources
- [HashTable](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)