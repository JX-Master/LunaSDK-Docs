# Luna::BasicString::insert

```c++
void insert(usize index, const value_type *s)
```

Inserts one null-terminated C string at the specified position. 



## Parameters
* *in* **index**

    The index to insert the characters. 

* *in* **s**

    The pointer to one null-terminated string, where characters are copied from. 

## Valid Usage
* `s` must points to a valid null-terminated string. 

