# Luna::BasicString::data

```c++
BasicString< _Char, _Alloc >::pointer data()
```

Gets one pointer to the underlying character data. 

May returns `nullptr` if the string is empty.

## Return value
Returns one pointer to the underlying character data. The returned pointer may be `nullptr` if the string is empty, to ensure one non-null return value, use [c_str](class_luna_1_1_basic_string_1ab63a641601252a6a8ddd2b28ee6d19b7.md) instead, which always return one valid but empty string buffer ("") if the string is empty. 

