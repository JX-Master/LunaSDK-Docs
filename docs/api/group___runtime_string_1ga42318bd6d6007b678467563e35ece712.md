# Luna::strncmp

```c++
template <typename _CharT>
i32 strncmp(const _CharT *lhs, const _CharT *rhs, usize max_chars)
```

Compares at most `max_chars` characters in two strings. 



## Parameters
* *in* **lhs**

    The first string to compare. 

* *in* **rhs**

    The second string to compare. 

* *in* **max_chars**

    The maximum number of characters to compare. 

## Return value
Returns `0` if both character sequences compare equivalent, or if `max_chars` is `0`.


Returns negative value if `lhs` appears before the character sequence specified by `rhs`, in lexicographical order.

Returns positive value if `lhs` appears after the character sequence specified by `rhs`, in lexicographical order. 

