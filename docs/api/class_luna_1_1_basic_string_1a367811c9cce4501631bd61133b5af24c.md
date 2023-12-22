# Luna::BasicString::erase

```c++
BasicString< _Char, _Alloc >::iterator erase(const_iterator pos)
```

Removes one character. 



## Parameters
* *in* **pos**

    The iterator to the character to remove. 

## Return value
Returns one iterator to the next character after the removed character, or `end()` if such character does not exist. 

## Valid Usage
* `pos` must specifies one valid character in the string. 

