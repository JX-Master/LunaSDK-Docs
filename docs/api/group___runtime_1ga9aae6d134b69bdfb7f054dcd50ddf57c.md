# Luna::get

```c++
template <usize, typename...>
TupleElement< _I, Tuple< _Tys... > >::type & get(Tuple< _Tys... > &t)
```

Gets the `_I`th element from the tuple. 



## Parameters
* *in* **t**

    The tuple to extract element from. 

## Return value
Returns one lvalue reference to the element in the tuple. 

