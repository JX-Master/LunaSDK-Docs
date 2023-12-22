# Luna::BasicString::erase

```c++
BasicString< _Char, _Alloc >::iterator erase(const_iterator first, const_iterator last)
```

Removes characters in the specified range. 



## Parameters
* *in* **first**

    The iterator to the first character to remove. 

* *in* **last**

    The iterator to the one-past-last character to remove. 

## Return value
Returns one iterator to the next character after the removed characters, or `end()` if such character does not exist. 

## Valid Usage
* `first` and `last` must specifies one valid character range [`first`, `last`) in the string. 

