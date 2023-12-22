# Luna::BasicString::compare

```c++
i32 compare(usize pos1, usize count1, const BasicString &rhs) const
```

Compares [`pos1`, `pos1 + count1`) substring of this string to `rhs`. 



## Parameters
* *in* **pos1**

    The index of the first character in `*this` to compare. 

* *in* **count1**

    The number of characters in `*this` to compare. If `pos1 + count1` is greater than `this->size()`, `count1` will be clamped to `this->size() - pos1`. 

* *in* **rhs**

    The string to compare with. 

## Return value
Returns `0` if both character sequences compare equivalent.


Returns negative value if `*this` appears before the character sequence specified by `rhs`, in lexicographical order.

Returns positive value if `*this` appears after the character sequence specified by `rhs`, in lexicographical order. 

## Valid Usage
* `pos1` must not be greater than `this->size()`. 

