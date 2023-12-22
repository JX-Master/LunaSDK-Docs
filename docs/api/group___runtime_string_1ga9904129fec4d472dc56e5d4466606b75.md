# Luna::strcmp

```c++
template <typename _CharT>
i32 strcmp(const _CharT *lhs, const _CharT *rhs)
```

Compares characters in two strings. 



## Parameters
* *in* **lhs**

    The first string to compare. 

* *in* **rhs**

    The second string to compare. 

## Return value
Returns `0` if both character sequences compare equivalent.


Returns negative value if `lhs` appears before the character sequence specified by `rhs`, in lexicographical order.

Returns positive value if `lhs` appears after the character sequence specified by `rhs`, in lexicographical order. 

## Valid Usage
* `lhs` and `rhs` must specify null-terminated strings. 

