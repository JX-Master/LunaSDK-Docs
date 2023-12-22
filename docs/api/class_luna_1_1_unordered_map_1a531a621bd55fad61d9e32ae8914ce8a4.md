# Luna::UnorderedMap::UnorderedMap

```c++
UnorderedMap(UnorderedMap &&rhs, const allocator_type &alloc)
```

Constructs a map with an custom allocator and with elements moved from another map. 



## Parameters
* *in* **rhs**

    The map to move elements from. 

* *in* **alloc**

    The allocator to use. The allocator object will be copy-constructed into the map. 

