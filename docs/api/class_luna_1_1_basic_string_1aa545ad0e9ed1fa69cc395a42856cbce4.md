# Luna::BasicString::erase

```c++
void erase(usize index=0, usize count=npos)
```

Removes `count` characters from the specified position. 



## Parameters
* *in* **index**

    The index of the first character to remove. 

* *in* **count**

    The number of characters to remove. If `count` is greater than `size() - index`, only `size() - index` characters will be removed. 

