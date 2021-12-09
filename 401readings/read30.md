# hash tables

hashs are made primerly for securety resons 
it is a list of key (bucket) and value pairs

- internal methods are: add, find, contains, gethash.
- Lookup in a hash table is extremely fast for large tables—in fact, the time required is essentially independent of how many elements are stored in the table. For smaller tables (a few tens of elements) alists may still be faster because hash tables have a more-or-less constant overhead.
- The correspondences in a hash table are in no particular order.
- There is no way to share structure between two hash tables, the way two alists can share a common tail.
- hashs help a lot in terms of big O for many problems.

