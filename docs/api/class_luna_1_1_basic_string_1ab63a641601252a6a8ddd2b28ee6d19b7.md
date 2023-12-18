# Luna::BasicString::c_str

```c++
BasicString< _Char, _Alloc >::const_pointer c_str() const
```

Gets a non-modifiable C string pointer to the characters stored by this string. 

Unlike `data`, this call always returns a valid string, not `nullptr`, even if the string is empty.

## Return value
Returns the C string pointer to the characters stored by this string. The returned pointer will never be `nullptr`. If this string is empty, one valid pointer to a null character is returned. 

