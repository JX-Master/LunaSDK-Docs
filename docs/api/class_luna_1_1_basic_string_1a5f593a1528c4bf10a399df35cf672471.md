# Luna::BasicString::resize

```c++
void resize(usize n, value_type v)
```

Resizes the string. 



## Parameters
* *in* **n**

    The new size of the string.


If `n` is greater than [size](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md), `n - size()` copied of `v` will be inserted to the back of the string.

If `n` is smaller than [size](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md), `size() - n` characters will be removed from the back of the string.

If `n` is equal to [size](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md), this function does nothing. 

## Parameters
* *in* **v**

    The character to insert if `n` is greater than [size](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md). 

