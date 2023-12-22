# Luna::UnorderedMultiMap::insert

```c++
iterator insert(value_type &&value)
```

Inserts the specified value to the map. The key is extracted from the value. 



## Parameters
* *in* **value**

    The value to insert. The element is move-constructed into the map. 

## Return value
Returns one iterator to the inserted element. 

