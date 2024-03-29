# Luna::UnorderedSet::insert_or_assign

```c++
template <typename _M>
Pair< iterator, bool > insert_or_assign(const key_type &key, _M &&value)
```

Assigns the value to the element with the specified key, or inserts the value pair to the set if such element is not found. The key is extracted from the value. 



## Parameters
* *in* **value**

    The element value to assign or insert. 

## Return value
Returns one iterator-bool pair indicating the result:* If the returned Boolean value is `true`, then the element is inserted to the set, and the returned iterator points to the inserted element.

* If the returned Boolean value is `false`, then one existing element is found and is assigned to the specified value, and the returned iterator points to the existing element in the set. 

