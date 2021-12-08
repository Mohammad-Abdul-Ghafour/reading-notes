# Hash Tables

* Data Structure used to store key-value information, allow fast retrieval of the data.
* Hash function gets a key and gives an index to where this key should be stored, the same key gives the same index.
* Finding a value takes the same time regardless of its location or the size of the array.
* The index of which is the value is stored can be calculated using the value itself.
* Sum up the ASCII code of the value and devide it to the size of the array, store the value at the index that equal the remaining.

![Image](https://miro.medium.com/max/1200/1*J7lzku84LsxaeXpbgqRy5Q.png)

## Vocabulary & Meaning

Vocabulary | meaning
---------|---------
Hash Table | Data Structure used to store key-value information, allow fast retrieval of the data
Chaining |In reatation
Collision |when two values have the same index when calculated
Hashing | Calculating the index from the value
Buckets | key-value pairs that are stored in an index

## Methods

1. **`Add()`** : to add a new key/value pair to a hash table
2. **`Find(key)`** : to find a value
3. **`Contains(key)`** : check if a value exists in the hash table, return a boolean.
4. **`GetHash(key)`** : to get the index to where this key should be saved.
