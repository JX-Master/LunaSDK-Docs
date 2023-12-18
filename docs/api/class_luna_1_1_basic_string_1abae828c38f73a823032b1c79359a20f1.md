# Luna::BasicString::assign

```c++
void assign(const value_type *s, usize count)
```

Assigns the string data by coping characters from the provided character array. 



## Parameters
* *in* **s**

    The pointer to the first character to copy. 

* *in* **count**

    The number of characters to copy. 

## Valid Usage
* If `count` is not `0`, `s` must points to a valid character array with at least `count` characters. 

