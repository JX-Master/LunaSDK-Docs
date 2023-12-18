# Luna::SelfIndexedUnorderedMap::insert

```c++
Pair< iterator, bool > insert(const value_type &value)
```

Inserts the specified value to the map. The key is extracted from the value. 



## Parameters
* *in* **value**

    The value to insert. The element is copy-constructed into the map. 

## Return value
Returns one iterator-bool pair indicating the insertion result:* If the returned Boolean value is `true`, then the element is successfully inserted to the map, and the returned iterator points to the inserted element.

* If the returned Boolean value is `false`, then the insertion is failed because another element with the same key already exists, and the returned iterator points to the existing element in the map. 

