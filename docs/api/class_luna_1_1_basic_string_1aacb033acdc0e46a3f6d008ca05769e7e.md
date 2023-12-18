# Luna::BasicString::assign

```c++
void assign(const value_type *s)
```

Assigns the string data by coping characters from the provided null-terminated C string. The length of the string is determined by the first null character. 



## Parameters
* *in* **s**

    The pointer to one null-terminated string, where characters are copied from. 

## Valid Usage
* `s` must points to a valid null-terminated string. 

