# Luna::BasicString::replace

```c++
void replace(const_iterator first, const_iterator last, const value_type *cstr, usize count2)
```

Replaces characters in range [`first`, `last`) with a character array [`cstr`, `cstr + count2). @param[in] first The iterator to the first character to replace. @param[in] last The iterator to the one-past-last character to replace. @param[in] cstr The pointer to the character array to use for replacement. @param[in] count2 The number of characters in`cstr`to use for replacement. @par Valid Usage. `

* [first`,`last`) must specify a valid range of this string. 

