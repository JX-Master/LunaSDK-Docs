# Luna::BasicString::append

```c++
void append(const BasicString &str, usize pos, usize count=npos)
```

Appends one subrange of another string to the back of the string. 



## Parameters
* *in* **str**

    The string to append. 

* *in* **index_str**

    The index of the first character in `str` to append. 

* *in* **count**

    The number of characters to append. If `count` is greater than `str.size() - pos`, only `str.size() - pos` characters will be appended. 

