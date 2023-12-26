# Luna::UnorderedMultiSet::insert

```c++
iterator insert(value_type &&value)
```

Inserts the specified value to the set. The key is extracted from the value. 



## Parameters
* *in* **value**

    The value to insert. The element is move-constructed into the set. 

## Return value
Returns one iterator to the inserted element. 

