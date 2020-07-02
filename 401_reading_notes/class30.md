# Hash Tables

***What Is Hashing?***

Hashing is a technique that is used to uniquely identify a specific object from a group of similar objects.

In other words, hashing is the process of **creating a unique identifier**. This is done through the use of a predefined function that, given the same input, will always produce the same output.

Hash maps take advantage of an array’s O(1) read access. Instead of adding elements to an array from beginning to end, a hash map uses a “hash function” to place each item at a precise index location, based off it’s key.

**It’s very important that hash codes are deterministic: their output is determined only by their input. Hash codes should never have randomness to them. The same key should always produce the same hash code.**

 The idea of hashing is to distribute entries (key/value pairs) uniformly across an array. Each element is assigned a key (converted key). By using that key you can access the element in O(1) time. Using the key, the algorithm (hash function) computes an index that suggests where an entry can be found or inserted.

**Hashing is implemented in two steps:**

1. An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
2. The element is stored in the hash table where it can be quickly retrieved using hashed key.

## Internal Methods
* Add()
* Find()
* Contains()
* GetHash()