# Luna::BasicString::back

```c++
BasicString< _Char, _Alloc >::const_reference back() const
```

Gets the last character of the string. 

The last character is the character with index `size() - 1`. 

## Return value
Returns one constant reference to the last character of the string. 

## Valid Usage
* [empty](class_luna_1_1_basic_string_1a644718bb2fb240de962dc3c9a1fdf0dc.md) must be `false` when calling this function. 

