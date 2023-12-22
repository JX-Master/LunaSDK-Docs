# Luna::BasicString::compare

```c++
i32 compare(usize pos1, usize count1, const BasicString &rhs, usize pos2, usize count2=npos) const
```

Compares a [`pos1`, `pos1 + count1`) substring of this string to a substring [`pos2`, `pos2 + count2`) of `rhs`. 



## Parameters
* *in* **pos1**

    The index of the first character in `*this` to compare. 

* *in* **count1**

    The number of characters in `*this` to compare. If `pos1 + count1` is greater than `this->size()`, `count1` will be clamped to `this->size() - pos1`. 

* *in* **rhs**

    The string to compare with. 

* *in* **pos2**

    The index of the first character in `rhs` to compare. 

* *in* **count2**

    The number of characters in `rhs` to compare. If `pos2 + count2` is greater than `rhs.size()`, `count2` will be clamped to `rhs.size() - pos2`. 

## Return value
Returns `0` if both character sequences compare equivalent.


Returns negative value if `*this` appears before the character sequence specified by `rhs`, in lexicographical order.

Returns positive value if `*this` appears after the character sequence specified by `rhs`, in lexicographical order. 

## Valid Usage
* `pos1` must not be greater than `this->size()`.

* `pos2` must not be greater than `rhs.size()`. 

