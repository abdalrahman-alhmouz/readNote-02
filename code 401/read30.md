# 401 Class-30: Hash Tables


## What is a Hashtable?
**Terminology:**

**Hash** - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.

**Buckets** - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.

**Collisions** - A collision is what happens when more than one key gets hashed to the same location of the hashtable.

## Why do we use them?
1. Hold unique values
2. Dictionary
3. Library

## What Are they
Hashtables are a data structure that utilize key value pairs. This means every `Node` or `Bucket` has both a key, and a value.

The basic idea of a hashtable is the ability to store the key into this data structure, and quickly retrieve the value. This is done through what we call a `hash`. A `hash` is the ability to encode the key that will eventually map to a specific location in the data structure that we can look at directly to retrieve the value.

Since we are able to `hash` our key and determine the exact location where our value is stored, we can do a lookup in an O(1) time complexity. This is ideal when quick lookups are required.



Introduction to hash tables

Key: Ethel
Value: phone #

    Hash(Key) -> index
O   Hash(Ethel) -> 3
[]  Hash(Person) -> 1
()  Hash(Somebody) -> 3 (how to avoid collision is to create a linked list off of the indexes) 


## Hashing is implemented in two steps:

1. An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
2. The element is stored in the hash table where it can be quickly retrieved using hashed key.
```
hash = hashfunc(key)
index = hash % array_size
```




