# Luna::BasicString::insert

```c++
void insert(usize index, const BasicString &str, usize index_str, usize count=npos)
```

Inserts one subrange of another string at the specified position. 



## Parameters
* *in* **index**

    The index to insert the characters. 

* *in* **str**

    The string to insert. 

* *in* **index_str**

    The index of the first character in `str` to insert. 

* *in* **count**

    The number of characters to insert. If `count` is greater than `str.size() - index_str`, only `str.size() - index_str` characters will be inserted. 

