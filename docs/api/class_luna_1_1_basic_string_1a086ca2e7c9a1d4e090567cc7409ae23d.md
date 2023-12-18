# Luna::BasicString::insert

```c++
BasicString< _Char, _Alloc >::iterator insert(const_iterator pos, usize count, value_type ch)
```

Inserts `count` copies of `ch` at the specified position. 



## Parameters
* *in* **pos**

    The iterator to the position to insert. 

* *in* **count**

    The number of characters to insert. 

* *in* **ch**

    The character to insert. 

## Return value
Returns one iterator to the first inserted character. 

