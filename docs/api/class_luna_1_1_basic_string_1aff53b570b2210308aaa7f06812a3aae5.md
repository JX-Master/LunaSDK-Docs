# Luna::BasicString::operator[]

```c++
BasicString< _Char, _Alloc >::reference operator[](usize n)
```

Gets the character at the specified index. 



## Parameters
* *in* **n**

    The index of the character. 

## Return value
Returns one reference to the character at the specified index. 

## Valid Usage
* [empty](class_luna_1_1_basic_string_1a644718bb2fb240de962dc3c9a1fdf0dc.md) must be `false` when calling this function.

* `n` must be in range [`0`, `size()`). 

