# C Hash Table

## Overview

Hash tables, arguably the single most important data structures in computer science, provide efficient key-value storage. This C implementation offers a robust hash table, tailored for diverse applications.

## What is a Hash Table?

Underneath the hood, a hash table is simply an array with its elements indexed by a hashed key. Like arrays, hash tables are initialized to a fixed size, and inserting, deleting, and reading elements within those boundaries can be accomplished in constant time, or O(1).

![Hash Table](img/HashTableImage.png)

In this diagram, you can see the key (a string) is run through a hash function which produces an integer 0-15 that is used as the index in a 16-element array.

## What is a Hash Function?

A hash function maps data of arbitrary size to data of a fixed size. For example, a size-16 hash function might hash string-typed keys like so:

- `"foo"` -> `10`
- `"bar"` -> `12`
- `"baz"` -> `5`
- `"Hello world!"` -> `6`
- `"Very long keys can be hashed as well"` -> `10`

In this way, keys of any length can be mapped to an integer value which is used as an array index for a hash table. Note that since there are an infinite amount of possible keys that must map to only 16 possible indices, values with different keys will inevitably collide.

## Key Concepts

- **Dynamic Indexing:** Utilizes a dynamic array structure with constant time complexity for critical operations.
- **Hashing Algorithm:** Employs a hash function to map keys to indices, ensuring fast data retrieval.
- **Collision Handling:** Addresses collisions through linked list chaining, ensuring seamless performance.

## Features

- **Essential Operations:** Supports core functions - insertion, reading, and deletion.
- **Collision Management:** Implements a linked list chaining mechanism for handling collisions effectively.
- **Dynamic Resizing:** Ensures optimal performance with dynamic resizing, preventing performance bottlenecks.


