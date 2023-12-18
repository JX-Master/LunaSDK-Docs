# Luna::BasicString::insert

```c++
void insert(usize index, const value_type *s, usize count)
```

Inserts one character array at the specified position. 



## Parameters
* *in* **index**

    The index to insert the characters. 

* *in* **s**

    The pointer to the first character to insert. 

* *in* **count**

    The number of characters to insert. 

## Valid Usage
* If `count` is not `0`, `s` must points to a valid character array with at least `count` characters. 

