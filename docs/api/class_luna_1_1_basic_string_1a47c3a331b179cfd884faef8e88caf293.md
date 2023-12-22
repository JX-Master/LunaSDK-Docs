# Luna::BasicString::compare

```c++
i32 compare(usize pos1, usize count1, const value_type *s, usize count2) const
```

Compares [`pos1`, `pos1 + count1`) substring of this string to the characters in the range [`s`, `s + count2`). 



## Parameters
* *in* **pos1**

    The index of the first character in `*this` to compare. 

* *in* **count1**

    The number of characters in `*this` to compare. If `pos1 + count1` is greater than `this->size()`, `count1` will be clamped to `this->size() - pos1`. 

* *in* **s**

    The string to compare with. 

* *in* **count2**

    The number of characters in `s` to compare. 

## Valid Usage
* `pos1` must not be greater than `this->size()`.

* If `count2` is not `0`, `s` must points to a valid character array with at least `count2` characters. 

