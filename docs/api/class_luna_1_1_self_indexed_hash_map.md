# Luna::SelfIndexedHashMap
```c++
class Luna::SelfIndexedHashMap
```

## Overview
The self indexed hash map is for values whose key is one data member of the value, or can be computed from the value. For every value type that the user want to use for self indexed hash map, the user must define one special structure called "key extractor", and passes the type as the `_ExtractKey` template argument for the map. In this structure, one operator function `const _Kty& operator()(const _Ty& p) const` (or `_Kty operator()(const _Ty& p) const` if the key is computed from value) must be defined to fetch the key of the value.

The user must ensure that the key data member is not changed after the element is inserted to the map and before the element is removed from the map, or the behavior is undefined. 

