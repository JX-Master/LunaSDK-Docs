# Luna::BasicString::compare

```c++
i32 compare(const BasicString &rhs) const
```

Compares this string with the specified string. 



## Parameters
* *in* **rhs**

    The string to compare with. 

## Return value
Returns `0` if both character sequences compare equivalent.


Returns negative value if `*this` appears before the character sequence specified by `rhs`, in lexicographical order.

Returns positive value if `*this` appears after the character sequence specified by `rhs`, in lexicographical order. 

