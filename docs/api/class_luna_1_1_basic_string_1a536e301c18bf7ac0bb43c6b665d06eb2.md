# Luna::BasicString::compare

```c++
i32 compare(const value_type *s) const
```

Compares this string to the null-terminated C string. 



## Parameters
* *in* **s**

    The null-terminated C string to compare with. 

## Return value
Returns `0` if both character sequences compare equivalent.


Returns negative value if `*this` appears before the character sequence specified by `rhs`, in lexicographical order.

Returns positive value if `*this` appears after the character sequence specified by `rhs`, in lexicographical order. 

