# Luna::BasicString::operator=

```c++
BasicString< _Char, _Alloc > & operator=(const value_type *s)
```

Assigns the string by coping characters from the provided null-terminated C string. The length of the string is determined by the first null character. 



## Parameters
* *in* **s**

    The pointer to the first character to copy. 

## Return value
Returns `*this`. 

## Valid Usage
* `s` must points to a valid null-terminated string. 

