# Luna::BasicString
The string template used by String, String16 and String32. 

```c++
class Luna::BasicString
```

## Functions
* [BasicString< _Char, _Alloc >::pointer data()](class_luna_1_1_basic_string_1abbe2708e47e4589174382b703afa3f15.md)

    May returns `nullptr` if the string is empty. 

* [BasicString< _Char, _Alloc >::const_pointer c_str() const](class_luna_1_1_basic_string_1ab63a641601252a6a8ddd2b28ee6d19b7.md)

    Unlike `data`, this call always returns a valid string, not `nullptr`, even if the string is empty. 

