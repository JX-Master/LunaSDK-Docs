# Luna::BasicString::replace

```c++
void replace(usize pos, usize count, const value_type *cstr, usize count2)
```

Replaces characters in range [`pos`, `pos + count`) with a character array [`cstr`, `cstr + count2). @param[in] pos The index of the first character to replace. @param[in] count The number of characters to replace. If`pos + count`is greater than`this->[size()](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md)`,`count`will be clamped to`this->[size()](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md) - pos`. @param[in] cstr The pointer to the character array to use for replacement. @param[in] count2 The number of characters in`cstr`to use for replacement. @par Valid Usage *`pos`must not be greater than`this->[size()](class_luna_1_1_basic_string_1a79348f1b7c06b34052b42656a0279429.md)`. 

