# Luna::Span::Span

```c++
constexpr Span(InitializerList< remove_cv_t< _Ty > > ilist)
```

Constructs one span using the data provided by the specified initializer list. 



## Parameters
* *in* **ilist**

    The initializer list used. 

## Remark
This is only used to specify one initializer list for one [Span](class_luna_1_1_span.md) parameter of one function. Since the initializer list exists only in the expression evaluation scope, you can not refer one initializer list on one lvalue span (spans exist as local variables, member variables or global/static variables), or the behavior is undefined. 

## Valid Usage
* `ilist.size()` must be greater than or equal to `_Size`. 

