What is a hastable?

Hash - A Hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either for security or some other purpose. In the case of a hashtable, it is used to determine the index of an array
Buckets - A bucket is what is contained in each index of the array of the hashtable - it can have multiple key/value pairs if a collision occurs
Collisions - a collision is what happens when more than one key gets hashed to the same location of the hashtable
We use them 
To hold unique values 
Dictionary
Library
More on hashtables 
Every node has a key and a value
Every node is a bucket
We use this to store the key in the data structure for easy retrieval 
We use what is called a hash to encode the key that will map to a specific location
Example : say we have a list of key value pairs with places and zipcodes and we want to return a certain zipcode. What we know is to for loop through it and go through each value but we can also use a faster approach

We can use hash tables to take a o(1) approach which is constant

The hash function takes a key and return an integer/ we use the integer to determine where the key/value pair should be placed in the array.

Breakdown
The hash code is used again to read something from the hash map
Take the key run it through the hash code to get a number
Use that number to index the array 
Calculating the hash code and reading the array at the index is all constant time to hash map has o(1) read access
A hash code turns a key into an integer. It's very important that hash codes are deterministic: their output is determined only by their input. Hash codes should never have randomness to them. The key should always produce the same hash code.
