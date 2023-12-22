# Luna::BasicString::append

```c++
void append(const value_type *s, usize count)
```

Appends one character array to the back of the string. 



## Parameters
* *in* **s**

    The pointer to the first character to append. 

* *in* **count**

    The number of characters to append. 

## Valid Usage
* If `count` is not `0`, `s` must points to a valid character array with at least `count` characters. 

