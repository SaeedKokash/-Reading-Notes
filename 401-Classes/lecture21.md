# Readings: Hash Tables #

## OSL Model ##

### What is Hash Tables ###
A hash table is an implementation of an associative array, a list of key-value pairs that allow you to retrieve a value via a key. Internally a hash table utilizes a hash function to transform a key value into an index that points to where the value is stored in memory. Hash tables have fast search, insertion and delete operations.

The Hash table data structure stores elements in key-value pairs where

- Key- unique integer that is used for indexing the values
- Value - data that are associated with keys.

![image2](https://cdn.programiz.com/sites/tutorial2program/files/Hash-0.png)

### Hashing (Hash Function) ###
In a hash table, a new index is processed using the keys. And, the element corresponding to that key is stored in the index. This process is called hashing.

### Hash Collision ###
When the hash function generates the same index for multiple keys, there will be a conflict (what value to be stored in that index). This is called a hash collision.

We can resolve the hash collision using one of the following techniques.

- **Collision resolution by chaining**, if a hash function produces the same index for multiple elements, these elements are stored in the same index by using a doubly-linked list.
- **Open Addressing: Linear/Quadratic Probing and Double Hashing**, Unlike chaining, open addressing doesn't store multiple elements into the same slot. Here, each slot is either filled with a single key or left NIL.

### Applications of Hash Table ###
Hash tables are implemented where

- constant time lookup and insertion is required
- cryptographic applications
- indexing data is required

<hr>

There are two main ways to implement a hash table/associative array in JavaScript.

### Using the Object Data Type ###

```
var simplehash = new Object();
// or
// var simplehash = {};

simplehash['key1'] = 'value1';
simplehash['key2'] = 'value2';
simplehash['key3'] = 'value3';

for (var key in simplehash) {
  // use hasOwnProperty() to filter out properties from Object.prototype
  if (simplehash.hasOwnProperty(key)) {
    console.log('key is: ' + key + ', value is: ' + simplehash[key]);
  }
}

the output would be:

key is: key1, value is: value1
key is: key2, value is: value2
key is: key3, value is: value3
```
### Using a Map Object ###
The Map object was created to implement this type of associative array without some of the downsides of using a basic Object:

There are no pre-existing keys that could result in a collision
- A Map object has a size property to track its contents.
- A Map object can have keys that are any data type.
- A Map has been optimized for repeated addition and insertion of key-value pairs.

A Map object also comes with the following methods:

- .clear() Removes all key-value pairs from the Map object.
- .delete(key) Deletes the key-value pair and returns true if the key exists. Returns false otherwise.
- .get(key) Returns the value associated with key, or undefined if key doesn’t exist.
- .has(key) Returns true if key exists, false otherwise.
- .set(key,value) Sets the value for the key in the Map object and returns the Map object.

```
var maphash = new Map();

maphash.set('key1', 'value1');
maphash.set('key2', 'value2');
maphash.set('key3', 'value3');

console.log(maphash.get('key3'));
// Output: value3

maphash.set('key1', 'new value');

console.log(maphash.get('key1'));
// Output: new value

console.log(maphash.size);
// Output: 3

maphash.delete('key2');

console.log(maphash.size);
// Output: 2

for (const [key, value] of maphash) {
  console.log(key + ' = ' + value);
}
// Output: key1 = new value
//         key3 = value3
```
### *[Source01](https://www.programiz.com/dsa/hash-table)*  *[Source02](https://www.codecademy.com/resources/docs/javascript/hashtables)*
