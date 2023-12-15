# Luna::BasicString::c_str

```c++
BasicString< _Char, _Alloc >::const_pointer c_str() const
```

Unlike `data`, this call always returns a valid string, not `nullptr`, even if the string is empty. 

